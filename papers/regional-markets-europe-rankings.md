---
schema: journal-v2
slug: regional-markets-europe-rankings
title: "The 400 Highest-Scoring Regional Commercial Centers in Europe"
subtitle: "Country distribution, tier composition, and the top-ranked markets from the current qualifying pool"
site: gis.woodfinegroup.com
imprint: WCP-2026-12
thesis: "Applying the composition-first qualification gate described in the companion methodology paper to Europe currently identifies 650 qualifying regional commercial centers; this paper publishes the 400 highest-scoring of them, by country and individually ranked, as the working data behind the map."
abstract: |
  This paper is the European ranking companion to the regional-markets methodology paper:
  a published, dated snapshot of the 400 highest-scoring regional commercial centers
  currently qualifying under the composition-first gate, out of 650 markets that qualify in
  total across 15 countries. It reports the real country distribution of the published set,
  the top 15 markets by score with their real catchment figures where available, and the
  tier composition of the qualifying pool. Coverage is genuinely uneven across countries —
  a real, disclosed feature of where the underlying retail-composition data is currently
  strongest, not an artifact of the methodology's own construction.
state: draft
version: "1.0.0"
published:
updated: "2026-09-15"
doi:
license: CC-BY-4.0
cites: []
draws_from:
  - commuter
  - urban-fringe
contributors:
  - name: Peter M. Woodfine
    roles: [Contributor]
  - name: Jennifer M. Woodfine
    roles: [Contributor]
  - name: Mathew Woodfine
    roles: [Contributor]
keywords:
  - regional market ranking
  - Europe
  - retail composition
  - market classification
  - working data
---

## What this is

This paper publishes the European half of the current Regional Markets ranking: the 400
highest-scoring qualifying markets out of 650 that meet the composition-first
qualification gate described in the companion methodology paper. It is a dated
data snapshot, not a narrative argument — the methodology, the three-tier qualification
gate, and the reasoning behind ranking only within an already-qualified pool are the
companion paper's subject, not restated here beyond what is needed to read the tables.

A market qualifies under one of three composition rules — Regional Market, District
Anchor, or Standalone Regional Centre — based on which anchor-store formats are physically
present and how they are geographically distributed, never by a fixed count and never by
population or spend. Once a market qualifies, its published rank is a composition- and
isolation-weighted score; that score decides ranking only, never qualification. This
publication reflects the 400 highest-scoring qualifying markets as of the data below —
the qualifying pool itself is larger (650) and unranked at its full size on the live map.

## Country distribution

| Country | Published markets | Share of 400 |
|---|---|---|
| Italy (IT) | 62 | 15.5% |
| Spain (ES) | 55 | 13.8% |
| Great Britain (GB) | 55 | 13.8% |
| Poland (PL) | 55 | 13.8% |
| Sweden (SE) | 32 | 8.0% |
| Czechia (CZ) | 27 | 6.8% |
| Finland (FI) | 19 | 4.8% |
| Hungary (HU) | 19 | 4.8% |
| Slovakia (SK) | 16 | 4.0% |
| Romania (RO) | 13 | 3.2% |
| Bulgaria (BG) | 11 | 2.8% |
| Denmark (DK) | 11 | 2.8% |
| Croatia (HR) | 9 | 2.2% |
| Norway (NO) | 9 | 2.2% |
| Greece (GR) | 7 | 1.8% |

No per-country quota applies anywhere in this methodology. This distribution is the real,
observed result of applying one score-based cutoff across the full European pool, and it
is genuinely uneven — a market's country does not affect whether or how strongly it
qualifies, so a country with sparser current retail-composition data will always be
under-represented relative to one with denser data, independent of retail reality on the
ground.

## Tier composition of the published 400

| Tier | Markets carrying this tier flag |
|---|---|
| Regional Market | 332 |
| Standalone Regional Centre | 73 |
| District Anchor | 28 |

A market may carry more than one tier flag where its composition qualifies it under more
than one rule; the columns are not mutually exclusive and do not sum to 400.

## Top 15 by score

| Rank | Market | Country | Nearest larger metro | Score | Catchment population | Catchment spend |
|---|---|---|---|---|---|---|
| 1 | Jönköping | SE | Gothenburg, 132 km | 2.13 | — | — |
| 2 | Karlstad | SE | Oslo, 165 km | 2.11 | — | — |
| 3 | San Giovanni Teatino | IT | Ancona, 122 km | 1.94 | 672,391 | see note |
| 4 | Thurrock | GB | London, 29 km | 1.94 | 9,241,683 | $42.6B |
| 5 | Gävle | SE | Stockholm, 156 km | 1.86 | — | — |
| 6 | Milton Keynes | GB | Luton, 27 km | 1.77 | 2,132,313 | $11.1B |
| 7 | Girona | ES | Barcelona, 84 km | 1.73 | 847,038 | see note |
| 8 | Padova | IT | Venice, 32 km | 1.72 | 2,165,363 | see note |
| 9 | Gorzów Wielkopolski | PL | Szczecin, 88 km | 1.72 | 348,178 | $3.9B |
| 10 | Helsingborg | SE | Copenhagen, 48 km | 1.67 | — | — |
| 11 | Słupsk | PL | Gdańsk, 107 km | 1.66 | 258,251 | $2.9B |
| 12 | Umeå | SE | Oulu, 279 km | 1.66 | — | — |
| 13 | Sassari | IT | Toulon, 343 km | 1.66 | 298,739 | see note |
| 14 | Ciudad Real | ES | Toledo, 98 km | 1.66 | 243,483 | see note |
| 15 | Malmö | SE | Copenhagen, 30 km | 1.66 | — | — |

Catchment population and spend are descriptive context only; they do not participate in
scoring or qualification. For a market with more than one member retail cluster, both
figures are computed as a deduplicated union of census/spend cells across all member
clusters, falling back to the strongest single cluster where a full union cannot be
computed.

## Data notes — real, disclosed gaps

**No catchment population or spend data is available for Swedish markets** (and, more
broadly, for Bulgaria, Finland, Croatia, Norway, and Romania) — shown as "—" in the tables
above. This is a real gap in the underlying census and spend source data for those
countries, not an error in ranking or an omission in this publication; it does not affect
scoring or qualification, which never use these fields.

**A second, distinct data-quality observation, not previously disclosed**: several Italian
and Spanish markets in the top 15 (marked "see note" above) carry a `catchment_spend`
value of exactly zero rather than a missing-data marker — flagged here as more likely an
incomplete-ingestion artifact than a genuine zero-retail-spend market, given each has a
real, substantial catchment population. This is reported honestly as an open data-quality
question for the underlying pipeline, not resolved or estimated in this paper.

This snapshot is machine-generated on demand from the live scoring pipeline; it is not
hand-edited and is not a live feed — re-running the underlying pipeline regenerates it as
a new dated pair. Array order in the underlying data is alphabetical by country and name,
not ordinal; no `rank` field is published in the source data itself, only the score this
table ranks by. One market display name in the top 15 carried a real formatting defect in
the raw source data — a missing-space concatenation — corrected here; no market's identity
or geography was altered in doing so.

## Contributors

Peter M. Woodfine, Jennifer M. Woodfine, and Mathew Woodfine are credited as contributors
to Woodfine Management Corp.'s geospatial research programme.

## How this paper was produced

This paper was prepared with AI assistance under human editorial direction; all analytical
claims and conclusions are the responsibility of the named institutional author.

## Disclosures

The ranking data described is this workspace's own engineering work, generated directly
from the live scoring pipeline. This paper makes no forward-looking claim about future
market coverage or ranking changes.

## Data and reproducibility

The underlying data is machine-generated by a dated scoring-and-selection pipeline run on
demand; every figure in this paper's tables is drawn directly from that output, not
estimated or rounded beyond the precision shown, with the two disclosed data-quality gaps
noted directly above the relevant tables rather than silently corrected or hidden.
