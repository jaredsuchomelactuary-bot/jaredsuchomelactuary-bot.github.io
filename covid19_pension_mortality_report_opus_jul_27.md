# The COVID-19 Pandemic and U.S. Pension Mortality Assumptions

## A Research Report on Implications for Mortality Modeling by U.S. Pension Actuaries

**Prepared:** July 2026
**Status:** Draft for review and discussion — educational research report
**Scope:** United States defined benefit pension plans (private single-employer, multiemployer, and public sector)

---

## 1. Executive Summary

The COVID-19 pandemic produced the largest short-term disruption to U.S. mortality in a century. U.S. period life expectancy at birth fell from 78.8 years in 2019 to 77.0 in 2020 and 76.4 in 2021 — the largest two-year decline since 1921–1923 — before recovering to 77.5 in 2022, 78.4 in 2023, and a record 79.0 in 2024 (NCHS 2022, 2024, 2026). For the population aged 65 and older, the population most relevant to pension liabilities, age-standardized deaths ran approximately 17% above expected levels in 2020 and 15% above expected in 2021 (measured against 2019 mortality projected forward with Scale MP-2021), falling to roughly 1.3% above expected for the twelve months ending June 2025 (SOA RPEC 2025).

This report examines what that experience implies for the mortality assumptions — base tables, improvement scales, and projection methodology — used by U.S. pension actuaries. Its principal findings are:

**Finding 1 — The pandemic is best modeled as a large transitory shock plus a smaller, uncertain persistent shift, not as a change in trend.** The acute mortality spike of 2020–2022 has largely dissipated at pension-relevant ages, and mortality at ages 65+ is now near, though slightly above, the pre-pandemic trajectory. Mechanically extrapolating 2020–2021 data into an improvement scale would badly distort projected trends; the Society of Actuaries' Retirement Plans Experience Committee (RPEC), the U.K.'s Continuous Mortality Investigation (CMI), and the Social Security Administration (SSA) have all, in different ways, excluded, down-weighted, or explicitly overlaid the pandemic years rather than allowing them to flow through standard trend-fitting machinery.

**Finding 2 — Residual excess mortality is small at retirement ages but is not zero, and it differs by sex and age.** RPEC estimates excess mortality at ages 65+ of approximately 1.3% for July 2024–June 2025 relative to MP-2021-projected 2019 rates (about 0.5% for males and 2.1% for females), and offers practitioners a mechanism to reflect this as an explicit load through the MIM-2021 model. Meanwhile, working-age mortality — particularly for males aged 35–44 — remains materially above 2019 levels, which matters for pre-retirement decrements, death-in-service benefits, and the long-run health of cohorts now approaching retirement.

**Finding 3 — No updated standard improvement scale is likely before approximately 2029, so the assumption-setting burden currently sits with individual actuaries.** MP-2021, fitted to data through 2019, remains the most recent published scale. RPEC's graduation methodology requires roughly five years of clean post-pandemic data, and Medicare data arrives with a two-plus-year lag; RPEC declined to publish a new scale in 2025 and signaled a full traditional update may not arrive until fall 2029. In the interim, actuaries must decide — and document under ASOP No. 35 and ASOP No. 41 — how, if at all, to adjust published assumptions.

**Finding 4 — The pandemic's sharply unequal impact by race, ethnicity, and socioeconomic status has direct modeling consequences.** Between 2019 and 2021, life expectancy fell 6.6 years for American Indian and Alaska Native (AIAN) people, 4.2 years for Hispanic people, and 4.0 years for Black people, versus 2.4 years for White people (KFF 2026; NCHS). Because U.S. pension mortality tables do not stratify by race but do stratify by proxies correlated with it (collar, income quartile, plan type), differential pandemic mortality (a) widened the gap between general-population data and insured pension populations, (b) shifted the surviving population's composition in ways that can masquerade as mortality improvement in aggregate data, and (c) interacts with long-run demographic change — the U.S. retiree population is becoming markedly more racially and ethnically diverse — to make population-level improvement scales an increasingly imperfect proxy for any particular plan.

**Finding 5 — For plans subject to prescribed assumptions, the regulatory framework has already embedded a specific answer.** The IRS final regulations under IRC §430(h)(3) (T.D. 9983, October 2023), effective for plan years beginning in 2024, adopt the Pri-2012 base tables with "2024 Adjusted Scale MP-2021 Rates" that eliminate assumed mortality improvement for 2020–2023 and cap future annual improvement at 0.78% pursuant to the SECURE 2.0 Act. Public plans and accounting valuations retain far more discretion, making the treatment of pandemic experience a live assumption-setting question there.

The report closes with nine recommendations, ranging from adopting an explicit, documented COVID treatment (rather than silence) to sensitivity testing, monitoring plan-specific experience with credibility procedures, and incorporating socioeconomic-based mortality differentiation where data permits.

---

## 2. Purpose, Scope, and Intended Users

This report is an educational research document. It synthesizes publicly available mortality data and published actuarial research to address one question: **how should the 2020 COVID-19 pandemic change the way U.S. pension actuaries model mortality?** "Model mortality" is interpreted broadly to include the choice of base table, the choice and modification of mortality improvement scales, the treatment of 2020–2023 experience data in experience studies, assumption governance and disclosure, and scenario/stochastic analysis of longevity risk.

The intended audience is retirement actuaries and actuarial students. The report does not constitute actuarial advice for any specific plan, does not reflect the circumstances of any particular covered population, and is not a Statement of Actuarial Opinion under the Actuarial Standards of Practice (ASOPs). Actuaries applying any approach described here remain responsible for compliance with ASOP No. 35 (Selection of Demographic and Other Noneconomic Assumptions), ASOP No. 25 (Credibility Procedures), ASOP No. 23 (Data Quality), and ASOP No. 41 (Actuarial Communications).

---

## 3. Background: The Pre-Pandemic Mortality Assumption Framework

U.S. pension mortality assumptions are conventionally built from two components.

**Base mortality tables** describe the level of mortality for a reference population in a reference year. The current standard tables are the Pri-2012 Private Retirement Plans Mortality Tables (SOA 2019) for private plans and the Pub-2010 Public Retirement Plans Mortality Tables (SOA 2019b) for public plans. Both are published by RPEC with variants by sex, annuitant/non-annuitant status, and socioeconomic proxies: collar and benefit-amount quartile for Pri-2012, and job category (teachers, public safety, general employees) plus income level for Pub-2010. Notably, neither family of tables stratifies by race or ethnicity; socioeconomic proxies carry that variation only indirectly.

**Mortality improvement scales** project how base rates change over time. The MP-series scales (MP-2014 through MP-2021), produced by RPEC primarily from Medicare experience data graduated with two-dimensional Whittaker–Henderson smoothing, provide age- and calendar-year-specific improvement rates that blend recent observed trends into an assumed long-term rate over a convergence period. In 2021 the RPEC model was folded into the Mortality Improvement Model (MIM-2021), an Excel-based framework — updated most recently as MIM-2021-v4b (October 2024) — that lets practitioners construct their own improvement assumptions by choosing data sets, weights, smoothing, and long-term rates (SOA 2021, 2024b). Generational projection (each cohort's rates improving through its own future lifetime) is the prevailing practice.

Critically for what follows: **Scale MP-2021 reflects historical data only through 2019.** It is, by construction, a pre-pandemic view of mortality trend. Every U.S. pension valuation performed since has therefore had to answer, implicitly or explicitly, how observed 2020+ experience should modify a 2019-vintage projection.

For single-employer private plan minimum funding and lump sums, mortality is prescribed by regulation under IRC §430(h)(3) and §417(e); Section 7.6 describes how the IRS resolved the COVID question for those purposes. For accounting measurements (ASC 715; GASB 67/68) and public-sector funding valuations, mortality is a best-estimate assumption selected by the actuary, and the questions examined in this report apply with full force.

---

## 4. Data and Sources

The analysis and figures in this report rest on the following publicly available sources. Section 10 provides full citations, and Appendix A outlines reproducible exercises using the raw data.

**Human Mortality Database (HMD), mortality.org.** The HMD U.S. series now includes deaths, exposures, death rates, and complete period life tables through 2024, with January 1 population estimates through 2025, in age × year configurations from 1×1 to 5×10. HMD is the cleanest single source for reproducing the aggregate results discussed here (life expectancy path, age-specific rate ratios 2020–2024 versus 2019, age-standardized death rates). Downloading requires free registration and acceptance of the user agreement. HMD's Short-Term Mortality Fluctuations (STMF) series additionally provides weekly deaths, useful for studying the wave structure of pandemic mortality.

**CDC / National Center for Health Statistics (NCHS).** Final mortality data through 2024 ("Mortality in the United States, 2024," Data Brief 548, January 2026; and the National Vital Statistics Reports underlying it), CDC WONDER for cause-, race-, and age-specific death counts, and NCHS life tables by race and Hispanic origin. NCHS is the authoritative source for race/ethnicity-stratified results, including adjustments for race misclassification on death certificates (a material issue for AIAN mortality, where roughly a third of deaths have historically been misclassified; NCHS 2021).

**SOA Research Institute / RPEC.** The Pri-2012 and Pub-2010 reports, Scale MP-2021, the MIM-2021 model and tools, and — most importantly for current practice — the annual RPEC Mortality Improvement Updates (2022–2025), which track actual-to-expected mortality against MP-2021 using CDC death counts and SSA population estimates.

**Social Security Administration.** The 2025 OASDI Trustees Report and its Long-Range Demographic Assumptions document, which disclose the Trustees' explicit COVID-19 mortality factors and the Social Security Area Population estimates RPEC uses for exposure.

**U.S. Census Bureau.** Population estimates and the 2023 National Population Projections, the standard reference for the projected size and racial/ethnic composition of the older population.

**International references.** CMI Working Paper 201 and the CMI_2024 Mortality Projections Model (U.K.), and the Canadian Institute of Actuaries' 2024 mortality improvement research ("CanMI-2024"), both summarized in SOA RPEC (2025), provide useful methodological contrast.

---

## 5. U.S. Mortality Experience, 2020–2025

### 5.1 Aggregate Experience

More than 1.1 million U.S. deaths have been attributed to COVID-19 as underlying or contributing cause since March 2020, concentrated overwhelmingly in 2020–2022. The resulting path of period life expectancy at birth (e₀) is summarized below (NCHS final data; HMD values are essentially identical):

| Year | e₀ (years) | Change | Age-adjusted death rate (per 100,000) |
|------|-----------|--------|----------------------------------------|
| 2019 | 78.8 | — | 715.2 |
| 2020 | 77.0 | −1.8 | 835.4 |
| 2021 | 76.4 | −0.6 | 879.7 |
| 2022 | 77.5 | +1.1 | 798.8 |
| 2023 | 78.4 | +0.9 | 750.5 |
| 2024 | 79.0 | +0.6 | 722.1 |

Life expectancy at age 65 followed a similar V-shape, reaching 19.7 years in 2024. By 2024, COVID-19 had fallen out of the ten leading causes of death (replaced by suicide at #10), and deaths involving synthetic opioids fell 35.6% from 2023 — a reminder that not all of the 2020–2023 excess, and not all of the subsequent recovery, is COVID-19 itself. Drug overdose, cardiovascular, diabetes, and "deaths of despair" dynamics moved materially over the same window and interact with pandemic effects (NCHS 2026).

Two features of this path matter for assumption-setting. First, the shock was enormous but predominantly **transitory**: 2024 age-adjusted mortality was slightly *better* than 2019 (722.1 vs. 715.2 per 100,000 is within ~1%, and e₀ reached an all-time high). Second, the recovery was **not uniform** across ages, sexes, or population subgroups, as the next two subsections show.

### 5.2 Age Pattern and Pension Relevance

COVID-19 death rates rose steeply with age, so the absolute burden fell heavily on retirement ages; but *proportional* excess mortality was actually highest in midlife, and midlife is where excess has proven most persistent. RPEC's age-standardized actual-to-expected (A/E) ratios versus 2019 rates (no improvement), for the twelve months ending June 2025, illustrate the residual pattern (SOA RPEC 2025, Table 2):

| Age group | Females | Males |
|-----------|---------|-------|
| 15–24 | 92.2% | 93.2% |
| 25–34 | 88.8% | 90.1% |
| 35–44 | 101.7% | 106.8% |
| 45–54 | 96.4% | 100.4% |
| 55–64 | 96.7% | 96.4% |
| 65–74 | 99.4% | 99.8% |
| 75–84 | 98.1% | 96.0% |
| 85+ | 98.8% | 96.4% |

Mortality at ages 15–34 is now well *below* 2019 levels (driven substantially by declining overdose deaths), mortality at 65+ is at or slightly below 2019 levels, but male mortality at 35–44 remains roughly 7% above 2019. For pension work this pattern cuts three ways: retiree annuitant mortality has essentially normalized in level terms; active-participant decrements and death-in-service experience at midlife may still run above pre-pandemic tables; and elevated midlife mortality and morbidity in current working cohorts is a plausible headwind for the improvement those cohorts experience as they age into retirement.

### 5.3 Actual-to-Expected Experience Versus MP-2021

The comparison that matters most for improvement-scale purposes is against 2019 mortality *projected forward with MP-2021* — i.e., how far actual experience has diverged from the assumption most valuations were using. RPEC's age-standardized results for the 65+ population (CDC deaths / SSA exposures; Medicare data corroborates within ~0.6% where available):

| Period | A/E vs. 2019 + MP-2021 |
|--------|------------------------|
| 2020 | 116.7% |
| 2021 | 114.6% |
| 2022 | 109.5% |
| 2023 | 102.1% |
| 2024 | 100.7% |
| Jul 2024 – Jun 2025 | 101.3% (males 100.5%, females 102.1%) |

Read literally: five years after the pandemic began, the 65+ population is dying at almost exactly the rate MP-2021 projected — the cumulative *level* shock has nearly washed out relative to the pre-pandemic trend line, with a residual of roughly 1% concentrated more in females than males. Note also the base-year dependence RPEC highlights: measured against a 2012 base year (relevant where Pri-2012 is used un-adjusted with MP-2021), the corresponding A/E ratios are about 101.6% for males and 102.5% for females (SOA RPEC 2025, Table 4). Whether that residual persists indefinitely, decays further, or re-widens is precisely the assumption an actuary must now take a position on; Section 7 takes up that question.

---

## 6. Demographic Heterogeneity: Race, Ethnicity, Socioeconomic Status, and Compositional Change

### 6.1 The Pandemic Was Not Experienced Equally

Aggregate national figures conceal enormous dispersion. Life expectancy at birth by race and Hispanic origin (NCHS life tables, adjusted for race and ethnicity misclassification on death certificates) moved as follows:

| Group | Change 2019 → 2021 | Change 2021 → 2023 | e₀ in 2023 |
|-------|--------------------|--------------------|------------|
| American Indian / Alaska Native (AIAN), non-Hispanic | −6.6 years | +4.5 years | 70.1 |
| Hispanic | −4.2 years | +3.5 years | 81.3 |
| Black, non-Hispanic | −4.0 years | +2.8 years | 74.0 |
| White, non-Hispanic | −2.4 years | — | 78.4 |
| Asian, non-Hispanic | −2.1 years | — | (highest of groups reported) |
| **Total population** | **−2.7 years** | **+2.0 years** | **78.4** |

Sources: KFF (2026) compilation of NCHS life tables; NCHS NVSR 72-12 (2023) and NVSR 74-6 (2025).

Several features deserve emphasis:

**The Black–White life expectancy gap reversed decades of convergence.** The gap had narrowed from 7.1 years in 1993 to 4.0 years in 2019; it widened to 5.9 years in 2020 (NCHS, NVSR 72-12). Partial re-narrowing followed, and NCHS reported that the largest 2023-to-2024 rate decreases occurred among younger age groups, Black non-Hispanic people, and males — but the episode demonstrates that subgroup mortality trends can diverge sharply and rapidly from the national aggregate.

**AIAN mortality data requires misclassification adjustment.** Approximately 34% of non-Hispanic AIAN deaths are misclassified as another race on death certificates (NCHS 2021, "Mortality Profile of the Non-Hispanic American Indian or Alaska Native Population, 2019"). Unadjusted CDC WONDER extracts will therefore materially understate AIAN mortality; NCHS life tables by race apply an adjustment. Any actuary working with race-stratified public data should use the adjusted series and disclose the adjustment.

**Excess mortality concentrated at younger ages for non-White populations.** Decomposition analyses find that increases in deaths at ages 40–64 alone accounted for life expectancy declines of 2.09 years (Native American), 1.18 years (Hispanic), and 1.08 years (Black) between 2019 and 2021 — each individually exceeding the *total* mean life expectancy decline of 0.39 years across peer high-income countries (Bor et al. / related decomposition work, Am J Public Health / PMC10773482). This is important for pension modeling because pre-retirement excess mortality has different actuarial consequences than post-retirement excess mortality: it reduces the number of participants reaching retirement, changes the composition of those who do, and affects pre-retirement death benefit costs — but it does not reduce annuity liability by shortening the lives of people already in pay status.

**Non-COVID causes contributed disproportionately in non-White populations.** Increases in deaths not attributed to COVID-19 (overdose, homicide, cardiovascular, diabetes) contributed relatively large life expectancy declines among Native American, Black, and Hispanic populations, especially at younger ages. This matters for projection because a portion of the "pandemic" mortality shock in these groups reflects trends in causes that predate COVID-19 and may persist independently of it.

### 6.2 Why This Matters When U.S. Pension Tables Have No Race Dimension

U.S. pension mortality tables do not contain a race or ethnicity variable, and there is no realistic prospect of one. Race is not collected in most plan administrative data, and its use as a rating or assumption-setting variable would raise legal and ethical objections. RPEC's tables instead differentiate on socioeconomic proxies: **Pri-2012** by collar (blue/white) and benefit-amount quartile; **Pub-2010** by job category (general, teachers, public safety) and by above/below-median benefit amount.

These proxies capture part — but only part — of the variation observed by race and ethnicity, because race, occupation, income, and mortality are correlated but far from collinear. The practical implications for pension modeling are four:

1. **General-population improvement scales embed a compositional mix that no plan matches.** MP-scales are fitted to Medicare (i.e., near-universal 65+) experience. A plan whose covered population differs from the national 65+ mix in race, occupation, income, and geography will not have experienced the pandemic in the same magnitude. RPEC states this directly: excess mortality varies significantly from one pension population to another, and, anecdotally, has generally been less severe in pension populations than in the general U.S. population (SOA RPEC 2025, §4).

2. **Aggregate improvement can be manufactured by compositional change.** If a subpopulation with above-average mortality suffers disproportionate pandemic losses, the survivors are a healthier-than-before mix, and subsequent aggregate death rates fall for reasons unrelated to any individual's mortality improving. This "mortality displacement" or harvesting effect — plus straightforward selection, since COVID-19 mortality was heavily concentrated among the frail and comorbid — is one plausible explanation for why 2023–2024 mortality at older ages came in *below* 2019 levels. An improvement scale fitted naively to 2020–2024 data would read that compositional artifact as genuine trend improvement and project it forward, which would be a modeling error.

3. **Long-run compositional change is running in the same direction.** The 65-and-older U.S. population is projected to grow from roughly 58 million in 2022 to approximately 78 million by 2040 and 89 million by 2060, and to become substantially more diverse: earlier Census projections put the 65+ population in 2060 at roughly 56% non-Hispanic White, 21% Hispanic, and 13% non-Hispanic Black, versus a far higher White share today; the Hispanic share of the 65+ population is projected to rise from about 9% in 2020 to roughly 21% by 2060 (U.S. Census Bureau 2018/2023 projections; ACL 2023 Profile of Older Americans). The Census Bureau's 2023 National Population Projections were explicitly updated to account for the impact of COVID-19. Any long-horizon pension projection using national mortality trends is therefore implicitly importing a changing racial and ethnic mix, and — separately — the composition of a given plan's own retiree population is likely shifting as older, less diverse cohorts are replaced by younger, more diverse ones.

4. **Compositional change does not translate mechanically into higher or lower plan mortality.** The direction is genuinely ambiguous. The "Hispanic paradox" — Hispanic life expectancy exceeding non-Hispanic White life expectancy despite lower average income — means a plan whose retiree population is becoming more Hispanic may see *improving* aggregate mortality from composition alone, even though Hispanic populations suffered among the worst pandemic-era losses. Conversely, an increasing Black or AIAN share would push aggregate mortality the other way. And because pension participation is itself selective on employment, income, and job stability, a plan's demographic mix is not the general population's mix. **The practical implication is not that actuaries should model race; it is that actuaries should be skeptical of national-population improvement scales as a substitute for plan-specific analysis, and should test the sensitivity of results to the assumption that the plan's population will continue to track the national trend.**

### 6.3 Socioeconomic Gradients as the Practical Modeling Channel

The workable channel for reflecting the heterogeneity described above is socioeconomic differentiation, for which published tools already exist:

- **Pri-2012 and Pub-2010 sub-tables** by collar, benefit quartile, job category, and income level. Where a plan's data supports it, selecting the sub-table matching the covered population — rather than the headline "total" table — is the single most direct way to reflect socioeconomic mortality differences.
- **Differentiated improvement by socioeconomic group.** MIM-2021 permits construction of custom improvement assumptions from alternative data sets and weights; RPEC's research and the SOA's broader mortality/longevity program have documented that improvement rates themselves differ by socioeconomic status, not merely mortality levels.
- **Geographic and index-based approaches.** Commercial longevity analytics (e.g., postcode/ZIP-based scoring) and public deprivation indices offer further granularity, subject to ASOP No. 23 data-quality and ASOP No. 25 credibility considerations.

---

## 7. Implications for Mortality Modeling

### 7.1 The Central Modeling Question: Transitory, Permanent, or Both

Every treatment of pandemic experience is, at bottom, a decomposition of observed 2020+ mortality into:

- a **transitory** component (the acute pandemic waves, plus mortality displacement in their aftermath),
- a possible **permanent level shift** (long COVID sequelae, delayed diagnoses and deferred care, healthcare system strain, behavioral and economic scarring), and
- the **underlying trend** the actuary wishes to project.

The three major published frameworks answer this differently, and the contrast is instructive:

| Framework | Treatment of pandemic years | Assumed persistence |
|-----------|----------------------------|---------------------|
| **SSA (2025 Trustees Report)** | Explicit multiplicative COVID factors applied to a counterfactual "baseline" by broad age group: e.g., 1.16 (2020), 1.17 (2021), 1.10 (2022), 1.03 (2023), 1.02 (2024) at ages 65–84; factors return to 1.00 for 2026 and thereafter | **No** long-term residual effect assumed. SSA notes 2024 factors below 1.00 at ages 15–64 and 85+, consistent with acute-phase deaths having primarily *accelerated* deaths that would have occurred later |
| **U.K. CMI (CMI_2024, June 2025)** | Prior versions gave 0% weight to 2020–2021 and 15% to 2022–2023. CMI_2024 replaced this with a **"fitted overlay"** approach: experience is decomposed into "underlying" and "overlay" mortality, with the overlay decaying at an assumed half-life *H*; the Core setting is *H* = 1 (excess halves each year from 2020). Five age terms were introduced to capture differing age-specific post-pandemic levels | **Partial, decaying.** Core CMI_2024 raises cohort life expectancies relative to CMI_2023 by ~1.25%–2.5% for males 65+ and ~0.15%–1.5% for females 65+ |
| **Canada (CIA / "CanMI-2024", April 2024)** | Scale developed from HMD data **1989–2019** — i.e., pre-pandemic only. Long-term improvement rate of 1.3% attained around 2059, up from 0.8% (CPM-B) and 1.0% (MI-2017) | **No** lingering pandemic effect assumed |
| **SOA RPEC (2021–2025)** | MP-2021 unchanged (data through 2019). RPEC declines to publish a COVID-adjusted scale, citing uncertainty, but explicitly enables practitioners to add their own load via MIM-2021 | **Practitioner's choice**, with 1.3% (65+, 2025+) offered as a documented candidate load |

The methodological convergence across these bodies is that **pandemic-year data must not be fed unweighted into standard trend-fitting**. The divergence is on residual persistence — where SSA and the CIA assume none, and the CMI assumes a decaying remainder.

### 7.2 Treatment of Pandemic-Year Data in Plan Experience Studies

For plan-level experience studies covering periods that include 2020–2022, the leading options are:

- **Exclude 2020–2021 (and possibly 2022) entirely.** Simple, transparent, and defensible where the pandemic effect is judged non-recurring. Cost: reduced exposure and therefore credibility, which under ASOP No. 25 may force greater reliance on the standard table.
- **Down-weight pandemic years.** The CMI's pre-2024 approach. Preserves some information without letting the shock dominate.
- **Overlay/decompose.** The CMI_2024 approach: model an excess-mortality overlay decaying with an assumed half-life, fit underlying mortality to all years net of that overlay. More sophisticated and more assumption-dependent; requires disclosure of the half-life parameter, to which results are sensitive.
- **Substitute expected values for pandemic years.** RPEC identifies this as a candidate alternative method: fill 2020–2022 with MP-2021-expected mortality, then graduate including 2023+ actual data.
- **Cause-of-death adjustment.** Remove COVID-19-coded deaths from 2020–2022 experience. Attractive in principle, but understates true pandemic effect (excess deaths exceeded COVID-coded deaths) and is sensitive to certification practice; use with caution and disclosure.

Whichever is chosen, the choice itself is a material assumption and should be disclosed under ASOP No. 41, with the rationale and the sensitivity of the result documented.

### 7.3 Improvement Scale: Practical Options for 2026 Valuations

Given that MP-2021 remains the most recent published scale and no successor is expected imminently, an actuary setting a best-estimate improvement assumption today has roughly five defensible positions:

**Option A — MP-2021 unmodified.** The status quo. Defensible on the grounds that 65+ A/E versus MP-2021 is now ~101%, i.e., MP-2021 has proven approximately right in aggregate, and that RPEC does not believe modified assumptions are inherently better predictors. Weakness: a growing share of MP-2021's projection period now sits at or past the end of its horizontal convergence period, meaning the scale is increasingly just its long-term rate, and it embeds no information from six years of subsequent experience.

**Option B — MP-2021 with a permanent COVID load.** RPEC's documented approach: add a level load to ages 65+ in the 2025+ columns of MIM-2021 Tab 1, Step 5 — 1.3% combined, or sex-distinct 0.5% male / 2.1% female. **Critically, if the base table is Pri-2012 (central year 2012) rather than a 2019-based table, the base-year-consistent loads are 1.6% male / 2.5% female** (SOA RPEC 2025, Table 4). Choosing loads calibrated to the wrong base year is an easy and material error.

**Option C — MP-2021 with a decaying COVID load.** A CMI-style overlay: apply the current ~1.3% excess and decay it to zero over a stated period (e.g., half-life of one to two years, or straight-line to zero by 2030). Sits between Options A and B and is arguably the best match to the observed trajectory, which has declined monotonically from ~17% to ~1.3%.

**Option D — Custom scale built in MIM-2021.** Use the Application Tool with pandemic years zero- or low-weighted, an extended convergence period, and/or an alternative long-term rate. Most flexible; heaviest documentation burden. Note RPEC's caution that such modifications are not demonstrably better predictors.

**Option E — Prescribed.** For IRC §430 funding and §417(e) lump sums, none of the above applies: the actuary uses the mandated tables (Section 7.6).

For plan sponsors and boards, the difference between Options A and B is usually small — on the order of a 1% shift in mortality rates translates to well under 1% of liability for a typical retiree population — but it is not nothing, and it is a difference the actuary should be able to explain and quantify.

### 7.4 Base Table Considerations

The base tables in current use predate the pandemic in their underlying data (Pri-2012 centered on 2012; Pub-2010 on 2010). Three points follow:

- **Base-year consistency is essential** when applying any COVID load or A/E adjustment, as noted in Option B above. Table 4 of the 2025 RPEC update gives A/E ratios for base years 2010 through 2019 for exactly this purpose; they range from 103.0% (2010 base) to 99.9% (2015 and 2017 bases), which is a wider spread than the headline number suggests.
- **Sub-table selection matters more than COVID adjustment for most plans.** The spread between Pri-2012 white-collar and blue-collar tables, or between Pub-2010 above- and below-median tables, is generally an order of magnitude larger than a 1–2% COVID load. An actuary who has not revisited sub-table selection is likely mis-specifying mortality far more seriously than one who has taken no COVID position.
- **Plan-specific base table adjustment factors** derived from experience studies remain the strongest tool where credibility permits — but see Section 7.2 on how to handle the pandemic years within those studies.

### 7.5 Selection, Displacement, and the Risk of Over-Reading Recent Data

Three mechanisms argue for caution in reading the low 2023–2024 mortality rates as evidence of an improved underlying trend:

- **Mortality displacement (harvesting).** Deaths pulled forward from 2023–2025 into 2020–2022 depress subsequent rates temporarily. SSA's assumption framework explicitly relies on this interpretation.
- **Selection within retiree populations.** Frailer annuitants died disproportionately, leaving a healthier surviving cohort — a level effect on the surviving group that is not improvement.
- **Cause-mix shifts unrelated to COVID.** The 35.6% single-year decline in synthetic-opioid deaths from 2023 to 2024 is a large, genuinely non-COVID contributor to recent aggregate improvement, concentrated at ages that barely affect annuity liability but which move headline life-expectancy numbers.

The practical implication: an improvement assumption should not be raised on the strength of two good years, any more than it should have been cut on the strength of two bad ones.

### 7.6 The Prescribed-Assumption Environment

For private single-employer plans, the IRS final regulations under IRC §430(h)(3) (published October 20, 2023; T.D. 9983), effective for plan years beginning on or after January 1, 2024, resolve the question by fiat:

- **Base tables:** Pri-2012 (base year 2012), gender-distinct, annuitant and non-annuitant.
- **Improvement:** the "2024 Adjusted Scale MP-2021 Rates," an IRS-constructed table that **eliminates the mortality improvement that would otherwise have been assumed for 2020 through 2023** and, per the SECURE 2.0 Act of 2022, **caps annual mortality improvement at 0.78% at all ages** for valuation dates in and after 2024.
- **Generational projection required** except for small plans (500 or fewer participants), which may use static combined tables.
- Net effect versus the prior RP-2014/MP-2016 basis: generally *lower* §430 funding liabilities and lower §417(e) minimum lump sums (on the order of 1%–1.5% for a typical annuity-based plan, varying by demographics), while the COVID and 0.78% adjustments push in the opposite direction relative to unadjusted Pri-2012/MP-2021.

Separately, the IRS issued proposed regulations on **substitute mortality tables** that include an adjustment to the mortality ratio to account for COVID-19's impact — relevant to any plan pursuing plan-specific tables under §430(h)(3)(C).

Two observations for practitioners. First, the regulatory answer is a policy choice embedding a *specific* view (no improvement 2020–2023, capped improvement thereafter) that is more conservative than the best-estimate views discussed above; it should not be mistaken for, or defaulted into, a best estimate for accounting or public-plan purposes. Second, the resulting divergence between prescribed funding mortality and best-estimate accounting mortality is now larger than it was pre-pandemic, and that divergence needs to be explained to sponsors.

### 7.7 Uncertainty, Scenarios, and Longevity Risk

The pandemic's most durable lesson for mortality modeling may be about **variance rather than level**. Prior to 2020, U.S. pension practice treated a 15–20% one-year deviation in aggregate 65+ mortality as effectively outside the plausible range; it happened twice in consecutive years. Reasonable responses include:

- **Scenario testing** with explicit alternatives: no residual excess (SSA/CIA view), permanent 1.3% load (RPEC's illustrative view), decaying overlay (CMI view), and an adverse scenario in which post-pandemic health effects (long COVID prevalence, deferred cancer and cardiovascular diagnoses) produce a larger persistent load.
- **Stochastic mortality modeling** (Lee–Carter, Cairns–Blake–Dowd and variants) explicitly recognizing that the historical volatility parameter estimated on 1950–2019 data understates realized tail risk; jump-diffusion or regime-switching extensions to capture pandemic-type events have a substantial academic literature and are worth considering for risk (as opposed to funding) applications.
- **Reverse stress testing:** how large a permanent mortality shift would be needed to change a funding, de-risking, or pension risk transfer decision? Often the answer is "much larger than any plausible COVID load," which is itself a useful and calming result to communicate.

---

## 8. Recommendations

1. **Take an explicit position on pandemic experience and document it.** Silence is itself a choice — continuing MP-2021 unmodified is a defensible position, but it should be an argued one, disclosed under ASOP No. 41, not a default.

2. **Do not let 2020–2022 data flow unweighted into trend fitting.** Exclude, down-weight, overlay, or substitute expected values, and disclose which was done. Every major standard-setting body has taken this position.

3. **If applying a COVID load, match it to the base table's central year.** ~1.3% (0.5% M / 2.1% F) against a 2019 base; ~2.0% (1.6% M / 2.5% F) against a 2012 base such as Pri-2012. Getting this wrong is a common and avoidable error.

4. **Prefer a decaying overlay to a permanent load unless there is a specific reason to believe otherwise.** The observed trajectory (17% → 15% → 10% → 2% → 1%) is far better described by decay than by a step to a new permanent level, and the SSA and CIA both assume full reversion.

5. **Spend effort on base-table and sub-table selection before spending it on COVID adjustments.** Collar, income quartile, and job-category selection typically move liability by multiples of any plausible COVID load. Where the plan's population differs materially from the national mix, this is where that difference gets reflected.

6. **Monitor plan-specific experience formally, and apply ASOP No. 25 credibility procedures.** RPEC's own guidance is that excess mortality varies significantly across pension populations and has generally been milder than in the general population — so national A/E ratios are a starting point, not an answer.

7. **Reflect demographic and compositional change explicitly in long-horizon projections.** For open plans and for public plans projecting decades forward, the racial, ethnic, and socioeconomic composition of the covered population in 2050 will not be its composition today. Where the plan's data supports segment-level analysis, model it; where it does not, sensitivity-test the assumption that the plan will track national trends.

8. **Distinguish pre- and post-retirement mortality effects.** Residual excess is concentrated at working ages (males 35–44 remain ~7% above 2019), where it affects death-in-service benefits, headcount reaching retirement, and — over a longer horizon — the health of cohorts now entering retirement. Retiree annuitant mortality has largely normalized. A single aggregate adjustment obscures this.

9. **Widen the modeled range of longevity outcomes, not just the central estimate.** The pandemic demonstrated that mortality is subject to shocks outside the range implied by late-20th-century volatility. Build that into scenario and stochastic work, and communicate it to sponsors and boards as a risk-management insight rather than a funding-basis change.

---

## 9. Reliance, Limitations, and Caveats

- This report relies entirely on publicly available secondary data and published research; no plan-specific data was analyzed and no independent audit of source data was performed.
- Figures cited from the SOA RPEC 2025 update are, per RPEC's own characterization, best estimates rather than hard data, because CDC death counts are paired with estimated SSA exposures; RPEC's estimates for prior periods have been revised as SSA population estimates were refined (the July 2023–June 2024 excess estimate moved from 2.5% to 1.8% on revised exposures).
- Life expectancy figures are period measures and are not the cohort measures relevant to annuity valuation; they are used here as summary indicators of the shock's size, not as valuation inputs.
- Race and ethnicity data on death certificates is subject to misclassification; figures cited from NCHS life tables incorporate NCHS's misclassification adjustment, but residual error remains, particularly for AIAN and multiracial populations.
- National-population results do not translate directly to any pension population. Selection into pension coverage, geography, occupation, and income all drive material differences.
- The report reflects information available through July 2026. RPEC's 2026 update (expected fall 2026) and subsequent CMS data releases may change the picture materially.

---

## 10. References and Data Sources

**Data**

- Human Mortality Database. University of California, Berkeley (USA), and Max Planck Institute for Demographic Research (Germany). U.S.A. country page: https://mortality.org/Country/Country?cntr=USA — deaths (1×1 through 5×10), exposures, Mx, age-standardized death rates, period life tables 1933–2024, and January 1 population estimates 1933–2025. Registration required. See also the HMD Methods Protocol v6 and Short-Term Mortality Fluctuations (STMF) series.
- Centers for Disease Control and Prevention, National Center for Health Statistics. CDC WONDER online mortality databases: https://wonder.cdc.gov
- U.S. Census Bureau. 2023 National Population Projections: https://www.census.gov/programs-surveys/popproj.html
- Social Security Administration. Social Security Area Population estimates, 2025 OASDI Trustees Report.
- Internal Revenue Service. Pension plan mortality tables (2024 Adjusted Scale MP-2021 Rates, Pri-2012 base tables): https://www.irs.gov/retirement-plans/pension-plan-mortality-tables

**Actuarial research and standards**

- Society of Actuaries Research Institute, Retirement Plans Experience Committee. *RPEC 2025 Mortality Improvement Update.* October 2025. https://www.soa.org/resources/research-reports/2025/rpec-mort-improvement-update/ (and the 2022, 2023, and 2024 updates in the same series)
- Society of Actuaries. *Mortality Improvement Scale MP-2021.* October 2021. https://www.soa.org/resources/experience-studies/2021/mortality-improvement-scale-mp-2021/
- Society of Actuaries. *The Mortality Improvement Model, MIM-2021-v4b.* October 2024. https://www.soa.org/resources/research-reports/2023/mortality-improvement-model/
- Society of Actuaries. *Pri-2012 Private Retirement Plans Mortality Tables Report.* 2019.
- Society of Actuaries. *Pub-2010 Public Retirement Plans Mortality Tables Report.* 2019.
- Continuous Mortality Investigation (Institute and Faculty of Actuaries). *Working Paper 201: CMI Mortality Projections Model, CMI_2024.* June 2025.
- Canadian Institute of Actuaries. *Mortality Improvements Research: Report to the Canadian Institute of Actuaries' Project Oversight Group.* April 2024. https://www.cia-ica.ca/publications/224043e/
- Actuarial Standards Board. ASOP No. 23 (Data Quality), No. 25 (Credibility Procedures), No. 35 (Selection of Demographic and Other Noneconomic Assumptions), No. 41 (Actuarial Communications). http://www.actuarialstandardsboard.org

**Mortality and demography literature**

- Xu J, Murphy SL, Kochanek KD, Arias E. *Mortality in the United States, 2024.* NCHS Data Brief No. 548. January 2026. https://www.cdc.gov/nchs/products/databriefs/db548.htm
- Murphy SL, Kochanek KD, Xu J, Arias E. *Mortality in the United States, 2023.* NCHS Data Brief No. 521. December 2024.
- Arias E, et al. *United States Life Tables by Hispanic Origin and Race.* National Vital Statistics Reports Vol. 72 No. 12 (Nov. 2023) and Vol. 74 No. 6 (July 2025). https://www.cdc.gov/nchs/data/nvsr/nvsr74/nvsr74-06.pdf
- NCHS. *Mortality Profile of the Non-Hispanic American Indian or Alaska Native Population, 2019.* National Vital Statistics Reports, November 2021 (race misclassification).
- NCHS press release, *Life Expectancy in the U.S. Dropped for the Second Year in a Row in 2021.* August 31, 2022. https://www.cdc.gov/nchs/pressroom/releases/20220831.html
- KFF. *Racial Disparities in Life Expectancy* and *Key Data on Health and Health Care by Race and Ethnicity.* Updated 2025–2026. https://www.kff.org/racial-equity-and-health-policy/racial-disparities-in-life-expectancy/
- *Life Expectancy Changes During the COVID-19 Pandemic, 2019–2021: Highly Racialized Deaths in Young and Middle Adulthood in the United States as Compared With Other High-Income Countries.* American Journal of Public Health / PMC10773482. https://pmc.ncbi.nlm.nih.gov/articles/PMC10773482/
- Andrasfay T, Goldman N. *Reductions in 2020 US life expectancy due to COVID-19 and the disproportionate impact on the Black and Latino populations.* PNAS 118(5), 2021. (Foundational early quantification of differential impact.)
- Administration for Community Living. *2023 Profile of Older Americans.* https://acl.gov

**Regulatory and practitioner commentary**

- Internal Revenue Service. T.D. 9983, *Mortality Tables for Determining Present Value Under Defined Benefit Pension Plans.* 88 Fed. Reg. (October 20, 2023).
- IRS Notice 2024-42, *Updated Static Mortality Tables for Defined Benefit Pension Plans for 2025.* https://www.irs.gov/pub/irs-drop/n-24-42.pdf
- SECURE 2.0 Act of 2022, Division T of the Consolidated Appropriations Act, 2023, Pub. L. 117-328 (0.78% improvement cap).
- Groom Law Group, *Final Regulations Update Pension Plan Mortality Tables and Proposed Regulations Address COVID Impact on Substitute Tables.* October 2023.
- Mercer, *IRS issues eagerly awaited 2024 defined benefit mortality tables.* 2023.

---

## Appendix A — Reproducible Analyses Using HMD U.S. Data

The following exercises can be run directly from the HMD U.S.A. files (free registration required at mortality.org). File names refer to the links on the U.S.A. country page.

**A.1 Replicate the life-expectancy path.**
Download `E0per.txt` (life expectancy at birth, 1×1, both sexes and by sex, 1933–2024). Plot 2010–2024; confirm the 2019→2021 decline and the 2022–2024 recovery. Compare the magnitude to 1918 and to 1921–1923 for historical context.

**A.2 Age-specific rate ratios versus 2019.**
Download `Mx_1x1.txt` (age-specific death rates by single year of age and calendar year, by sex). Compute, for each single age *x* and each year *t* ∈ {2020, …, 2024}, the ratio m(x,t) / m(x,2019). Plot as a heat map or as a family of curves by year. Expected result: a large hump at ages 50–85 in 2020–2021, collapsing by 2023–2024, with a persistent bulge at ages 35–50 for males. This reproduces, from raw data, the pattern RPEC reports in its Tables 2 and 3.

**A.3 Age-standardized excess mortality, pension ages.**
Using `Deaths_1x1.txt` and `Exposures_1x1.txt`, compute age-standardized death rates for ages 65+ using 2019 exposures as weights (the same standardization RPEC uses; see RPEC 2025 Appendix §6.3):

ASDR(t) = Σₓ [D(x,t) / E(x,t)] · E(x,2019) ÷ Σₓ E(x,2019), for x = 65 … 110+

Then compute ASDR(t) / ASDR(2019). This is directly comparable to RPEC's "without mortality improvement" (dashed red) series. To reproduce the "with MP-2021" series, multiply the 2019 base rates by cumulative MP-2021 improvement factors (downloadable as an Excel file from the SOA MP-2021 page) before taking the ratio.

**A.4 Cohort vs. period life expectancy at 65.**
Download `bltper_1x1.txt` (or `mltper_1x1.txt` / `fltper_1x1.txt`) and extract e(65) by year. Then construct a generational (cohort) life expectancy at 65 using the 2019 period table projected with MP-2021, with and without a 1.3% load, and with and without a decaying overlay. The difference in cohort e(65) across these treatments is a direct, communicable measure of what the COVID assumption choice is worth — typically a few tenths of a year, versus the ~2-year swing in *period* life expectancy that dominated the headlines.

**A.5 Compositional sensitivity (requires CDC WONDER, not HMD).**
HMD does not stratify by race or ethnicity. To examine composition effects, pull deaths and population by single-year age, sex, and race/Hispanic origin from CDC WONDER, construct group-specific ASDRs, and then compute a counterfactual national ASDR holding the 2019 racial/ethnic composition fixed. The gap between the actual and counterfactual series quantifies how much of the aggregate change is compositional rather than rate-driven — the effect described in Section 6.2. Note the AIAN misclassification issue (Section 6.1) when interpreting results.

**A.6 Volatility recalibration.**
Fit a Lee–Carter model to U.S. `Mx_1x1.txt` for 1950–2019 and extract the estimated volatility of the time index κ(t). Then compute where the realized 2020 and 2021 values of κ fall in that fitted distribution. The result — typically many standard deviations out — is a compact demonstration of the Section 7.7 point that pre-pandemic calibrations understate tail risk, and a useful exhibit for a board discussion.

---

## Appendix B — Key Numbers at a Glance

| Quantity | Value | Source |
|----------|-------|--------|
| U.S. e₀, 2019 → 2021 | 78.8 → 76.4 years | NCHS |
| U.S. e₀, 2024 (record high) | 79.0 years | NCHS Data Brief 548 |
| U.S. e(65), 2024 | 19.7 years | NCHS Data Brief 548 |
| Peak 65+ excess mortality vs. 2019+MP-2021 | ~16.7% (2020) | SOA RPEC 2025 |
| 65+ excess, 12 months to June 2025 | 1.3% (M 0.5% / F 2.1%) | SOA RPEC 2025 |
| Same, measured against a 2012 base year | 2.0% (M 1.6% / F 2.5%) | SOA RPEC 2025, Table 4 |
| Male 35–44 mortality vs. 2019, 12 months to June 2025 | 106.8% | SOA RPEC 2025, Table 2 |
| e₀ decline 2019–2021, AIAN / Hispanic / Black / White | −6.6 / −4.2 / −4.0 / −2.4 years | KFF; NCHS |
| Black–White e₀ gap, 2019 → 2020 | 4.0 → 5.9 years | NCHS NVSR 72-12 |
| SECURE 2.0 cap on assumed annual improvement (§430) | 0.78% | Pub. L. 117-328 |
| Expected timing of next traditional MP scale | possibly fall 2029 | SOA RPEC 2025, §2 |

---

*End of report.*
