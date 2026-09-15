---
schema: journal-v2
slug: regional-markets-north-america-rankings
title: "The 400 Highest-Scoring Regional Commercial Centers in North America"
subtitle: "Country distribution, tier composition, and the top-ranked markets from the current qualifying pool"
site: gis.woodfinegroup.com
imprint: WCP-2026-11
thesis: "Applying the composition-first qualification gate described in the companion methodology paper to North America currently identifies 1,121 qualifying regional commercial centers; this paper publishes the 400 highest-scoring of them, by country and individually ranked, as the working data behind the map."
abstract: |
  This paper is the North American ranking companion to the regional-markets methodology
  paper: a published, dated snapshot of the 400 highest-scoring regional commercial centers
  currently qualifying under the composition-first gate, out of 1,121 markets that qualify
  in total. It reports the real country distribution of the published set, the top 15
  markets by score with their real catchment figures, and the tier composition of the
  qualifying pool. It does not re-argue the methodology itself — that is the companion
  paper's job — and it publishes no ranking or count that was not computed directly from
  the underlying data.
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
  - North America
  - retail composition
  - market classification
  - working data
---

## What this is

This paper publishes the North American half of the current Regional Markets ranking: the
400 highest-scoring qualifying markets out of 1,121 that meet the composition-first
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
the qualifying pool itself is larger (1,121) and unranked at its full size on the live map.

## Country distribution

| Country | Published markets | Share of 400 |
|---|---|---|
| United States (US) | 298 | 74.5% |
| Canada (CA) | 56 | 14.0% |
| Mexico (MX) | 46 | 11.5% |

No per-country quota applies anywhere in this methodology. This distribution is the real,
observed result of applying one score-based cutoff across the full North American pool —
not a target.

## Tier composition of the published 400

| Tier | Markets carrying this tier flag |
|---|---|
| Regional Market | 331 |
| Standalone Regional Centre | 86 |
| District Anchor | 58 |

A market may carry more than one tier flag where its composition qualifies it under more
than one rule; the columns are not mutually exclusive and do not sum to 400.

## Top 15 by score

| Rank | Market | Country | Nearest larger metro | Score | Catchment population | Catchment spend |
|---|---|---|---|---|---|---|
| 1 | Culiacán, Sinaloa | MX | Chihuahua, 448 km | 2.60 | 985,863 | $26.7B |
| 2 | Greater Sudbury, ON | CA | Toronto, 338 km | 2.51 | 175,456 | $1.0B |
| 3 | Regina, SK | CA | Winnipeg, 535 km | 2.49 | 274,273 | $1.5B |
| 4 | Lexington-Fayette, KY | US | Cincinnati, 122 km | 2.49 | 639,621 | $4.0B |
| 5 | Missoula, MT | US | Boise, 401 km | 2.31 | 132,540 | $757M |
| 6 | Fredericton | CA | Moncton, 145 km | 2.29 | 132,937 | $757M |
| 7 | Bozeman, MT | US | Boise, 469 km | 2.29 | 112,623 | $752M |
| 8 | Lubbock, TX | US | Fort Worth, 436 km | 2.28 | 328,043 | $2.0B |
| 9 | Tepic | MX | Guadalajara, 185 km | 2.28 | 598,523 | $14.1B |
| 10 | Vaughan, Ontario | CA | Toronto, 21 km | 2.28 | 6,129,331 | $36.3B |
| 11 | Grand Junction, CO | US | Denver, 318 km | 2.27 | 177,167 | $844M |
| 12 | Prescott, AZ | US | Phoenix, 127 km | 2.27 | 191,075 | $1.5B |
| 13 | Yakima, WA | US | Tacoma, 167 km | 2.27 | 210,862 | $1.3B |
| 14 | Saint John | CA | Moncton, 134 km | 2.26 | 130,645 | $795M |
| 15 | Red Deer, AB | CA | Calgary, 136 km | 2.26 | 195,036 | $1.1B |

Catchment population and spend are descriptive context only; they do not participate in
scoring or qualification. For a market with more than one member retail cluster, both
figures are computed as a deduplicated union of census/spend cells across all member
clusters, falling back to the strongest single cluster where a full union cannot be
computed. No North American market in the published 400 carries a data gap in either
field.

## Data notes

This snapshot is machine-generated on demand from the live scoring pipeline; it is not
hand-edited and is not a live feed — re-running the underlying pipeline regenerates it as
a new dated pair. Array order in the underlying data is alphabetical by country and name,
not ordinal; no `rank` field is published in the source data itself, only the score this
table ranks by. A small number of market display names carried real formatting defects in
the raw source data — a missing-space concatenation and similar artifacts — corrected here
where found; no market's identity or geography was altered in doing so.

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
estimated or rounded beyond the precision shown.
