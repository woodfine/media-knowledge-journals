---
schema: journal-v2
slug: regional-markets
title: "Classifying Regional Commercial Centers by What They Actually Contain"
subtitle: "A composition-first replacement for an exact-count ranking that let isolation outrank real retail substance"
site: gis.woodfinegroup.com
imprint: WCP-2026-10
thesis: "Ranking commercial markets by an isolation-weighted score and cutting the list at a round number produces a list that looks authoritative but is not compositionally coherent — replacing the exact-count cutoff with a composition-first qualification gate, and using isolation only to rank markets that already qualify, produces a classification that says what it actually measures and admits no market by exception."
abstract: |
  An earlier version of this classification ranked commercial markets primarily by
  geographic isolation from other retail nodes, then published a fixed-count list cut at a
  round number. A full review found that formula let isolation dominate real retail
  substance: a meaningful share of published markets had only marginal retail composition,
  while hundreds of markets with genuinely stronger anchor-store composition were left off
  the list simply because they scored lower on isolation. The same version also tied its
  published count to an internal capital-deployment planning figure that should never have
  been derivable from public output — a disclosure defect independent of the ranking-quality
  problem, and one we treat as a closed, corrected incident rather than a live risk. We
  describe the replacement: a market qualifies as a genuine regional commercial center under
  one of three composition rules, based only on which anchor store formats are actually
  present and how they are geographically distributed — never by a fixed count, and never
  by any financial or population figure. Isolation, category breadth, and civic presence
  are used only to rank markets that have already qualified; they never decide whether a
  market qualifies at all. Applying this methodology today identifies substantially more
  qualifying commercial centers in North America than in Europe — a real, disclosed
  difference in market structure between the two continents, not an artifact of the
  methodology's own construction. This paper describes the methodology, its real current
  output, and states directly what a qualifying classification does and does not mean.
state: draft
version: "1.0.0"
published:
updated: "2026-09-15"
doi:
license: CC-BY-4.0
cites: []
draws_from:
  - aec-data-layers
  - commuter-urban-fringe
  - geometric-site-selection-national-tenancy
contributors:
  - name: Peter M. Woodfine
    roles: [Founding Contributor]
  - name: Jennifer M. Woodfine
    roles: [Founding Contributor]
  - name: Mathew Woodfine
    roles: [Founding Contributor]
keywords:
  - regional market classification
  - retail composition
  - geographic isolation
  - co-location geography
  - market structure
---

## 1. The question

Classifying which commercial locations function as genuine regional commercial centers — as
distinct from a suburb whose retail catchment merely overlaps a nearby larger city — is a
scale problem before it is anything else: there are far more candidate locations across a
large geography than any manual survey could evaluate consistently. A mechanically applied
classification rule can solve the scale problem, but only if the rule itself measures the
right thing. An earlier version of this classification measured the wrong thing first and
foremost: it ranked candidate markets primarily by geographic isolation from other retail
nodes — how far a market sits from its nearest peer — and then published a list cut at a
fixed, round number of entries.

A full review of that earlier version found two independent, serious problems, not one. The
ranking itself was compositionally incoherent: because isolation could dominate the score,
markets with only marginal retail substance — sometimes a single weak commercial cluster and
nothing else — could outscore markets with genuinely stronger, more diverse anchor-store
composition simply by being farther from any other node. And separately, the mechanism used
to size the published list was tied, indirectly but derivably, to an internal capital-
deployment planning figure that should never have been reconstructable from public output at
all — several groups landed at values close enough to that internal figure's own multiples to
make the connection recoverable. We treat this second problem as a closed, corrected
disclosure incident, not a live risk — it is stated here because the redesign that followed
directly addresses both problems together, not because the original figures are being
restated. This paper describes the question the redesign answers: what should actually
qualify a location as a genuine regional commercial center, using only what can be observed
about its retail composition and geography — never a count, and never a financial figure?

## 2. What we found

**Separating qualification from ranking — deciding whether a market counts as a genuine
regional commercial center using only its retail composition, and using isolation and other
factors only to order markets that already qualify — produces a classification that is
compositionally coherent by construction.** A market qualifies as the strongest classification
when it combines a full grocery/general-merchandise anchor with at least two of several
distinct destination-format categories (hardware, price-club, lifestyle, electronics, sport
retail) across its constituent retail clusters. A market qualifies as a second classification
when it has the grocery and hardware anchors present with genuine multi-site depth — at least
two real, distinct retail clusters, not one padded cluster counted twice — but lacks the
broader destination-format mix. A third classification applies the identical composition test
to markets that are otherwise geographically isolated from any other qualifying market beyond
a defined outer distance band. A market meeting none of these three tests does not appear in
the classification at all — there is no fourth tier, no exception, and no manual override.

**Removing the exact-count cutoff entirely, and replacing it with a pure composition gate,
eliminates the specific failure the earlier version had by construction, not by degree.**
Because admission to the classification no longer depends on where a market lands in a
ranked list cut at a round number, there is no mechanism left by which an internal planning
target — or any other number extraneous to retail composition — could shape which markets are
published or how many. The published output for a given continent is now simply every market
that meets one of the three composition tests, in whatever real quantity that turns out to
be.

**Applying the corrected methodology today finds a real, large, and durable difference in
market count between North America and Europe — a disclosed fact about retail-anchor
density, not an artifact of the classification's own construction.** North America currently
has substantially more than a thousand qualifying regional commercial centers under this
methodology; Europe currently has roughly six hundred fifty. Both figures reflect the same
composition test applied identically on both continents — the difference is a real fact about
how anchor-format retail is geographically distributed today, not a result of different rules
being applied to each continent.

**Ranking within a qualifying tier depends on category breadth and cluster depth, distance
from the nearest other qualifying market, and civic presence — with each element scoped to
avoid a specific, previously identified distortion.** Raw store or chain count was tested and
rejected as a ranking signal because it is corrupted by uneven data-collection density across
different retail chains, not by any real difference in a market's retail strength. Isolation
is measured against the nearest other *qualifying* market, not the nearest retail cluster of
any kind — the earlier version's isolation measure rewarded distance from any nearby cluster
regardless of whether that cluster itself was retail-significant, which is not the same
question. Civic presence — hospitals and universities within the market's catchment — is
capped in its contribution, because civic presence alone is close to universal across
candidate markets and carries limited power to distinguish a strong market from a weak one on
its own.

## 3. How we built it

The composition gate evaluates each candidate market against its constituent retail
clusters' anchor-store composition only, using observable facts about which anchor formats
are physically present, never a demographic, financial, or population figure. A market's
retail clusters are checked for the presence of a general-merchandise/grocery anchor, and
then for the presence and diversity of destination-format anchors — hardware, price-club,
lifestyle, electronics, and large-format sporting-goods retail — unioned across every
cluster that belongs to the same market rather than evaluated cluster by cluster in
isolation. A market's geographic classification — whether it sits close enough to an existing
major metropolitan retail node to be excluded as already served, in the intermediate
suburban-regional band, or genuinely standalone beyond the outer distance threshold — is
computed from real geographic distance to the nearest major metro node, independent of the
composition test itself; the two are combined only after each is computed on its own terms.
A market whose constituent clusters span an unreasonably large geographic area is excluded
regardless of its composition or isolation classification, on the grounds that such a case
represents a name collision between geographically distinct clusters rather than one coherent
market.

Once a market clears the composition gate, its rank within its classification tier is
computed as a product of four factors: category breadth and best-single-cluster depth (a
measure we call node strength, deliberately built to avoid the raw-count distortion described
in §2); isolation from the nearest other *qualifying* market; a capped civic-presence bonus;
and a confidence factor reflecting data-completeness for that specific market. None of these
four ranking factors can move a market into or out of qualification — they operate strictly
within a tier a market has already qualified for on composition grounds alone.

A separate, deliberately distinct process derives a curated, per-continent list of a bounded
number of markets for editorial and wiki-content purposes specifically — publishing the
highest-scoring qualifying markets up to a fixed target count per continent, with no
per-country quota beyond a small floor guaranteeing no country with genuinely qualifying
markets is entirely excluded by chance. Where a continent's real qualifying pool is smaller
than that target count, every qualifying market is published, and the shortfall is disclosed
plainly as a real count, not treated as a defect to correct by relaxing the composition gate.
This editorial derivation never feeds back into, or alters, the underlying classification
itself — it is a downstream, bounded selection built for a specific purpose, entirely separate
from the live, uncapped, unranked classification that qualifying-market status itself is based
on.

## 4. What it changes

For anyone using this classification — an internal team scoping site-selection work, or an
external reader trying to understand where genuine regional commercial centers actually
exist — the practical change is that a market's presence in the classification, and its tier
within it, now means exactly one thing: a specific, disclosed, and mechanically verifiable
fact about its retail-anchor composition and geographic isolation. It no longer means the
market happened to clear an isolation-weighted score high enough to make a fixed-size cut,
and it carries no trace, direct or derivable, of any internal financial planning figure.

It also changes what a genuinely coherent regional commercial center count actually looks
like across a large geography. The earlier version's fixed-count design implicitly suggested
comparable market density across regions by publishing similarly-sized lists regardless of
underlying reality; the corrected, uncapped methodology instead discloses the real,
substantially different market counts North America and Europe currently produce under an
identical rule — a more honest, if less tidy, picture of where this kind of retail
infrastructure actually concentrates today.

## 5. Where this could be wrong

**The composition gate reflects a specific, chosen set of anchor-store categories and a
specific set of thresholds for combining them — a different reasonable set of categories or
thresholds could produce a different classification.** We tested several composition-gate
variants before settling on the current one, and disclose that choice directly rather than
presenting the current gate as the only defensible option; the specific threshold for how
many destination formats a market needs, and which formats count, reflects real testing
against live data, not an arbitrary a priori decision, but it remains a judgment call among
several tested alternatives.

**Underlying retail-location data has real, uneven completeness across countries and
categories, and this affects which markets clear the composition gate.** A market whose
retail landscape is genuinely strong but whose underlying source data has gaps in a specific
category can fail to qualify not because it lacks the real-world retail composition, but
because that composition is not yet reflected in the underlying data. We treat this as a
disclosed data-completeness limitation, not a claim that every non-qualifying market
genuinely lacks the retail substance the classification is looking for.

**This classification measures retail-anchor composition and geographic isolation only —
it makes no claim about population, income, market growth, or any economic outcome.**
A market's classification tier or rank within a tier says nothing about its investment merit,
its future trajectory, or any specific financial figure; conflating classification status
with an economic recommendation is a real, avoidable misreading this paper explicitly warns
against.

## 6. Conclusion

An earlier version of this classification let geographic isolation dominate real retail
composition, producing a list that was compositionally incoherent and, separately, carried a
disclosure defect tying its published count to an internal planning figure. The corrected
methodology separates these concerns cleanly: a market qualifies as a genuine regional
commercial center purely on the strength and diversity of its actual retail-anchor
composition, with no exact-count cutoff and no financial figure anywhere in the qualification
logic; isolation, category breadth, and civic presence rank markets that have already
qualified, and never decide qualification itself. Applying the corrected methodology today
finds a real, substantial, and honestly disclosed difference in qualifying market count
between North America and Europe — a fact about retail geography, not an artifact of how the
classification counts.

---

## 7. Claims and what would count against them

**Compositional-coherence claim.** Every market appearing in the classification meets at
least one of the three defined composition gates on its own retail-anchor composition,
independent of any ranking factor; no market qualifies by isolation, ranking score, or count
alone.

**Disclosure-independence claim.** No published field, count, or derived statistic in the
current classification allows an external reader to reconstruct any internal capital-
deployment planning figure.

| Test | What it checks | Status |
|---|---|---|
| Qualification-basis audit | Whether any currently-qualifying market's admission depends on anything other than its own composition-gate result | Verified in the current implementation: composition gate is the sole admission criterion |
| Count-derivability check | Whether the published per-continent counts or any per-group count can be checked against, or used to reconstruct, an internal planning figure | Verified: the current output contains no per-group count field and no exact-count cutoff of any kind |
| Ranking-non-interference check | Whether node strength, isolation, or civic bonus can move a market into or out of qualification | Verified in the current implementation: these factors apply only within an already-qualified tier |
| Data-completeness audit | Whether qualifying and non-qualifying status correlates with underlying data completeness rather than real-world composition, for a sample of markets | Not yet run as a formal audit — a disclosed, known limitation (§5), not a tested and cleared item |

The compositional-coherence claim is falsified if any currently-qualifying market is found to
have qualified through a path other than its own composition-gate result. The disclosure-
independence claim is falsified if any published field or derivable statistic is shown to
allow reconstruction of an internal planning figure.

### Appendix A — Representative current counts

North America: composition gate currently qualifies substantially more than one thousand
regional commercial centers. Europe: the composition gate currently qualifies approximately
six hundred fifty. Both counts reflect the identical composition test applied independently
per continent, with no per-country quota; a curated, bounded editorial selection (for wiki
content purposes) draws a fixed number of the highest-scoring qualifying markets per
continent separately from this live, uncapped classification, publishing every qualifying
market where a continent's real pool is smaller than the selection target.

---

## Contributors

Peter M. Woodfine, Jennifer M. Woodfine, and Mathew Woodfine are credited as founding
contributors to Woodfine's geographic-analysis research programme.

## How this paper was produced

This paper was prepared with AI assistance under human editorial direction; all analytical
claims and conclusions are the responsibility of the named institutional author.

## Disclosures

This paper describes a geographic classification methodology only. It makes no recommendation
regarding, and no claim about the investment merit of, any specific market or property.
Nothing in this paper is an offer to sell, or a solicitation of an offer to buy, any security
or interest in real property. A prior version of the underlying published output carried a
disclosure defect, described in §1 as a closed, corrected incident; this paper does not
restate the internal figures involved.

## Data and reproducibility

The classification methodology is maintained by this workspace's geographic-analysis
programme and is reproducible from the same underlying retail-location source data described
in a companion paper (`aec-data-layers`). The representative counts in Appendix A reflect the
most recent methodology refresh available at the time of writing and are expected to change
as underlying data coverage improves.
