# Urban hydroclimate: bibliographic and numerical verification notes

## Scope and bibliographic audit

The six requested DOI records match the stated first-author surnames and years. Title, first author, year and DOI were checked against the published articles, exact-DOI Crossref records, and OpenAlex DOI records. The Crossref science-database search treated DOI strings as general search queries and returned unrelated hits, so exact DOI records were retrieved directly from the Crossref API instead. No title/DOI mismatch was found. All six primary-source links in Sources returned article content; Du’s is the author-hosted full paper. No underlying draft was supplied, so the warnings below identify potential misstatements rather than changes to an existing draft.

## Xiong et al. (2025)

**Jinghua Xiong et al., “Asymmetric shifts in precipitation due to urbanization across global cities,” Nature Communications 16, 5802 (2025).** The study uses hourly satellite-based precipitation for 741 cities, contrasting urban and rural climatologies over 2001–2023. Across the sample, 63% of cities showed higher total urban precipitation and 37% lower; only 21% and 8%, respectively, showed statistically significant increases or decreases. These are shares of cities, not percentage changes in rainfall. The overall pattern is increased lower-intensity and decreased higher-intensity precipitation, with geographic exceptions; it is not an increase in heavy rainfall in every city. Hourly categories are drizzle 0.1–0.5, light 0.5–2.5, moderate 2.5–10, and heavy ≥10 mm/hour. [1]

## Guccione et al. (2026): Europe clarification

**Alice Guccione et al., “Extreme precipitation changes in relation to urbanization,” npj Natural Hazards 3, 10 (2026).** In the global station analysis, 6,028 selected GHCN-Daily stations are examined over 1962–2021, with station-specific extreme events defined as each station’s 60 most intense daily precipitation events. The estimated increase in event frequency across the period is 29% for urban stations and 19% for rural stations: these are relative changes over the full period, not annual rates, rainfall intensity changes, or Europe-only results. The station distribution is geographically uneven and the authors cannot rule out regional confounding. [2]

**Europe and Mediterranean are a separate modeled analysis, not the station result.** CHAPTER is a WRF dynamical downscaling of ERA5, with 3 km × 3 km grid cells, over part of Europe and the Mediterranean, 1981–2022. Defining extremes as each grid point’s 42 highest daily precipitation events, the reported urban and rural frequency increases over the 42-year period are **17.8% and 6.5%**, respectively. The paper reports the difference as statistically significant; the rural trend alone did not pass its 95% significance test. The figure caption rounds these to approximately 18% and 6%, respectively. They are not millimeters, annual rates, changes in mean rainfall, or direct gauge observations. Spatial heterogeneity and correlated neighboring grid cells remain limitations; a causal attribution to urbanization alone is not established by the contrast. [2]

## Du et al. (2023)

**Huilin Du et al., “Contrasting Trends and Drivers of Global Surface and Canopy Urban Heat Islands,” Geophysical Research Letters 50, e2023GL104661 (2023).** This is a heat-island paper, not a precipitation study. For 5,643 cities during 2003–2020, global mean daytime surface urban–rural temperature-contrast trend was 0.19 ± 0.006 °C/decade versus 0.03 ± 0.002 °C/decade for canopy air temperature; nighttime figures were 0.06 ± 0.004 and 0.03 ± 0.002 °C/decade, respectively. Errors are standard errors. These are trends in urban–rural contrasts, not the magnitude of the heat island or total urban warming. The canopy surface air temperatures are spatially continuous estimates, not direct station measurements everywhere. [3]

## Hao et al. (2023)

**Lu Hao et al., “Urbanization alters atmospheric dryness through land evapotranspiration,” npj Climate and Atmospheric Science 6, 149 (2023).** Of 25 large urban agglomerations, 17 exhibited urban dry islands and 8 urban wet islands. In humid vegetated regions the paper reports urban–rural differences in annual evapotranspiration as high as 215 mm per year; this is an annual water-depth difference, not a daily amount, precipitation change, or universal city average. Wet islands are associated in this sample with arid or dry-summer climates; the result does not mean every city is drier than its surroundings. [4]

## Yang et al. (2024)

**Long Yang et al., “Urban development pattern’s influence on extreme rainfall occurrences,” Nature Communications 15, 3997 (2024).** The study examines 1,790 inland cities without notable complex terrain or land–water boundaries and urban development in 2003–2018. Compact development is associated with larger increases in extreme-rainfall frequency downtown than in surrounding rural areas; dispersed development shows weaker urban–rural contrasts. The daily extreme definition in the relevant composite is rainfall exceeding the 99th percentile of rainy-day daily rainfall. A weak urban–rural contrast does not mean neither urban nor rural locations experience risk or increases; the study explicitly discusses extended exposure in dispersed developments. [5]

## Liu and Niyogi (2019) review

**Jie Liu and Dev Niyogi, “Meta-analysis of urbanization impact on rainfall modification,” Scientific Reports 9, 7301 (2019).** The quantitative meta-analysis used 85 studies drawn from 48 papers, not 85 independent papers. It reports mean precipitation enhancements of 18% downwind and 16% over cities, with enhancement approximately 20–50 km from city centers in the abstract. These are pooled results across selected studies, not an estimate that applies to every city or solely to extremes. The paper also distinguishes results from case studies and climatological studies. [6]

## Sources

[1] Xiong et al. (2025), published article: https://www.nature.com/articles/s41467-025-61053-0

[2] Guccione et al. (2026), published article, Results and Discussion: https://www.nature.com/articles/s44304-026-00173-z

[3] Du et al. (2023), author-hosted published paper: https://tc25.github.io/Papers/GRL_2023b.pdf — DOI: 10.1029/2023GL104661.

[4] Hao et al. (2023), published article: https://www.nature.com/articles/s41612-023-00479-z

[5] Yang et al. (2024), published article: https://www.nature.com/articles/s41467-024-48533-5

[6] Liu and Niyogi (2019), published article: https://www.nature.com/articles/s41598-019-42494-2
