# Proposed pilot protocol

**Status: DRAFT — advisor proposal, not an author-confirmed protocol or a completed analysis.**
Prepared 2 November 2026. No data have been downloaded or analyzed.

## Goal and estimand

Assess whether shallow liquid-cloud microphysical properties are associated with aerosol exposure over Bangladesh's coastal outflow and the northern Bay of Bengal after accounting for measured environmental covariates and retrieval selection.

The first estimand is a **conditional observational association** within the sampled cloud regime. It is not a causal ACI effect, an attribution of rainfall change, or anthropogenic radiative forcing.

Recommended primary responses: cloud droplet effective radius and cloud optical thickness, analyzed separately. Estimated droplet number concentration (Nd) is secondary because of retrieval assumptions and error amplification.

## Proposed pilot domain and dates

- Mapping/transport domain: 18–27°N, 85–94°E.
- Initial marine cloud analysis box: 18–22°N, 87–92°E; keep only marine pixels using an explicit land mask.
- Coast-distance exclusions: compare no extra exclusion with 25 km and 50 km buffers where retrievals permit. These are proposed sensitivity settings, not validated optimal thresholds.
- Winter pilot: 1 December 2018–28 February 2019.
- Pre-monsoon pilot: 1 March–30 April 2019, analyzed separately.
- Proposed expansion: 2010–2021, only after the coverage audit and specification freeze.
- Optional modern case: January–February 2025 haze, analyzed as a separate sensor/overpass epoch. Never append an uncalibrated modern VIIRS/PACE/EarthCARE record to MODIS as if it were one sensor.

These dates prioritize a compact historical pilot with mature archives and reduce sensitivity to later orbital drift. They do not imply that older years are scientifically preferable for all questions.

## Minimum acquisitions

1. Aqua MODIS MYD06_L2 Collection 6.1 cloud properties plus MYD03 geolocation if required by the reader; record the collection and production timestamps.
2. MYD04_L2 Collection 6.1 ocean aerosol retrievals for clear-air aerosol context. Treat clear-air aerosol and cloudy-pixel observations as different samples.
3. ERA5 hourly pressure/single-level meteorology, subset to the domain and relevant overpass and preceding hours.
4. MERRA-2 M2T1NXAER hourly aerosol optical diagnostics, or CAMS EAC4 3-hourly aerosol fields. Start with one and use the second as a sensitivity extension if feasible.
5. IMERG Final V07 for rain context only if precipitation separation becomes part of the locked design.

Do not download a global multidecadal archive initially. Discover granules first; estimate actual file sizes, available RAM/disk, download throughput and regional subset options.

## Acquisition and provenance record

For every input file or remotely accessed subset, retain:
- Provider, collection shortname, version and processing/revision date.
- Granule ID or dataset request ID; source URL without authentication material.
- Actual observation start/end time in UTC and native spatial support.
- Download/access date, byte count and SHA-256 after acquisition.
- Bounding box, variable names, levels, units and API/subset request.
- License/use conditions and the official dataset citation.
- Any incomplete transfer, retry, missing file or service failure.

A zero-row [manifest template](../data/manifest.csv) is supplied. Populate it only with real acquisitions. Never describe a planned product or missing file as downloaded.

## Quality-control sequence

1. **Decode first.** Verify fill values, scale/offset and QA bit fields against the exact product guide. Check units after decoding, not from plausible numeric ranges.
2. **Map coverage before relationships.** Count valid aerosol/cloud/meteorology observations by day, cell, phase and filter stage. Map missingness and count independent overpass-days as well as pixels.
3. **Define the cloud regime.** Use confidently liquid, shallow clouds; start with cloud top below about 3 km and above-freezing cloud-top temperature, then test alternate definitions. Exclude multilayer/ice/cirrus-contaminated scenes where flags permit. Height/pressure assumptions and top-temperature uncertainties must be retained.
4. **Screen retrieval geometry.** Use successful, high-quality cloud optical retrievals. Proposed sensitivity settings include optical thickness >=5, solar zenith <65° and view zenith <55°; confirm suitability against the retrieval guide. Thin/broken/cloud-edge scenes need a separately documented sensitivity analysis. Retain sample attrition counts for every filter.
5. **Separate sample definitions.** A high-cloud-fraction, near-overcast subset may be suitable for Nd estimation. Never use this outcome-selected subset to estimate the aerosol effect on cloud fraction. Define cloud fraction from a separate cloud-mask sampling population.
6. **Collocate at observation time.** Use actual pixel/scan timestamps and interpolate meteorology in time. Keep Aqua and Terra separate initially. Do not substitute daily averages for instantaneous retrieval conditions without testing the effect.
7. **Keep footprints honest.** Store native supports, then create a transparent aggregate (initially 0.5° cell–overpass summaries as a practical proposal). MERRA-2/CAMS repeated across finer cells does not create additional independent aerosol information. Test 0.25°, 0.5° and 1° summaries only with support-aware interpretation.
8. **Do not fill cloudy AOD blindly.** Record the distance/time from clear-air AOD to cloud observations. Compare feasible neighboring/upwind/preceding exposures; use reanalysis as modeled exposure, not as an observed AOD fill indistinguishable from satellite data.

## Atmospheric controls and causal diagram

Write a small directed acyclic graph before fitting:
- Prior humidity, stability, circulation, SST and surface/season can affect both aerosol exposure and clouds.
- Aerosols can affect cloud microphysics, water, precipitation and perhaps stability.
- Clouds and precipitation affect aerosol retrieval and removal.
- Cloud cover and retrieval success influence which observations enter the dataset.

Candidate controls: preceding-hour temperature/humidity profiles, lower-tropospheric stability or estimated inversion strength, SST, wind speed/direction, boundary layer height, large-scale ascent and season/location. Use physical reasoning to choose these, not automated p-value selection.

**Mediators and selection:** same-time stability can be on an aerosol-heating pathway; cloud LWP and cloud fraction can be aerosol responses. Conditioning on these changes the question and can introduce bias. Present models with clearly stated conditioning sets. Do not add current LWP to a model claiming to estimate a total aerosol effect. A fixed-LWP microphysical sensitivity is a different, explicitly conditional analysis.

## Analysis plan

1. Plot seasonal distributions and joint coverage, including unavailable days.
2. Plot unadjusted exposure–response relationships as diagnostics, with no causal labels.
3. Match/stratify measured prior meteorology and season; check overlap and covariate balance. Do not extrapolate high-AOD cases into weather conditions lacking cleaner matches.
4. Fit transparent regression or generalized additive models for log(radius) and log(optical thickness), with spatial and seasonal terms. Report response curves, effect sizes and uncertainty.
5. Analyze estimated Nd only after documenting the adiabatic-cloud assumptions. Its common form is proportional to sqrt(optical thickness) times effective_radius^(-2.5); radius errors are therefore strongly amplified.
6. Keep retrieved LWP and Nd relationships descriptive unless mathematical coupling and correlated retrieval errors have been assessed. They share retrieval inputs and cannot independently validate each other.
7. Use spatial/temporal blocked validation and bootstrap blocks based on diagnosed dependence (e.g. synoptic episodes/overpass-days). Pixels from one scene are not independent replicates.
8. Hold out complete years/episodes and spatial blocks after expansion. Random pixel train/test splits are unsuitable.
9. If using ML, compare with the transparent baseline. SHAP values are predictive attributions, not causal effects.
10. Apply multiplicity control to exploratory maps, or label them exploratory and prioritize predeclared regional contrasts.

## Robustness checks

- Alternate aerosol exposure: observed ocean AOD, MERRA-2 and CAMS. Report shared assimilated observations.
- Alternate meteorological conditioning sets, with clear estimand changes.
- Coastal/cloud-edge buffers, QA filters, grid scale and collocation windows.
- Exposure timing (preceding/upwind versus same-time), acknowledging persistent-weather confounding.
- Winter versus pre-monsoon and liquid-cloud regime definitions.
- Rain history: wet scavenging can reverse apparent exposure–response directions; IMERG absence of rain does not prove absence of drizzle.
- Aerosol vertical placement on available CALIOP tracks; retain attenuated/unknown cases.
- Leave-one-year/episode-out influence checks.
- Placebo dates/exposure shifts appropriate to the design. Autocorrelation can make even a placebo association nonzero.
- Compare retained and excluded observations; selection bias cannot be declared solved because a regression includes humidity.

## Pilot decision

Proceed to the multiyear analysis only if:
- Both relatively low and high aerosol exposures have adequate coverage within comparable weather/cloud regimes.
- Effective sample size, assessed by independent days/episodes, supports a useful precision target.
- Conclusions are not driven by one event, a retrieval edge case or a single aerosol product.
- The principal result survives reasonable filtering, or instability itself is a clear and reproducible methodological result.

Set a minimum scientifically useful effect and estimate detectable effects after auditing variance and dependence; do not choose a sample-size cutoff solely from the raw number of pixels. If clouds are too sparse in winter, revise the season/domain transparently before the main analysis. A well-constrained null is a legitimate outcome.

## Expected outputs, not results

1. Availability and missingness maps.
2. QA attrition table and independent-day counts.
3. Aerosol/cloud/weather distributions.
4. Matched-sample balance and common-support plots.
5. Unadjusted versus adjusted response curves.
6. Product/filter/scale sensitivity plots.
7. A short diagnostic slide deck explaining findings, limitations and the next decision.

No result values or charts should be generated without real input data. Prepare any manuscript only after these outputs have been checked.

## Limits of this planning session

The execution environment is unavailable. File decoding, downloads, sample counts, data licensing, field names, memory requirements and analysis code have not been tested. NASA Earthdata and Copernicus accounts may be needed; no credential setup has been attempted.
