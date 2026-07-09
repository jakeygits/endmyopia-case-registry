# EndMyopia Case Report Registry (v2.0)

An open, structured registry of **self-reported adult myopia-reduction case reports**, drawn from first-person accounts published or submitted via endmyopia.org, 2013–2026. v2.0 indexes **363 records** (344-case adult analysis set; 19 excluded as child / post-LASIK / pending).

**Canonical version — cite this:** DOI [10.5281/zenodo.21016339](https://doi.org/10.5281/zenodo.21016339) (concept DOI, always resolves to the latest version).
This GitHub copy mirrors that deposit; the Zenodo DOI is the citable record of reference.

- Registry page: https://endmyopia.org/myopia-improvement-registry/
- Zenodo record (v2.0): https://zenodo.org/records/21270702
- License: Creative Commons Attribution 4.0 (CC BY 4.0)

## What this is

A transparent, auditable index of individual adult cases reporting reduction in myopia (nearsightedness), each graded by how well it is corroborated. It documents people who reported their own results, most of them working from the free method self-directed rather than the guided program. It deliberately excludes the much larger BackTo20/20 program-participant dataset, which is held separately. It exists so the individual-level data can be examined on its merits.

**What it is not:** a clinical trial, and not a population success rate. The cohort is self-selected and predominantly self-reported. It cannot establish how often the approach works; it documents that individual, measured reductions are on record, with the limitations stated up front.

## Summary figures (adult analysis set, n = 344)

- Median starting myopia: **−5.00 D** (range −0.75 to −13.75; n = 282)
- Median recorded reduction: **−1.75 D** (n = 257; maximum −12.75)
- Externally corroborated (third-party exam or official record): **58 / 344 (17%)** in the analysis set; **61** across all 363 documented cases
- Reduction rate, cases with a ≥ 12-month window: **median 1.25 D/yr** (IQR 0.63–1.99; n = 84)

## Verification classes (adult analysis set)

| class | n |
|---|---|
| official record (e.g. driving-license vision record) | 12 |
| third-party exam reported | 46 |
| dated self-measurement | 95 |
| published report, no numbers | 51 |
| numbers, method unclear | 140 |

## Files

- `em-case-registry-v2.0.csv` — the current registry (363 rows; `excluded = true` flags the 19 non-analysis rows)
- `em-case-registry-v2.0.json` — same data plus metadata
- `em-case-registry-v1.0.csv` / `.json` — the prior version, retained for history

## Data dictionary

| column | meaning |
|---|---|
| `case_id` | stable case identifier (EM-####) |
| `verification_class` | strength of corroboration (see table above) |
| `start_numbers` / `end_numbers` | refraction as stated in the source report |
| `start_dpt` / `end_dpt` | starting / latest myopia magnitude, diopters (worse-eye sphere) |
| `delta_dpt` | recorded reduction, diopters |
| `timeline_months` | reported time window |
| `timeline_basis` | how the window was derived |
| `rate_d_yr_12mo_plus` | annualized rate, populated only for ≥ 12-month windows |
| `member_status` | reporter's relationship to the program |
| `first_post` / `last_post` | dates of the source post(s) |
| `n_posts` | number of source posts consolidated into the case |
| `excluded` / `exclusion_reason` | analysis-exclusion flag + reason (child case / post-LASIK / pending verification) |
| `source_posts` | link(s) to the original published report(s) |

## Privacy

All cases derive from reports the participants published or submitted. Direct given-name identifiers have been removed from this distribution; individuals may remain inferable from the cited source posts, which are retained for verification. Removal requests: jake@endmyopia.org.

## Background

The eye regulates its own axial growth in response to optical defocus, and clinical myopia-control research shows that growth can be slowed in children. Sustained reversal of established adult myopia is not established in the controlled literature, but a flat "impossible" overstates what that literature supports. This registry organizes the otherwise scattered individual reports into one auditable resource, with the numbers and the limitations both on the table.
