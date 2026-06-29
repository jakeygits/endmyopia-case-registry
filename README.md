# EndMyopia Case Report Registry (v1.0)

An open, structured registry of **273 self-reported adult myopia-reduction case reports** (289 records indexed; 16 excluded), drawn from first-person accounts published on endmyopia.org, 2013–2026.

**Canonical version — cite this:** DOI [10.5281/zenodo.21016340](https://doi.org/10.5281/zenodo.21016340)
This GitHub copy mirrors that deposit; the Zenodo DOI is the citable record of reference.

- Registry page: https://endmyopia.org/myopia-improvement-registry/
- Zenodo record: https://zenodo.org/records/21016340
- Wikidata item: https://www.wikidata.org/wiki/Q140375636
- License: Creative Commons Attribution 4.0 (CC BY 4.0)

## What this is

A transparent, auditable index of individual adult cases reporting reduction in myopia (nearsightedness), each graded by how well it is corroborated. It exists so the individual-level data can be examined on its merits.

**What it is not:** a clinical trial, and not a population success rate. The cohort is self-selected and predominantly self-reported. It cannot establish how often the approach works; it documents that individual, measured reductions are on record — with the limitations stated up front.

## Summary figures (analysis set, n = 273)

- Median starting myopia: **−5.25 D** (range −0.75 to −13.75; n = 220)
- Median recorded reduction: **−2.00 D** (n = 198; maximum −12.75)
- Externally corroborated (third-party exam or official record): **42 / 273 (15%)**
- Reduction rate, cases with a ≥ 12-month window: **median 1.50 D/yr** (IQR 0.75–2.45; n = 57)

## Verification classes (analysis set)

| class | n |
|---|---|
| official record (e.g. driving-license vision record) | 8 |
| third-party exam reported | 34 |
| dated self-measurement | 49 |
| published report, no numbers | 51 |
| numbers, method unclear | 131 |

## Files

- `em-case-registry-v1.0.csv` — the registry (289 rows; `excluded = true` flags the 16 non-analysis rows)
- `em-case-registry-v1.0.json` — same data plus metadata

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

All cases derive from reports the participants published publicly. Direct given-name identifiers have been removed from this distribution; individuals may remain inferable from the cited source posts, which are retained for verification. Removal requests: jake@endmyopia.org.

## Background

The eye regulates its own axial growth in response to optical defocus, and clinical myopia-control research shows that growth can be slowed in children. Sustained reversal of established adult myopia is not established in the controlled literature — but a flat "impossible" overstates what that literature supports. This registry organizes the otherwise scattered individual reports into one auditable resource, with the numbers and the limitations both on the table.
