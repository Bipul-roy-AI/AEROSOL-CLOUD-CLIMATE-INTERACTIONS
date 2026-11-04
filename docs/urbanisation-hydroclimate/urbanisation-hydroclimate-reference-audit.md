# Reference audit: urbanisation–hydroclimate review

## Scope and method

Audited all 15 cited URLs and bibliographic entries in `/workspace/outputs/urbanisation-hydroclimate.md`, and checked the specific uses of references 6, 7, 11, 13 and 15. No changes were made to that review. Exact-DOI Crossref `/works/{DOI}` API records were retrieved for all 14 papers (including the DOI discovered from the publisher for reference 6); publisher pages were read for references 6, 7, 13 and 15, and the EPA page for 14. Crossref requests initially returned HTTP 429 for 2, 9 and 10; sequential exact-DOI retries succeeded. The DOI links were separately requested using `fetch_content`.

**Important access limitation:** all 13 listed `doi.org` URLs returned HTTP 406 in this fetching environment. That is a blocked/content-negotiation result, **not evidence of dead or wrong DOIs**. All 13 corresponding exact DOI records exist in Crossref; the direct publisher pages for 7, 13 and 15 also loaded. Reference 6's MDPI page and 14's EPA page loaded. Reference 11's attempted AMS publisher page returned HTTP 403; the Crossref record and independent indexed abstract support identification. This audit did not complete a second independent scholarly-index check of every paper; exact Crossref and publisher checks should not be misrepresented as two-index validation.

## Bibliographic and URL audit

Crossref exact-record URLs are obtained by appending the displayed DOI to `https://api.crossref.org/works/`, URL-encoding the DOI where needed. ‘Matches’ means the listed author names, publication year and title agree with that exact record; it does not imply a full-text check of all claims. DOI-link access for each row is subject to the HTTP 406 qualification above.

| Ref. | Exact DOI / listed URL | Bibliography finding | Link result and action |
|---|---|---|---|
| 1 | 10.1073/pnas.2311496121 | Sui, Yang, Shepherd and Niyogi, 2024, title, PNAS 121 e2311496121 match. | DOI request 406; exact Crossref record exists. |
| 2 | 10.1038/s41467-025-61053-0 | Xiong, Yang, Yang and Yang, 2025 and title match; article 5802. | DOI request 406; Crossref exact record exists after retry. |
| 3 | 10.1038/s44304-026-00173-z | Guccione, Bassi, Desbiolles et al., 2026 and title match; volume 3 article 10. | DOI request 406; Crossref record exists. |
| 4 | 10.1029/2023GL104661 | Du et al., 2023 and title match; volume 50 e2023GL104661. Case of DOI immaterial. | DOI request 406; Crossref record exists. |
| 5 | 10.1038/s41612-023-00479-z | Hao, Sun, Huang et al., 2023 and title match; volume 6 article 149. | DOI request 406; Crossref record exists. |
| 6 | https://www.mdpi.com/2073-4441/2/3/605; DOI 10.3390/w2030605 | Title, 2010, *Water* 2, 605–648 match; **authors omitted**. Add O’Driscoll, M., Clinton, S., Jefferson, A., Manda, A. & McMillan, S. | Listed MDPI page loaded and contains article. |
| 7 | 10.1038/s43247-022-00598-0 | Mazzoleni et al., 2022 and title match. Can add volume 3, article 262. | DOI request 406; direct [Nature page](https://www.nature.com/articles/s43247-022-00598-0) loaded. |
| 8 | 10.1007/s10040-022-02517-1 | La Vigna, 2022 and English title match. Can add volume 30, 1657–1683. | DOI request 406; Crossref record exists. |
| 9 | 10.1038/s41598-019-42494-2 | Liu and Niyogi, 2019 and title match; article 7301. | DOI request 406; Crossref exact record exists after retry. |
| 10 | 10.1016/0004-6981(73)90140-6 | Oke, 1973 and title match; volume 7, 769–779. Crossref calls journal *Atmospheric Environment (1967)*. | DOI request 406; Crossref exact record exists after retry. |
| 11 | 10.1175/1520-0450(1976)015<0544:AHFURA>2.0.CO;2 | Changnon, Semonin and Huff, 1976 and title match; add volume 15, 544–560. The percent-encoded URL in the review represents this DOI. | DOI request 406; [attempted AMS page](https://journals.ametsoc.org/view/journals/apme/15/6/1520-0450_1976_015_0544_ahfura_2_0_co_2.xml) 403; Crossref record exists. |
| 12 | 10.1038/s41467-024-48533-5 | Yang et al., 2024 and title match; volume 15 article 3997. | DOI request 406; Crossref record exists. |
| 13 | 10.1088/1748-9326/acf7d7 | Huang and Song, 2023 and title match; add volume 18, article 103003. | DOI request 406; direct [IOP page](https://iopscience.iop.org/article/10.1088/1748-9326/acf7d7) loaded. |
| 14 | https://www.epa.gov/caddis/urbanization-hydrology | Institutional author and title match the page; no publication year is asserted in the review. Not a journal DOI. | Listed EPA page loaded. |
| 15 | 10.1038/s41586-018-0676-z | Zhang, Villarini, Vecchi and Smith, 2018 and title match; *Nature* 563, 384–388. | DOI request 406; direct [Nature page](https://www.nature.com/articles/s41586-018-0676-z) loaded. |

No DOI/title/first-author/year mismatch was found in the exact Crossref records. An HTTP 406 or 403 is an access issue, not a demonstrated 404. Direct publisher alternatives above are usable where the DOI resolver is blocked by the same client.

## Targeted claim audit

**6 — recharge and hydrology.** The [MDPI review](https://www.mdpi.com/2073-4441/2/3/605) explicitly reports 53 mm/year pre-urban direct recharge, 31 mm/year direct recharge around 2000 and 94 mm/year combined recharge from direct recharge, utility leakage and irrigation return. It attributes the water-balance example to Garcia-Fresca (2006), so the draft appropriately calls this a secondary historical estimate. These numbers are estimated budget components, not measured universal effects. The review also supports modified runoff and recharge pathways; it does not alone prove the exact effect in every landscape.

**7 — global flood extent.** The [paper](https://www.nature.com/articles/s43247-022-00598-0) identifies 106 selected large perennial river basins, 1985–2018, and states rainfall and urban area were the main explanatory variables in 57% of analyzed basins. The draft correctly interprets this as statistical explanatory-variable selection, not a 57% flood increase or causal effect. The dependent measure is annual maximum *seasonal surface-water extent within floodplains*, a satellite-derived flood proxy—not a comprehensive inventory of all short-lived urban floods. Urban area is represented by an artificial-impervious-area proxy. The paper describes a stepwise statistical analysis, with observational and omitted-variable limitations.

**11 — METROMEX.** Crossref identifies the cited 1976 paper, and an [indexed article description](https://doi.org/10.1175/1520-0450%281976%29015%3C0544%3AAHFURA%3E2.0.CO%3B2) surfaced by search describes the METROMEX-based hypothesis concerning St Louis and downwind rainfall anomalies. The modest statement that METROMEX-era work made urban rainfall anomalies a research issue is consistent. The phrase ‘rather than a universally reproducible rainfall multiplier’ is the review's interpretation, not a numerical result from the paper. Full text could not be examined at AMS due to HTTP 403.

**13 — humidity.** The [IOP review](https://iopscience.iop.org/article/10.1088/1748-9326/acf7d7) describes both urban moisture and dry islands, their temporal and climatic variability, and anthropogenic water inputs including irrigation. It also discusses irrigation's cooling–moisture and water-use trade-offs. This supports the cited broad claims. The specific assertion about measurement height was not separately located in the passages checked; retain only with a specific supporting passage or another source. Humidity metric choice is important: temperature-sensitive relative humidity and specific humidity need not yield the same sign.

**15 — Harvey.** The [Nature paper](https://www.nature.com/articles/s41586-018-0676-z) investigates the urban land-cover contribution to Harvey rainfall and flood response using atmospheric and hydrological modelling. The draft's event-specific counterfactual framing and cautions against treating it as a general hurricane or isolated global-warming estimate are consistent. The claim should not be expanded into an independently established effect for other storms.

## Residual risks

* The review's other quantitative claims were outside the requested detailed claim audit; bibliographic matches do not independently validate their calculations.
* DOI resolver requests were blocked by HTTP 406 from this client and the AMS route by 403. Browser or alternate-network behavior remains untested. Direct publisher pages were not checked for every paper.
* The independent second-index paper-by-paper cross-check remains outstanding; no mismatches were found in the exact Crossref records, but this is not a two-index attestation.
