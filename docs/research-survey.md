# Research survey and feasible directions

Prepared 2 November 2026. This is a targeted literature-based advisory survey, covering 2020–2026, not a systematic review and not an empirical result. Full citations and reading scopes are in [literature.md](literature.md) and [references.bib](../references.bib).

## Recommendation

Begin with **meteorology-adjusted aerosol–liquid-cloud associations over the northern Bay of Bengal and Bangladesh coastal outflow**. Add aerosol vertical structure as a focused extension if coverage permits. Treat deep-convective invigoration and anthropogenic radiative forcing as later questions requiring stronger evidence.

A candidate question is: **Under comparable weather conditions, how do shallow liquid-cloud droplet size and optical thickness differ between relatively polluted and cleaner air masses reaching the northern Bay of Bengal, and how sensitive are the findings to aerosol proxy, vertical placement, and satellite sampling?**

This is an advisor-proposed question, not an author-approved final study or a claim of novelty.

## Physical interpretation

Cloud droplets form on suitable aerosol particles called cloud condensation nuclei (CCN), when cooling produces enough supersaturation. At comparable liquid water, increasing activated droplet number usually reduces droplet size and raises optical thickness: the Twomey brightening effect. Activation depends on particle size/composition and cloud-base updrafts, so aerosol mass or AOD alone cannot determine droplet number.

Cloud liquid water and cloud coverage can then adjust. Suppressed collision–coalescence can delay rain, while stronger evaporation and mixing of dry air can reduce cloud water. Absorbing aerosol also heats the atmosphere and changes stability. Its placement above, within, or below clouds matters. Therefore, more aerosol does not universally imply more cloud, more rain, or brighter scenes.

Separate three quantities:
- **Cloud optical reflectivity/albedo:** how much sunlight a cloud reflects.
- **Radar reflectivity:** a hydrometeor-size/concentration-dependent radar measurement, strongly affected by larger particles.
- **Vertical air velocity:** upward/downward motion of air. Neither reflectivity nor cloud-top temperature measures it directly. EarthCARE Doppler velocity also includes hydrometeor fall speed and needs careful interpretation.

A regional cloud radiative effect anomaly is not automatically anthropogenic effective radiative forcing. Historical forcing requires an anthropogenic counterfactual, normally using additional model experiments and radiative diagnostics. See [IPCC AR6 Chapter 7](https://www.ipcc.ch/report/ar6/wg1/chapter/chapter-7/), Bellouin (2020), Stier (2024), and Im (2026).

## Locations and recent events

| Location/event | Scientific opportunity | Main limitation | Recommendation |
|---|---|---|---|
| Bangladesh coast and northern Bay of Bengal; recurring winter haze, including January–February 2025 | Continental-to-marine transport; seasonal changes in cloud regime; land/ocean contrast | Humidity, inversions, cloud contamination and aerosol height can mimic an ACI signal | Best local starting region; begin with one shallow-liquid-cloud regime |
| Bay of Bengal shipping corridors; IMO2020 sulfur regulation | An identifiable emission-policy change and spatial exposure gradient | Existing 2025 lightning study; COVID-era shipping changes, global regulation, meteorology and drift complicate controls | Feasible higher-risk extension focused on liquid clouds and robustness |
| Southeast Atlantic shipping corridor; IMO2020 | Published counterfactual method and public code (Diamond 2023) | Different cloud/climate regime from Bangladesh | Strong method-replication benchmark |
| North Atlantic; Canadian wildfire smoke in 2023 | Distinct smoke transport events and extensive satellite coverage | Smoke may sit above clouds; event selection, synoptic weather and wet removal confound | Good later event study, less direct local relevance |

NASA documented haze over India and Bangladesh on [28 January 2025](https://modis.gsfc.nasa.gov/gallery/individual.php?db_date=2025-01-30) and [10 February 2025](https://modis.gsfc.nasa.gov/gallery/individual.php?db_date=2025-02-12). CAMS documented a [November 2024 regional pollution episode](https://atmosphere.copernicus.eu/cams-global-system-tracks-exceptional-air-pollution-episode-south-asia). These establish candidate exposure episodes, not aerosol effects on clouds. The [2025 Bangladesh Clean Air Project](https://www.worldbank.org/en/news/press-release/2025/06/18/world-bank-helps-bangladesh-improve-energy-security-air-quality) establishes policy relevance, not a realized emissions treatment suitable for immediate causal analysis.

The [IMO sulfur limit](https://www.imo.org/en/mediacentre/hottopics/pages/sulphur-2020.aspx) changed on 1 January 2020. [NASA's account of Canadian smoke reaching Europe](https://science.nasa.gov/earth/earth-observatory/canadian-smoke-reaches-europe-151507/) establishes that event's transport context.

Proposed mapping domain: **18–27°N, 85–94°E**, covering Bangladesh and surrounding transport pathways. Proposed ocean analysis box: **18–22°N, 87–92°E**, with an explicit land mask and coast-distance sensitivity. These are planning bounds, not an empirically optimized study area. Do not treat Bangladesh's political border as the boundary of its air mass.

## Technology and methods

The minimum viable observational stack is MODIS/Aqua cloud retrievals, ERA5 weather, one aerosol reanalysis, and an observed AOD product for sensitivity checks. See the [data catalog](data-catalog.csv) for product links, scales and limitations.

- **MODIS and VIIRS:** daytime cloud phase, optical thickness, effective radius, cloud top and cloud mask. Swath data retain QA and overpass time. VIIRS continuity products support an extension beyond the historical MODIS record; check release-specific phase corrections and cross-sensor differences.
- **AOD retrievals:** ocean Dark Target products for marine exposure and MAIAC over land. MAIAC is not an open-ocean aerosol product. AOD is not CCN, particle number or surface PM2.5.
- **CALIPSO/CALIOP and CloudSat archives:** aerosol/cloud layer geometry and cloud/rain profiles. Their narrow tracks and attenuation limit sample sizes. Science data collection ended in 2023; do not assume a 2024–2026 archive.
- **EarthCARE:** atmospheric high-spectral-resolution lidar, Doppler cloud radar, imager and broadband radiometer. Useful for vertical overlap, cloud structure and radiation consistency checks. Since 2024, with public products from 2025, it is a short-record extension, not a decadal trend substitute. Verify product release, version, flags and usable local overpasses before making it essential.
- **PACE OCI, SPEXone and HARP2:** hyperspectral/multi-angle polarimetric information on aerosol and droplet properties. Promising for aerosol type/size and cloud microphysical cross-checks. Algorithm status, product footprints and land/ocean support differ; exact regional coverage remains untested here.
- **INSAT-3D/3DR/3DS and Himawari:** high-frequency cloud evolution. INSAT viewing geometry is favorable for South Asia; confirm MOSDAC archive/access. Himawari can cover the region with more oblique geometry. Cloud-top cooling/rise rates are development proxies, not direct updraft observations.
- **ERA5:** hourly humidity, temperature, winds, boundary layer height, stability, SST and synoptic ascent. Reanalysis vertical motion is resolved large-scale ascent, not a cloud-core updraft.
- **MERRA-2 and CAMS EAC4:** complete-in-time modeled/assimilated aerosol fields, including species. They fill an exposure role when satellite AOD is cloud-masked but are not independent observations of cloud-base aerosol. Shared assimilated AOD limits independent validation.
- **CERES:** top-of-atmosphere shortwave/longwave flux and cloud radiative effect. Use SYN1deg for synoptic context and EBAF for monthly climate context. Avoid pretending a 1° radiation product resolves an individual kiln or cloud pixel.
- **GPM IMERG and DPR:** precipitation context and rain structure. IMERG is an estimate and not a drizzle detector for individual warm cloud pixels.
- **AERONET:** ground-based AOD/size information for exposure checks. Dhaka and Bhola have documented observations; current station identifiers, Level-2 quality data and overlaps must be audited.
- **FIRMS plus HYSPLIT:** fire timing and transport pathways; neither yields definitive chemical source attribution.
- **Statistical practice:** meteorological stratification/matching, generalized additive models, spatial/temporal blocking, missingness audits, multiscale sensitivity and event-study diagnostics. ML/SHAP can explain predictions but does not establish causality.

The newest methods are valuable because they improve vertical, temporal or microphysical specificity, not simply because their spatial resolution is higher.

## Field observations and models

Public **ACTIVATE (western North Atlantic, 2020–2022)** aircraft measurements connect aerosol, CCN, cloud microphysics and meteorology. **CAMP2Ex (Philippines, 2019)** is a useful tropical monsoon/convection comparator. **EPCAPE (California, 2023–2024)** provides ground-based aerosol, cloud and precipitation observations. They can help test a method or understand proxy failures without acquiring instruments, but their relationships must not be transferred to Bangladesh as established local physics.

Campaign sources: [ACTIVATE](https://www-air.larc.nasa.gov/missions/activate/index.html), [CAMP2Ex](https://impact.earthdata.nasa.gov/casei/campaign/CAMP2Ex/), [EPCAPE](https://csl.noaa.gov/projects/ages/epcape/).

Model hierarchy:
- HYSPLIT trajectories: feasible first modeling element; assess air-mass history.
- Existing CESM/CAM or CMIP6 output: feasible model evaluation after observations. AerChemMIP/RFMIP experiments such as piClim-aer and piClim-control help define aerosol ERF; variable availability differs by model.
- WRF-Chem: regional aerosol–meteorology simulations, but emissions, initialization, cloud physics and ensembles make a first independent project demanding.
- Large-eddy/cloud-resolving models, including SAM/UCLALES and newer storm-resolving systems: useful for mechanisms, normally a later collaborative step.
- A radiative-transfer package such as libRadtran can estimate conditional radiative sensitivities later; it cannot create missing anthropogenic attribution.

Do not infer an indirect aerosol effect simply by subtracting simulations with different microphysics configurations. [NCAR's WRF-Chem guidance](https://www2.acom.ucar.edu/sites/default/files/2025-07/WRF_CHEM_Best-Practices-2015.pdf) explicitly cautions against that comparison. See [CMIP experiment definitions](https://wcrp-cmip.github.io/CMIP6_CVs/docs/CMIP6_experiment_id.html).

## Candidate research designs

### 1. Weather-adjusted coastal outflow and liquid-cloud microphysics

**Question:** Within a single shallow-liquid-cloud regime, do effective radius, optical thickness and estimated droplet concentration differ with aerosol exposure after matching prior meteorological conditions?

**Data:** MYD06_L2/MYD03; MYD04_L2 ocean AOD; ERA5; MERRA-2 or CAMS; optional AERONET and IMERG. Land MAIAC is context, not marine AOD.

**Approach:** Audit December 2018–February 2019 and March–April 2019 separately; expand provisionally to 2010–2021 if coverage permits. Collocate at overpass time, separate land/ocean and winter/pre-monsoon, classify air masses, match humidity/stability/SST/winds and fit transparent nonlinear associations. Use lagged/upwind aerosol estimates as sensitivities. Assess both exposure and cloud retrieval missingness. Keep cloud fraction and liquid water as separate response analyses with different sample definitions.

**Difficulty:** Moderate; primarily remote sensing and statistics. A modest pilot should be feasible without HPC, but storage/runtime must be measured.

**Contribution:** A reproducible estimate of how much the inferred regional aerosol–cloud association changes with weather adjustment, sample selection and exposure proxy. A robust null would also be informative. Novelty is conditional on the detailed literature audit.

### 2. Does aerosol height change the inferred interaction?

**Question:** At comparable column aerosol load and meteorology, do cloud associations differ when aerosol is near cloud level versus elevated above low clouds?

**Data:** CALIOP aerosol profiles/layers and cloud layers; MODIS; ERA5; optional CloudSat precipitation flags. EarthCARE supplies a separate 2024–2026 validation/case-study epoch if usable data exist.

**Approach:** Start with track-based counts. Collocate nearby cloud observations with strict time/space windows; classify likely overlap using uncertainty intervals and retain an ambiguous category. Compare matched cases and sensitivity to altitude margins. Use MERRA-2/CAMS vertical structure as contextual model information, not an independent validation. Do not assume that a clear-air lidar profile beside an opaque cloud reveals the aerosol below that cloud.

**Difficulty:** Moderate to high because of sparse sampling, attenuation and multi-sensor geometry.

**Contribution:** A regional assessment of when column AOD is an unsuitable cloud-exposure proxy. Directly builds on Kant (2023) and Li (2026), so Bangladesh-specific robustness and process separation need to supply the added value.

### 3. Liquid-cloud response to shipping sulfur regulation

**Question:** Did liquid-cloud microphysics along a Bay of Bengal shipping corridor change relative to matched low-shipping regions after IMO2020, and does the contrast survive contamination and weather controls?

**Data:** MODIS/VIIRS cloud retrievals, ERA5, aerosol context, and independently validated shipping routes/activity or licensed AIS data. CERES only for a secondary regional radiation analysis. Lightning is optional and should not drive feasibility.

**Approach:** Multi-year before/after event study or difference-in-differences, with matched corridor-adjacent comparisons, wind-dependent transport, pre-trend checks and placebo dates/corridors. Handle 2020 separately and test 2015–2019 versus 2021–2023/2024, auditing orbit drift and product changes. The regulation was global: adjacent regions are lower-exposure comparators, not guaranteed untreated controls.

**Difficulty:** High relative to Design 1; exposure information and counterfactual validity are the bottlenecks.

**Contribution:** A liquid-cloud and sampling-robustness extension to existing Bay shipping/lightning studies. Simply repeating a pre/post comparison would be insufficient.

## Open questions a new study could address

1. Does a bulk AOD–cloud relation survive weather matching and stricter cloud-edge filtering?
2. Do aerosol–cloud associations change when the aerosol is placed near cloud level rather than inferred from total-column AOD?
3. Are winter and pre-monsoon differences attributable to comparable cloud regimes, or just to changing regime occurrence?
4. How much does clear-sky AOD availability select the analyzed cloud sample?
5. Does a signal persist across exposure products and spatial scales without mistaking shared assimilation for independence?
6. Can temporal/transport information reduce reverse causality from precipitation scavenging?
7. Which signatures are consistent with droplet activation versus stability/heating adjustments, and which remain observationally indistinguishable?

These are candidate gaps in a targeted search, not claims that no one has addressed them anywhere.

## Journals and conferences

Monitor **Atmospheric Chemistry and Physics, Journal of Geophysical Research: Atmospheres, Geophysical Research Letters, Atmospheric Measurement Techniques, Atmospheric Research, Journal of the Atmospheric Sciences, and Journal of Climate**. Add **Remote Sensing of Environment** for retrieval/spatial methods; **Nature Geoscience, Nature Climate Change, npj Climate and Atmospheric Science, Communications Earth & Environment, and Reviews of Geophysics** for broader results and synthesis.

Monitor **EGU General Assembly Atmospheric Sciences**, **AGU Annual Meeting Atmospheric Sciences**, **AMS Annual Meeting and cloud-physics/atmospheric-chemistry conferences**, the **IAMAS International Conference on Clouds and Precipitation**, and aerosol-focused **AAAR/European Aerosol Conference/International Aerosol Conference** programs. Use official societies' sites for schedules and calls; conferences with similar names are not necessarily the same event.

Start with citation alerts for Kant (2023), Li (2026), Goren (2025), and Varble (2023), plus searches for "Bay of Bengal aerosol cloud meteorology" and "satellite aerosol cloud causal sampling".

## Limits and next decision

The survey verifies identifiable publications and official product documentation but does not certify every full-text interpretation, current download service, station record or regional data overlap. Read scopes are recorded. No data were acquired or analyzed in this planning session.

The immediate decision is which candidate to pilot. Recommended next artifact: a **data availability and quality-control report**, then a diagnostic presentation of actual pilot findings. Manuscript preparation remains deferred.
