# Urbanisation and hydroclimate: research notes

## Coverage status
- **Done:** global multidecadal flood-extent and rainfall studies, physical runoff and recharge mechanisms, methods and confounding. Primary papers [1–3], review [4] and official technical source [5] directly inspected; DOI strings for [1–4] checked on publication/PMC pages.
- **Needs follow-up:** robust global multi-decadal *causal* estimates of urban-driven runoff, infiltration or recharge, and regional gauged-catchment effect sizes. A potentially useful US study (https://doi.org/10.1029/2021WR030742) was found but its full text and reported numerical estimates were not independently checked; do not quote its search-result figures as verified.
- **Interpretation:** the studies measure different endpoints, sampling frames and temporal/spatial scales. No single global percentage describes urbanisation’s effect on flooding, recharge or rainfall.

## Evidence table

| # | Source | URL | Key claim | Type | Confidence |
|---|---|---|---|---|---|
| 1 | Mazzoleni et al. (2022), *Deciphering human influence on annual maximum flood extent at the global level* | https://doi.org/10.1038/s43247-022-00598-0 | 106 large basins, 1985–2018; rainfall and urban area selected as main explanatory variables in 57% | Primary observational | High for reported statistic; low–medium for causal attribution |
| 2 | *Global scale assessment of urban precipitation anomalies* (2024) | https://doi.org/10.1073/pnas.2311496121 | 63% of 1,056 cities have positive annual urban–rural precipitation contrast, 2001–2020 | Primary satellite observational | High for reported contrast, not causation |
| 3 | *Asymmetric shifts in precipitation due to urbanization across global cities* (2025) | https://doi.org/10.1038/s41467-025-61053-0 | 741 cities, 2001–2023; positive total-precipitation urban–rural contrast in 63%, statistically significant increases in 21% | Primary satellite observational | High for reported statistic; lower for causal wording |
| 4 | La Vigna (2022), *Urban groundwater issues and resource management* | https://doi.org/10.1007/s10040-022-02517-1 | Urban groundwater depends on natural and human water pathways; leakage recharge and abstraction need monitoring | Scholarly review | High for context-dependent mechanisms |
| 5 | US EPA, *Urbanization – Hydrology* | https://www.epa.gov/caddis/urbanization-hydrology | Imperviousness and drainage alter infiltration, runoff delivery and streamflow | Government technical overview | High for qualitative mechanism |

## Findings

### Runoff, infiltration, flood response and groundwater
Impervious cover reduces rainfall infiltration at the paved surface, while stormwater conveyance can route water quickly to channels, raising runoff and modifying hydrograph timing and peaks [5]. This is not a universal proportional relationship: connected impervious area, drainage engineering, soil, antecedent moisture and rainfall severity matter. **Inference:** one should distinguish local excess rainfall, runoff volume, streamflow peak, floodwater extent and damage; a change in one is not a numeric estimate of another [1,5].

Recharge is not synonymous with infiltration and cannot safely be assumed always to fall with urbanisation. Paving reduces direct natural recharge, while water-supply and sewer leakage and managed infiltration can supply recharge; groundwater abstraction and drainage affect groundwater levels independently of recharge [4,5]. Tracers and water budgets, groundwater-level and aquifer monitoring, and supply/sewer inventories help distinguish sources and storage changes [4]. A global numerical effect on net recharge was not verified.

### Global flood extent: large basins, not individual storm peaks
Mazzoleni et al. [1] use Landsat-derived seasonal water presence as a proxy for annual maximum flood extent (AMFE), urban area as a human-activity proxy, and hydroclimatic variables in statistical analyses across 106 selected basins during 1985–2018. Rainfall plus urban area were the main explanatory variables in **57% of basins**, not a 57% increase in flooding. Authors report adding urban area increased adjusted R² by *up to* 71% and reduced RMSE by *up to* 30%; these are model-performance changes, not physical flood effect sizes. The 8- or 16-day satellite revisit can miss short floods; large-basin aggregation, omitted deforestation/agriculture and climate patterns, and concurrent urban growth limit causal interpretation. Floodplain water presence is neither direct peak discharge nor exposed population or loss [1].

### Urban land–atmosphere effects and precipitation
The 2024 global analysis [2] compares city and surrounding rural rainfall with 0.1° satellite estimates in **1,056 cities, 2001–2020**. **63%** have wetter urban areas on annual totals; this is the fraction with a positive spatial contrast, not an average rainfall increase or fraction statistically significant. Seventeen cities exceeded +200 mm/year (8.3–85.3%), while 12 were below −200 mm/year (−15.8 to −9.7%); examples are tails, not global averages [2]. Fixed 2020 urban boundaries and topographic/coastal gradients mean this is primarily a spatial contrast, not a measured before–after effect of urban growth [2].

The independent 2025 global comparison [3] uses 741 cities and 2001–2023 satellite data: **63%** had a positive total precipitation contrast, but only **21%** showed statistically significant increases and **8%** significant decreases. It uses hourly intensity classes and finds responses differ with intensity. The two 63% figures come from related designs and satellite products; they are not independent experimental replications and do not establish that urbanisation caused a 63% increase. City size selection, coarse pixels, rural reference selection, mountains, coasts, spatial spillovers and heavy-rain satellite underestimation can bias contrasts [2,3].

Plausible pathways include urban sensible heat and heat-island circulation, altered surface roughness and convergence, reduced evapotranspiration/moisture supply, and aerosol–cloud interactions [3,5]. These mechanisms can reinforce or oppose one another; spatial rainfall association alone does not isolate their individual contributions [3]. **Inference:** urban effects on precipitation can interact with direct drainage and imperviousness effects on flooding, but rainfall anomalies must not be added mechanically to runoff or flood-extent estimates [1–3,5].

### Attribution designs and confounders
- Use meteorological controls (rainfall intensity and timing, temperature, snowmelt, antecedent moisture), plus time-varying imperviousness and drainage, dams, land use, pumping, wastewater and management; climate and urban development co-trend [1,4,5].
- **Inference:** matched or paired catchments and before–after designs, city fixed effects or difference-in-differences with pre-trend checks, and physically based counterfactual simulations can strengthen attribution; each requires comparable controls, consistent measurement and checks for concurrent interventions. Combine gauge, radar, remote-sensing and groundwater observations; account for spatial scale, missing short-duration extremes and boundary sensitivity [1–4].
- Report water quantity and quality separately, and runoff/flood hazard separately from exposure and vulnerability; global satellite studies leave the local extremes and causal pathways uncertain [1,4].

## Sources
1. Mazzoleni et al., *Deciphering human influence on annual maximum flood extent at the global level* — https://doi.org/10.1038/s43247-022-00598-0
2. *Global scale assessment of urban precipitation anomalies* — https://pmc.ncbi.nlm.nih.gov/articles/PMC11420207/ ; DOI https://doi.org/10.1073/pnas.2311496121
3. *Asymmetric shifts in precipitation due to urbanization across global cities* — https://doi.org/10.1038/s41467-025-61053-0
4. La Vigna, *Review: Urban groundwater issues and resource management, and their roles in the resilience of cities* — https://doi.org/10.1007/s10040-022-02517-1
5. US EPA, *Urbanization – Hydrology* — https://www.epa.gov/caddis/urbanization-hydrology
