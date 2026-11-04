# Urbanisation and hydroclimate: attribution methods and global evidence

Research cutoff: 4 November 2026. Evidence is selected, not an exhaustive systematic review. Confidence refers to accuracy of reporting the source, not proof of a causal effect.

## Evidence table

| # | Source and date | Direct URL / DOI | Key claim checked | Type | Confidence |
|---|---|---|---|---|---|
| 1 | Lalonde, Oudin & Bastin, 2023, *Urban Climate* | https://doi.org/10.1016/j.uclim.2023.101605 | 174 experiments from 48 articles; results sensitive to data type; radar studies did not reach consensus | Review, abstract inspected at https://ludovicoudin.github.io/publications/2023_Urban_Climate_Lalonde_Oudin.html | High |
| 2 | Liu & Niyogi, 2019, *Scientific Reports* | https://doi.org/10.1038/s41598-019-42494-2 | 85 studies from 48 papers quantitatively synthesized; mean changes 18% downwind and 16% over city | Meta-analysis, full text https://pmc.ncbi.nlm.nih.gov/articles/PMC6514167/ | High |
| 3 | Sui et al., 2024, *PNAS* | https://doi.org/10.1073/pnas.2311496121 | Of 1,056 cities, 63% had higher annual precipitation than peripheral rural areas; topography matters | Primary observational, full text https://pmc.ncbi.nlm.nih.gov/articles/PMC11420207/ | High |
| 4 | Xiong et al., 2025, *Nature Communications* | https://doi.org/10.1038/s41467-025-61053-0 | IMERG urban–rural contrasts across 741 large cities, 2001–2023, differ by intensity; heavy-rain satellite underestimation and reference definition matter | Primary observational, full text https://www.nature.com/articles/s41467-025-61053-0 | High |
| 5 | Guccione et al., 2026, *npj Natural Hazards* | https://doi.org/10.1038/s44304-026-00173-z | Global gauge and European/Mediterranean regional-model analysis clusters daily extreme precipitation trends by urbanization | Primary observational/model analysis, full text https://www.nature.com/articles/s44304-026-00173-z | High |
| 6 | Qian et al., 2022, *Advances in Atmospheric Sciences* | https://doi.org/10.1007/s00376-021-1371-9 | Reviews observational and modelling methods, and >500 studies of urban regional climate, moisture, storms and extremes | Review, abstract inspected https://www.pnnl.gov/publications/urbanization-impact-regional-climate-and-extreme-weather-current-understanding | High |
| 7 | Fletcher et al., 2024, *Nature Reviews Earth & Environment* | https://doi.org/10.1038/s43017-024-00599-x | Reviews urban runoff, stormwater transformation and downstream implications | Review, abstract inspected https://www.usgs.gov/publications/concepts-and-evolution-urban-hydrology | High |
| 8 | Widespread global exacerbation of extreme drought induced by urbanization, 2024, *Nature Cities* | https://doi.org/10.1038/s44284-024-00102-z | Study exists and addresses urbanisation and drought; detailed numerical findings not independently checked from primary article body | Primary, https://www.nature.com/articles/s44284-024-00102-z | Medium |

## Findings and interpretation

### What can and cannot be attributed

- Distinguish **precipitation generation** (rainfall amount, timing, extremes, spatial shift), **catchment response** (infiltration, drainage, runoff and flood extent), and **human risk** (exposure and vulnerability). A changing flood is not evidence by itself that cities changed rainfall. This distinction is an inference from the different atmospheric and hydrological processes reviewed in [6,7].
- City effects can operate through heat, aerodynamic roughness, moisture and aerosol–cloud pathways; mechanisms can interact with storm regime, coast and terrain [1,3,4,6]. Spatial rainfall contrasts do not isolate these mechanisms or exclude pre-existing geographical differences [3,4].
- Study definitions differ: local annual means, distributional intensity classes, daily extreme frequency, and storm-event rainfall are distinct estimands. The meta-analysis [2] is not a universal effect size; the large-city global spatial contrasts [3,4] are not estimates for every city or a controlled before/after intervention.

### Attribution designs

1. **Spatial urban–rural contrasts.** Compare city, upwind and downwind zones and multiple rural rings, stratifying by storm direction and terrain. In [3], the outermost rural ring is explicitly assumed free from city influence; the 2020 land-cover map is applied retrospectively to the 2001–2020 rainfall period. That spatial design cannot itself establish a change caused by historical urban growth. Coast, mountains, wind exposure and rural spillover threaten the control assumption [3].
2. **Longitudinal difference-in-differences or matched controls (recommendation/inference).** Combine dated urban expansion and consistent observations with matched non-urban areas; inspect pre-trends, changing station exposure and instruments, and alternative controls. Report the assumptions, including no confounding time-varying drivers and minimal interference, rather than labeling every differential trend causal. Compare synoptic conditions and natural variability. This is a proposed extension to the observational designs in [3–5], not a claim those papers implement a particular causal estimator.
3. **Paired numerical counterfactuals.** Compare otherwise matched simulations with urban and plausible preurban land cover under the same meteorological forcing; perturb urban heat, roughness, vegetation and aerosols individually and in combinations. Report choice of counterfactual vegetation, uncertainty, internal weather variability, and observational skill. Such model-based differences are conditional on model structure and do not independently prove the historical effect; simulation and observational methods are reviewed in [6].
4. **Factorial hydroclimate and hydrology scenarios (recommendation/inference).** Cross urban/nonurban land surface with historical/altered climate forcing, then force a validated runoff/flood model with each rain field and each drainage/land-use configuration. This separates atmospheric and runoff pathways and their interaction, conditional on assumptions; exposure and damage remain separate outcomes [6,7].
5. **Triangulation and uncertainty.** Use gauges, radar and satellite products where possible, account for effective resolution, sample the same locations before comparing instruments, and examine intensity thresholds and duration. Radar findings differ across reviewed experiments [1]; [3] reports greater IMERG–Stage IV differences for extremes than annual anomalies, and [4] notes underestimated heavy precipitation and sparse rural gauge sampling. Station relocations and multiple comparisons warrant explicit checks (recommendation).

### Global and recent evidence

- **Global/continents:** [3] finds 63% positive urban annual precipitation contrast across 1,056 cities, with 9 of 17 cities with anomalies above 200 mm/year in Africa. Kuala Lumpur's contrast is +247 mm/year, while negative contrasts include Jakarta and Himeji–Osaka–Kyoto; authors identify complex coastal and mountain terrain as important. These examples are observed contrasts, not isolated urban causal effects [3].
- **Diverse intensities:** [4] compares total, drizzle, light, moderate and heavy precipitation across 741 cities. Urban and rural boundaries and selection of cities larger than 100 km² limit transfer to small cities. In Shanghai, low-intensity contrasts varied from 7.7% for gauge-colocated satellite cells and 6.5% for gauges to 1.7% using all satellite cells; only three rural gauges were available [4].
- **Recent extreme-rainfall trends:** [5], published February 2026, compares changes in daily extremes according to urbanization metrics using global stations and a regional-model analysis. This is not a randomized urbanization intervention; interpret partitioning of urbanization versus background warming in light of observational and model assumptions [5].
- **Drought:** [8] is directly relevant but the available page extraction returned references rather than the article's results; precise estimates, drought metric and causal identification need direct verification before use. Meteorological drought, water supply shortfall and flood response must not be conflated (inference based on [6–8]).
- **Research synthesis:** The rainfall literature reviewed by [1] is sensitive to sensor and method. The earlier pooled 18% downwind enhancement [2] should be reported with the studied literature's selection and design limitations, not as an effect expected in each world city.

## Coverage status

- **Done:** directly checked two reviews, a meta-analysis, two global city studies, a 2026 paper and a hydrology review; DOIs checked against article pages, citations or publisher-linked source pages. Broad web and scholarly searches performed; the academic database identified [2].
- **Needs follow-up:** systematic, region-balanced evidence for African, Latin American and South Asian individual cities; drought article's study design and exact outcomes; more late-2026 papers and detailed model counterfactual case studies. Searches to 4 November cannot cover subsequent November publications. The 2026 Leeds flood article was inaccessible (403), and is deliberately not used for a numerical claim. AlphaXiv login unavailable.
- **Residual risk:** journal site extraction for some articles began in the body rather than abstract; findings above are restricted to directly inspected sections. Global city products may reflect regional sampling and instrument bias; no global generalisation about unobserved small cities is warranted.

## Sources

1. Lalonde, Oudin & Bastin, *Urban effects on precipitation* — https://doi.org/10.1016/j.uclim.2023.101605
2. Liu & Niyogi, *Meta-analysis of urbanization impact on rainfall modification* — https://doi.org/10.1038/s41598-019-42494-2
3. Sui et al., *Global scale assessment of urban precipitation anomalies* — https://doi.org/10.1073/pnas.2311496121
4. Xiong et al., *Asymmetric shifts in precipitation due to urbanization across global cities* — https://doi.org/10.1038/s41467-025-61053-0
5. Guccione et al., *Extreme precipitation changes in relation to urbanization* — https://doi.org/10.1038/s44304-026-00173-z
6. Qian et al., *Urbanization impact on regional climate and extreme weather* — https://doi.org/10.1007/s00376-021-1371-9
7. Fletcher et al., *Concepts and evolution of urban hydrology* — https://doi.org/10.1038/s43017-024-00599-x
8. *Widespread global exacerbation of extreme drought induced by urbanization* — https://doi.org/10.1038/s44284-024-00102-z
