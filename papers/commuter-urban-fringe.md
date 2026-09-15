---
schema: journal-v2
slug: commuter-urban-fringe
title: "Two Non-Retail Commercial Archetypes in the Metropolitan Ring"
subtitle: "Industrial-supply and transit-adjacent clusters, identified the same way as retail co-location"
site: gis.woodfinegroup.com
imprint: WCP-2026-02
thesis: "The same open-data, composition-based method that identifies retail co-location clusters also identifies two structurally different, non-retail commercial patterns — each defined by what is present or absent, not by a retail anchor at all."
abstract: |
  Retail anchor co-location is not the only commercial pattern visible in open map data. This
  paper applies the same composition-based, open-data method described in our companion paper
  on retail co-location to two structurally different commercial archetypes that occupy the
  same metropolitan ring but serve entirely different demand bases. The first, which we call
  the industrial-supply archetype, is a cluster of hardware retail, trades supply, and
  equipment rental with no grocery hypermarket present — a pattern serving contractors, not
  households. Across eighteen countries, roughly one in four hardware retail locations (about
  26%) sits without a nearby grocery anchor, and these locations cluster into a distinct,
  identifiable commercial type. The second, which we call the transit-adjacent archetype, is a
  cluster of car-rental branches near a regional airport or intercity rail station, serving the
  traveller who drives to a transit hub and continues by rail or air. Car-rental presence
  reliably marks this pattern, and it appears at roughly seven times as many rail stations as
  airports in the current dataset, reflecting the greater reach of intercity rail relative to
  regional aviation. Both archetypes are identified from OpenStreetMap data alone, using the
  same distance-and-composition logic as our companion paper, adapted to a different presence
  or absence signal for each. The main limitation, shared by both: the current counts describe
  a snapshot from an earlier pipeline run and are pending a refresh against the live,
  continuously-updated dataset, and one internal parameter in the clustering method could not
  be reconciled with confidence between two source documents describing it differently — we
  say so directly rather than picking a number without a way to check it.
state: draft
version: "1.0.0"
published:
updated: "2026-09-15"
doi:
license: CC-BY-4.0
cites:
  - duranton-puga-2004-agglomeration-microfoundations
  - marshall-1890-principles-of-economics
  - von-thunen-1826-isolated-state
  - hotelling-1929-stability-in-competition
  - cervero-kockelman-1997-travel-demand-3ds
  - calthorpe-1993-next-american-metropolis
  - kasarda-lindsay-2011-aerotropolis
  - haklay-2010-osm-quality
  - cidell-2010-logistics-sprawl-chicago
draws_from: []
contributors:
  - name: Peter M. Woodfine
    roles: [Founding Contributor]
  - name: Jennifer M. Woodfine
    roles: [Founding Contributor]
  - name: Mathew Woodfine
    roles: [Founding Contributor]
keywords:
  - industrial co-location
  - transit-adjacent commercial
  - metropolitan ring
  - open geospatial data
  - spatial clustering
  - agglomeration
---

## 1. The question

Our companion paper describes a method for identifying retail co-location clusters from open
map data alone, using the composition of anchor categories present — not their count — as the
signal that independent, well-resourced retail decisions have converged on a location. That
method depends on one specific structural fact about retail: several different kinds of
large-format retailer, sited close together, is itself informative, because it reveals
something about the strength of a household consumer market.

Not every commercial pattern worth identifying is retail, and not every useful signal is
"which categories are present together." This paper applies the same underlying logic —
identify a real commercial pattern from open data, using composition rather than raw count —
to two patterns that are not retail at all, and that each require a different kind of signal
to detect.

The first pattern serves contractors and light industry, not households: clusters of hardware
retail, trades supply, and equipment rental where no grocery hypermarket is present. We call
this the industrial-supply archetype. Its defining signal is not which categories are present
together, but which category is conspicuously *absent* — the household grocery anchor that
defines a retail cluster. A hardware store with no grocery nearby is not a smaller, weaker
version of a retail cluster; it is evidence of a different demand base entirely, one built
around contractors visiting multiple trade suppliers in a single working trip rather than
households doing weekly shopping.

The second pattern serves travellers, not local shoppers or contractors: clusters of
car-rental branches near a regional airport or intercity rail station, serving the person who
drives from home, parks, and continues onward by train or plane. We call this the
transit-adjacent archetype. Its defining signal is neither composition nor absence, but a
specific, purpose-revealing co-location: car rental — a service that exists almost nowhere
except where someone has just arrived and needs a vehicle, or is about to leave and is
returning one — clustered near a transit anchor.

The question this paper asks is whether both of these genuinely different patterns can be
identified reliably, at the same continental scale as our companion paper's retail analysis,
using the same open-data discipline: no licensed mobility panel, no proprietary leasing
database, just public map data and a stated, checkable rule for what counts as a match.

## 2. What we found

**The industrial-supply archetype is real, common, and clearly distinguishable from retail
co-location.** Across roughly ten thousand hardware retail locations studied in eighteen
countries, about three-quarters sit near a grocery hypermarket — meaning they are, in effect,
already part of a retail cluster of the kind our companion paper describes. The remaining
quarter or so — roughly 26% — have no grocery anchor nearby at all, and it is this remainder
that forms the industrial-supply pattern. Auto-parts retail is by far the strongest companion
signal: it sits near more than half of all hardware locations, retail-anchored or not, which
makes sense once the underlying client base is considered — a contractor's commercial vehicle
needs upkeep on the same trip schedule as the contractor's supply runs. Builders' merchants,
trade-supply distributors, and equipment rental follow at lower but still meaningful rates,
and which of these secondary categories shows up varies by country in ways that track real
differences in how each country's construction trades are supplied, not random noise. The
industrial-supply pattern concentrates most heavily in a ring roughly ten to thirty kilometres
from a major metropolitan centre — inside dense urban cores, land is too valuable for
large-footprint trade-supply retail; well beyond the ring, there isn't enough contractor
traffic to sustain the cluster at all.

**The transit-adjacent archetype is also real and clearly distinguishable, but by a different
kind of test entirely.** Car-rental branches cluster reliably near regional transit anchors —
airports and intercity rail stations — that sit a meaningful distance from a major
metropolitan core, and excluding the handful of major hub airports that already have their own
large retail complex built directly into the terminal. Of the transit-adjacent clusters
identified, the large majority sit near intercity rail stations rather than airports — on the
order of seven rail-adjacent clusters for every one airport-adjacent cluster — which reflects
a real, structural difference between the two transit modes: intercity rail networks,
particularly in Europe, reach far more sub-metropolitan places than regional air service does.
A meaningful minority of transit-adjacent clusters — roughly a quarter, and noticeably higher
for airports than for rail stations — sit close enough to an existing retail cluster
(identified the same way as in our companion paper) to be considered integrated with it,
suggesting that some transit hubs anchor genuinely complete sub-metropolitan commercial
markets while most stand somewhat apart from one.

**The two archetypes occupy overlapping distance bands, and we want to be explicit about
that rather than let it cause confusion later.** The industrial-supply archetype is defined
within roughly five to eighty kilometres of a metropolitan core; the transit-adjacent
archetype, within roughly fifteen to one hundred fifty kilometres. These bands overlap between
roughly fifteen and eighty kilometres — meaning a single location could, in principle, qualify
for both archetypes at once, if it happened to have both a hardware store without a grocery
anchor and a nearby transit hub with car rental. This is not a flaw in either definition; the
two archetypes are identified by completely independent signals (grocery absence for one, a
transit anchor with car rental for the other) and there is no reason a place could not
genuinely exhibit both patterns. What matters is that this overlap is stated plainly here, so
that neither archetype's distance band gets casually borrowed to describe the other one, or
folded into a third, undefined "sub-metropolitan ring" figure that belongs to neither — a
conflation that has already happened once, in an unrelated wiki article describing a different
system, and which we are flagging here specifically so it does not happen again in this
paper's own record.

## 3. How we identified each archetype

Both archetypes are identified using the same two ingredients as our companion paper: a
two-pass, distance-based clustering method run on OpenStreetMap point data, and a stated
composition rule that determines which clusters qualify. What differs between the two
archetypes, and between each of them and the retail-cluster method, is the specific rule.

**Industrial-supply.** A cluster qualifies if a hardware retail anchor is present, if no
grocery hypermarket anchor is present anywhere in the same cluster, and if the cluster sits
within roughly five to eighty kilometres of a major metropolitan centre. Clusters are then
ranked by how many additional trade-supply categories — auto parts, builders' merchants,
trade-tool and MRO distributors, equipment rental — accompany the hardware anchor, with more
categories present indicating a richer, more complete industrial-supply node rather than a
single isolated hardware store. We want to note directly, rather than paper over, that the
exact minimum-cluster-size parameter used in the underlying distance-clustering step is stated
differently across two source documents describing this pipeline — one says the tight-pass
minimum is a single point, another says three — and we were not able to reconcile which is
correct without access to the live pipeline configuration. We are stating this discrepancy
plainly rather than picking one number and presenting it as settled; it does not affect the
qualifying logic described above, but it should be confirmed against the live system before
this figure is cited as precise.

**Transit-adjacent.** A cluster qualifies if a regional airport or intercity rail station is
present, if at least one car-rental branch sits within a short distance of that transit
anchor, and if the transit anchor itself sits within roughly fifteen to one hundred fifty
kilometres of a major metropolitan centre — excluding the small number of major hub airports
that already have a large, purpose-built retail complex directly on site, since those exhibit
a fundamentally different commercial pattern from the park-and-travel behaviour this archetype
is meant to capture. A transit-adjacent cluster is considered integrated with the broader
commercial market if an existing retail-co-location cluster (identified per our companion
paper's method) sits within a further short distance of the transit anchor.

Both methods share the same underlying design principle as our companion paper: hold the
geometric thresholds constant across every country studied, rather than tuning them per
country to hit a target count, and let the resulting distribution — however lopsided between
countries or between rail and air — describe something real about how each country's
commercial and transit geography actually developed, rather than something engineered to look
tidy.

## 4. What it changes

For a developer or planner evaluating a metropolitan ring, the practical change these two
archetypes make is the same kind of change our companion paper makes for retail: identifying
a real, open-data-visible commercial pattern before it shows up in demand data, rather than
after. A market with a strong industrial-supply cluster and no retail cluster nearby is not an
underdeveloped retail market — it may be a genuinely different kind of commercial node,
serving contractors rather than households, and evaluating it against retail-market
assumptions would be a category error. Similarly, a transit hub with a strong car-rental
cluster but no nearby retail cluster is a real, if incomplete, sub-metropolitan commercial
node — one where transit demand exists but the surrounding retail market has not yet developed
to match it, which is itself a useful, actionable finding distinct from either "no market
here" or "already a complete market."

For our companion paper's own framework, the practical change is a caution rather than an
extension: not every commercial signal worth measuring is a retail-composition signal. The
industrial-supply archetype is identified by absence, the transit-adjacent archetype by a
purpose-revealing service category, and neither would be visible under the retail-composition
rule alone. A screening process that only looked for retail anchor co-location would miss both
real patterns entirely — not because they are rare, but because they are structurally
different kinds of pattern, requiring a different question asked of the same underlying open
data.

## 5. Where this could be wrong

**The published counts in this paper are a snapshot, not a live figure.** Both archetypes'
counts come from an earlier pipeline run, predate a later rebuild of the underlying retail
clustering system that this paper's companion paper already flags as materially changing
retail cluster counts, and have not been independently re-verified against the current live
dataset. Directional findings (rail dominates over air; roughly a quarter of hardware
locations sit without a grocery anchor) are likely to hold; the precise counts should be
treated as approximate pending a refresh.

**One clustering parameter is genuinely unresolved, not just unreported.** As noted in §3, the
industrial-supply archetype's minimum-cluster-size parameter is stated inconsistently across
two source documents. We chose to disclose this rather than silently pick a value, because
silently picking one would misrepresent a real, currently-unresolved fact as a settled one.

**Neither archetype's causal claim has been tested.** Like our companion paper, both
archetypes here describe a real, structural, open-data-visible pattern. Neither this paper nor
its predecessor has yet shown that either pattern predicts measured commercial activity — that
test, for both archetypes, awaits the same kind of employment and mobility data our companion
paper's falsification programme depends on.

**Map-data coverage is uneven across both archetypes, in the same way and for the same
reasons described in our companion paper** — coverage of both hardware chains and intercity
transit operators varies by country and by local mapping community activity, which likely
understates rather than overstates both archetypes' true prevalence in less-covered markets.

## 6. Conclusion

The question was whether the same open-data, composition-based approach that identifies
retail co-location clusters also identifies real, non-retail commercial patterns in the same
metropolitan ring. It does, for two structurally different patterns that each require their
own signal: industrial-supply clusters, identified by the deliberate *absence* of a household
grocery anchor alongside a hardware retail anchor, and transit-adjacent clusters, identified by
the presence of car rental near a regional transit hub. Both are real, both are currently
measurable from open map data alone, and both occupy an overlapping stretch of the
metropolitan ring without being the same thing — a distinction this paper has tried to state
plainly enough that it does not get lost or conflated in later work that draws on it.

---

## 7. Claims and falsification

**H1 (industrial-supply).** Clusters identified by the hardware-present/grocery-absent rule
show a systematically higher ratio of trade-supply-category presence to grocery presence than
retail co-location clusters at matched metropolitan distance.

**H2 (transit-adjacent).** Car-rental presence is significantly more common near qualifying
transit anchors than at matched non-transit locations at equivalent metropolitan distance and
population density.

| Test | What it checks | Status |
|---|---|---|
| Trade-supply-to-grocery ratio test | H1: industrial-supply clusters differ compositionally from retail clusters at matched distance | Executable now against current data; not yet re-run against the refreshed pipeline |
| Car-rental concentration test | H2: car-rental presence is elevated at transit anchors versus matched non-transit control points | Executable now; not yet re-run against the refreshed pipeline |
| Industrial land-use validation | Do industrial-supply cluster centroids sit closer to independently-tagged industrial land than retail cluster centroids? | Designed; treated as confirmatory if positive, inconclusive (not falsifying) if negative, given known gaps in the underlying land-use tagging |
| Passenger-volume validation | Do transit-adjacent clusters correlate with actual station/airport passenger volume, for the subset of countries with public ridership data? | Designed; requires matching station records across data sources, not yet executed |

H1 is falsified if the trade-supply-to-grocery ratio does not differ meaningfully between
industrial-supply and retail clusters once metropolitan distance is controlled for. H2 is
falsified if car-rental presence does not differ meaningfully between transit anchors and
matched non-transit control points.

### Appendix A — Method notation

| Term | Definition |
|---|---|
| Industrial-supply cluster | Hardware retail anchor present, grocery hypermarket anchor absent, within the qualifying metropolitan-distance band |
| Transit-adjacent cluster | Car-rental branch present near a qualifying regional airport or intercity rail station |
| Integrated (transit-adjacent) | A qualifying transit-adjacent cluster with a retail co-location cluster nearby |
| Major-hub exclusion | Airports with an existing large, on-site retail cluster are excluded from the transit-adjacent archetype |

### Appendix B — Data sources

Retail, hardware, and car-rental point data: OpenStreetMap, under the Open Database Licence.
Transit anchor locations (airports, intercity rail stations): OpenStreetMap, filtered to
public commercial facilities and intercity operators by country. Metropolitan reference
points: public settlement population data. A current, refreshed count for both archetypes
against the live pipeline is a planned near-term follow-up, not included in this posting.

## References

Cervero, R., and K. Kockelman. 1997. Travel demand and the 3Ds: Density, diversity, and
design. *Transportation Research Part D* 2(3): 199–219.

Calthorpe, P. 1993. *The Next American Metropolis: Ecology, Community, and the American
Dream.* New York: Princeton Architectural Press.

Cidell, J. 2010. Concentration and decentralization: The new geography of freight
distribution in US metropolitan areas. *Journal of Transport Geography* 18(3): 363–371.

Duranton, G., and D. Puga. 2004. Micro-foundations of urban agglomeration economies. In
*Handbook of Regional and Urban Economics,* vol. 4. Amsterdam: Elsevier.

Haklay, M. 2010. How good is volunteered geographical information? *Environment and Planning
B: Planning and Design* 37(4): 682–703.

Hotelling, H. 1929. Stability in competition. *Economic Journal* 39(153): 41–57.

Kasarda, J. D., and G. Lindsay. 2011. *Aerotropolis: The Way We'll Live Next.* New York:
Farrar, Straus and Giroux.

Marshall, A. 1890. *Principles of Economics.* London: Macmillan.

Von Thünen, J. H. 1826. *Der isolierte Staat in Beziehung auf Landwirtschaft und
Nationalökonomie.* Hamburg: Perthes.

---

## Contributors

Peter M. Woodfine, Jennifer M. Woodfine, and Mathew Woodfine are credited as founding
contributors to Woodfine Capital Projects Inc.'s geographic-intelligence research programme.

## How this paper was produced

This paper was prepared with AI assistance under human editorial direction; all analytical
claims and conclusions are the responsibility of the named institutional author.

## Disclosures

The datasets this paper describes are built and operated by an affiliate of the paper's
author, Woodfine Capital Projects Inc.; we disclose this because it is relevant to how the
work should be read, not because it changes the falsifiability of the claims tested in §7. All
source data is public and independently reproducible from the sources listed in Appendix B.
This paper contains forward-looking statements about planned data refreshes and future tests;
such statements reflect current intentions and are subject to change without notice.

## Data and reproducibility

Point-of-interest data for both archetypes is drawn from OpenStreetMap under the Open
Database Licence. The clustering and classification methods are described in full in §3. A
current per-country breakdown for both archetypes, refreshed against the live pipeline, is not
yet published; the counts in §2 should be treated as a dated snapshot pending that refresh.
