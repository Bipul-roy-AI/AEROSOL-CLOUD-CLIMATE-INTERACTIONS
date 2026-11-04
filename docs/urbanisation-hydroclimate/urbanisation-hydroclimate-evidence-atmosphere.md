# Urbanization and atmospheric hydroclimate: research notes

## Evidence table

| # | Source | Direct URL | Key claim and context | Type | Confidence |
|---|---|---|---|---|---|
| 1 | Changnon, Semonin & Huff (1976), *A Hypothesis for Urban Rainfall Anomalies* | https://doi.org/10.1175/1520-0450%281976%29015%3C0544%3AAHFURA%3E2.0.CO%3B2 | Foundational journal study identified and DOI/title/authors checked with Crossref; primary abstract was inaccessible. No numerical conclusion extracted. | Primary, metadata only | Medium |
| 2 | Sui et al. (2024), *Global scale assessment of urban precipitation anomalies*, PNAS | https://doi.org/10.1073/pnas.2311496121 | >1,000 cities; >60% of cities and downwind areas wetter than surrounding rural areas; urban wet-island magnitude nearly doubled over 20 years. | Primary, abstract directly read via PubMed https://pubmed.ncbi.nlm.nih.gov/39250669/ | High |
| 3 | Xiong et al. (2025), *Asymmetric shifts in precipitation due to urbanization across global cities*, Nature Communications | https://doi.org/10.1038/s41467-025-61053-0 | 741 cities, 2001–2023; 63% show positive total precipitation contrast; only 21% significant increases, 8% significant decreases. | Primary, abstract and full-text results directly read | High |
| 4 | *Extreme precipitation changes in relation to urbanization* (2026), npj Natural Hazards | https://doi.org/10.1038/s44304-026-00173-z | 6,028 gauges, 1962–2021; extreme-event frequency increases 29% at urban vs 19% at rural stations. | Primary, full-text results directly read | High |
| 5 | Shen & Zhao (2024), *Intensifying urban imprint on land surface warming*, iScience | https://doi.org/10.1016/j.isci.2024.109110 | 536 cities, satellite surface urban heat-island daily mean 0.99–1.10°C, 2003–2018; urban latent heat flux lower in 91.6% of cities. | Primary, abstract/summary and results directly read | High |
| 6 | Hao et al. (2023), *Urbanization alters atmospheric dryness through land evapotranspiration*, npj Climate and Atmospheric Science | https://doi.org/10.1038/s41612-023-00479-z | Of 20 urban flux sites, 19 had lower remotely estimated ET than nearby nonurban areas; mean annual difference about 215 mm. | Primary, full-text methods/results directly read | High |
| 7 | Mazrooei et al. (2021), *Urbanization impacts on evapotranspiration across various spatio-temporal scales*, Earth's Future | https://doi.org/10.1029/2021EF002045 | Identified relevant primary ET study; bibliographic metadata verified with Crossref, primary abstract inaccessible. No numerical conclusion extracted. | Primary, metadata only | Medium |

## Findings and critical interpretation

### Precipitation — done

- The global PNAS study reports urban and downwind rainfall greater than rural rainfall for a majority of >1,000 cities, and a near doubling of urban wet-island intensity over two decades [2]. The doubled quantity is the *urban–rural anomaly*, not total precipitation, and its abstract does not identify a universal city-level effect size. Associations of enhancement with heat, aerosol loading, population and humid climates are not independent causal identification [2].
- Xiong et al. compare paired urban/rural climatologies from hourly satellite precipitation for 741 cities over 2001–2023 [3]. The 63% positive contrasts include nonsignificant cities; 21% are significantly positive and 8% significantly negative. The abstract reports lower-intensity precipitation increases, higher-intensity decreases, and distinct tropical monsoon behavior; lower-intensity gains are most evident early morning and higher-intensity decreases late afternoon [3]. These are climatological urban–rural contrasts across 23 years, **not** an estimated 23-year trend. Satellite retrieval and rural pairing can influence results; effects on rare extremes must not be generalized to every city or timescale.
- The 2026 global gauge analysis provides a longer record [4]. Its extreme threshold is the 60 highest daily rainfall observations in each 60-year record, roughly one event per year; it reports 29% versus 19% increases in event *frequency*, not 29% versus 19% changes in rainfall depth. Urban/rural classification is principally based on 2015 settlement conditions; urban–rural trend differences may reflect geography and station selection as well as urbanization, so 10 percentage points is not a clean causal estimate. It does not establish that global average extreme rainfall fell, nor does it directly contradict the different hourly/intensity contrasts in [3].
- The historical 1976 study is a bibliographically verified foundational lead [1]; its primary abstract could not be fetched, so its results and proposed mechanisms remain unverified here.

### Temperature and ET — done with limitations

- Shen & Zhao [5] use satellite-derived land-surface temperature over 536 cities, 2003–2018. Their annual daily mean surface urban heat-island intensity rises from 0.99°C to 1.10°C; this is an urban–rural *surface-temperature* contrast, not air temperature, a global mean temperature trend, or urbanization's contribution to greenhouse warming. Their calculated urban minus rural annual latent heat flux is negative for 91.6% of cities, mean −7.70 W m⁻²; remote-sensing and energy-balance attribution are not direct causal experiments [5].
- Hao et al. [6] examine urban moisture, energy flux and ET with multiple datasets. Their reported mean 215 mm/year difference is the mean urban–nonurban ET difference for **20 flux-site locations**, not 25 urban agglomerations nor the global average; 19 sites have less urban ET. Flux data cover 2003–2020; urban towers were compared with surrounding ERA5 grid cells for paired rural meteorology, and ET was independently remote-sensing-derived. Correlations between ET contrast and humidity/temperature contrasts support a mechanism, but cannot uniquely establish causality. A separate 580-station China analysis spans 1980–2018 and five agglomerations; it should not be represented as globally distributed [6].
- Mazrooei et al. [7] is a directly verified bibliographic lead on cross-scale ET, but access to its primary abstract failed; do not reuse numerical results without checking.

### Humidity and synthesis — done with limitations

- Specific humidity (actual water vapor), relative humidity, and vapor-pressure deficit (which also responds to air temperature) are different metrics; a drier relative atmosphere does not automatically mean a decline in actual water vapor. Hao et al. distinguish q, VPD and air temperature and consider both urban dry and wet islands [6]. Urban ET suppression and warming are plausible linked mechanisms, but sign and magnitude are climate- and site-dependent; no uniform global multiplier is warranted [5, 6].
- **Inference across studies:** atmospheric urbanization responses are neither spatially nor temporally uniform. Rainfall intensity class, timing and spatial comparison matter, as do the distinction between air and surface temperature and between moisture content and atmospheric demand [2–6]. Urban/rural contrasts and correlations should not be treated as randomized land-conversion effects.

## Coverage status

- Directly checked: abstracts [2,3,5] and primary results/methods [3–6]; long-record precipitation [4] and local multi-decadal moisture [6].
- Foundational precipitation [1] and primary ET study [7] DOI metadata checked through Crossref, but abstracts blocked; no findings attributed to them. DOI identity verified via PubMed/Crossref or matching publisher article identifier; automated HTTP DOI access for [1,7] returned 406, so resolution was not independently confirmed by browser.
- Remaining gap: a foundational primary heat-island or humidity paper with accessible abstract; no definitive globally representative multi-decade ET trend established. The 2026 article abstract was not exposed by the page extractor; numerical values were checked in the primary article's results instead.

## Sources

1. Changnon, Semonin & Huff, *A Hypothesis for Urban Rainfall Anomalies* — https://doi.org/10.1175/1520-0450%281976%29015%3C0544%3AAHFURA%3E2.0.CO%3B2
2. Sui et al., *Global scale assessment of urban precipitation anomalies* — https://doi.org/10.1073/pnas.2311496121
3. Xiong et al., *Asymmetric shifts in precipitation due to urbanization across global cities* — https://doi.org/10.1038/s41467-025-61053-0
4. *Extreme precipitation changes in relation to urbanization* — https://doi.org/10.1038/s44304-026-00173-z
5. Shen & Zhao, *Intensifying urban imprint on land surface warming* — https://doi.org/10.1016/j.isci.2024.109110
6. Hao et al., *Urbanization alters atmospheric dryness through land evapotranspiration* — https://doi.org/10.1038/s41612-023-00479-z
7. Mazrooei et al., *Urbanization impacts on evapotranspiration across various spatio-temporal scales* — https://doi.org/10.1029/2021EF002045
