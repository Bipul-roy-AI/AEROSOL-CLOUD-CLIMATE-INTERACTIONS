# Evidence audit: urbanisation–hydroclimate draft

## Summary

The draft is a selective narrative review of urban influences on temperature, rainfall, evapotranspiration, runoff and groundwater. It separates spatial contrasts from temporal change and conditional model experiments, and compiles source-specific quantitative examples.

I checked the full text of Sui [1], Xiong [2], Guccione [3], Hao [5], Mazzoleni [7] and the secondary review [6]; Du [4] was checked against its abstract. This was a targeted audit, not a full independent recalculation or verification of all 15 references. The FATAL and MAJOR classifications below distinguish demonstrated errors from important evidence-interpretation omissions.

## Strengths

- [S1] The table accurately distinguishes Guccione’s global station estimates (29% versus 19%) from the European model-domain estimates (17.8% versus 6.5%); the primary article reports these as changes in extreme-event occurrence, not depth [3].
- [S2] The 19-of-20 and approximately 215 mm/year ET figures, the 57% flood-basin statistic, and the 53/31/94 mm/year Austin values are traceable to the cited sources [5–7]. The Austin numbers are correctly presented as a secondary-source water budget.
- [S3] The discussion repeatedly warns that urban–rural contrasts do not by themselves identify an urbanisation effect; this is especially important for interpreting [1–3].

## Weaknesses

### FATAL

- **None established in the material checked.** No inspected source supports classifying the draft’s overall argument or a central numerical result as demonstrably fatal. This is not a certification of every citation or figure.

### MAJOR

- [W1] **MAJOR — apparently corroborating global rainfall figures share a key dataset, and a competing product result is omitted** (Abstract; §§2 and 5). Both Sui [1] and Xiong [2] use IMERG at 0.1°; their matching 63% values are therefore not independent satellite-product replication. More importantly, Xiong’s methods report that GSMaP did not effectively detect the expected global urban rainfall island, although IMERG performed better against gauges. The draft’s unqualified “Recent global satellite studies find predominantly positive annual urban–rural rainfall contrasts” masks this material product sensitivity. **Repair:** identify both results as IMERG-based, describe their distinct samples and rural definitions, and report the GSMaP non-replication alongside the authors’ gauge-validation rationale; avoid treating the two 63% shares as independent confirmation. Cite [1] and [2], methods and validation discussion. This omission does not prove IMERG is wrong.
- [W2] **MAJOR — station-trend comparison lacks the fixed classification needed to interpret attribution** (§2 global-gauge row; §5 Guccione paragraph). Guccione [3] groups stations by 2015 settlement conditions, not measured changes in each station’s urbanisation over 1962–2021; the authors report a 1975-classification sensitivity check with consistent significant results. The draft flags geographical confounding but leaves open the misleading inference that it compares trends at stations as they actually urbanised. **Repair:** say explicitly “stations classified urban or rural using 2015 settlement conditions” and note the 1975 sensitivity check; retain the warning that the difference is not a causal urbanisation effect. Do not describe 29% minus 19% as an identified treatment effect.
- [W3] **MAJOR — flood metric is labelled more directly than the observations warrant** (§2 flood row; §7). Mazzoleni [7] derives annual maximum flood extent using Landsat-derived surface-water observations; the mapped maximum is an observation-dependent proxy for seasonal surface-water/flood extent, not an independently verified inventory of flood events or necessarily a synchronous event footprint. The draft mentions missed short events, but “satellite-observed annual maximum water extent” and “Flooded extent” still invite reading it as measured flood hazard across basins. **Repair:** label the metric “Landsat-derived annual maximum surface-water/flood-extent proxy,” specify that revisit, cloud and water classification constrain detection, and preserve the noncausal interpretation of 57%. Confirm exact processing against [7] before adding further algorithmic detail.
- [W4] **MAJOR — arid irrigation reversal and geographic measurement gaps need direct evidence** (§6 and §9). The assertion that an irrigated arid city can have higher ET than its dry surroundings is plausible and consistent with the broad mechanisms in [5], but the immediately following claim is uncited and [5]’s abstract establishes urban *humidity* wet islands, not by itself an observed higher-ET arid-city example. Likewise, §9 names African, South Asian and Latin American cities and informal settlements as underrepresented in direct measurements without an inventory or citation establishing those particular comparisons. **Repair:** attach a specific arid-city ET flux or validated remote-sensing study to the ET claim, or qualify it as a plausible mechanism rather than an established empirical generalisation. Cite a global station/flux-network coverage inventory for the named regions and settlements, or narrow the claim to the evident sampling limitations of [1], [2] and [5]. Do not use humidity alone as proof of the ET sign.

## Questions for Authors

- [Q1] For [1] and [2], can the review report the explicit urban/rural definitions and quantify how many cities overlap? The common IMERG source is established; overlap of the actual city lists has not been checked here.
- [Q2] For [7], what exact annual surface-water statistic and threshold define the reported flood-extent proxy, and is it an observed snapshot or a composite? The review should quote the source’s methods rather than assume equivalence.
- [Q3] For the geographic coverage assertion in §9, what denominator and direct-measurement inventory support the named regional gaps and the specific claim about informal settlements?

## Verdict

**Revision required, primarily for evidence independence and interpretation rather than correction of the checked numerical values.** Confidence: **moderate** in the identified issues and in the checked figures; lower for completeness because the audit did not reproduce underlying analyses, inspect all references, or retrieve the original Garcia-Fresca Austin study.

## Revision Plan

1. [W1] Amend the abstract, table and §5 to identify IMERG as common to [1] and [2], and report Xiong’s GSMaP sensitivity and better gauge performance for IMERG together.
2. [W2] Add the 2015 fixed-classification detail and 1975 sensitivity result to the global station row or its adjacent text.
3. [W3] Relabel the Landsat flood outcome as a surface-water-derived proxy and add its observation-dependent interpretation; retain the 57% number as a model-selection result, not an effect size.
4. [W4] Add primary citations for the arid ET reversal and region-specific measurement gaps, or appropriately narrow the claims.
5. [Q1–Q3] If feasible, inspect city-list overlap, the original flood processing and the original Austin study. The latter remains a secondary-source estimate even though its arithmetic, 31 + 31 + 32 = 94 mm/year, is internally consistent in [6].

## Inline Annotations

> “Recent global satellite studies find predominantly positive annual urban–rural rainfall contrasts, alongside important exceptions and contrasts by intensity.”

**[W1] MAJOR:** Both global studies highlighted in the table use IMERG. Xiong also reports that GSMaP did not effectively detect the expected global urban rainfall island, while IMERG validated better against gauges. Add this product sensitivity and avoid implying independent product replication.

> “Event occurrence increased 29% at urban and 19% at rural stations [3].”

**[W2] MAJOR:** These are trends at stations classified using 2015 settlement conditions, not a comparison of measured station-level conversion trajectories. Add that classification and the reported 1975 sensitivity analysis.

> “Mazzoleni et al. [7] link urban area and rainfall statistically to satellite-observed annual maximum water extent in large basins”

**[W3] MAJOR:** Identify this as a Landsat-derived proxy for annual maximum flood/surface-water extent; its observation and classification limitations make it distinct from an event-by-event flood inventory. Check exact construction before specifying the composite method. **[Q2]**

> “But an irrigated urban landscape in an arid region can have more ET than its dry surroundings.”

**[W4] MAJOR:** Add a direct empirical ET citation or mark this as a plausible water-balance mechanism. Hao’s wet-island classification by humidity alone does not establish this particular ET comparison.

> “African, South Asian and Latin American cities, informal settlements and smaller rapidly expanding cities remain insufficiently represented by direct measurements.”

**[W4; Q3] MAJOR:** Supply a comparative global monitoring inventory or soften to a documented sampling limitation. Specific regional and settlement-type underrepresentation is not demonstrated by the citations adjacent to this sentence.

## Sources

Primary and secondary sources additionally inspected for this audit (direct URLs):

- Sui et al., full text: https://pmc.ncbi.nlm.nih.gov/articles/PMC11420207/
- Xiong et al., full text and methods: https://pmc.ncbi.nlm.nih.gov/articles/PMC12214829/
- Guccione et al., full text and methods: https://www.nature.com/articles/s44304-026-00173-z
- Du et al., abstract and bibliographic record: https://doi.org/10.1029/2023GL104661
- Hao et al., full text: https://www.nature.com/articles/s41612-023-00479-z
- Sun and Lockaby review, Austin case summary: https://www.mdpi.com/2073-4441/2/3/605
- Mazzoleni et al., full text: https://www.nature.com/articles/s43247-022-00598-0
