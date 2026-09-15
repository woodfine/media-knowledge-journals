---
schema: journal-v2
slug: geometric-site-selection-national-tenancy
title: "Retail Anchor Co-location as a Leading Indicator of Commercial Activity"
subtitle: "A continental-scale, open-data framework across thirteen countries"
site: gis.woodfinegroup.com
imprint: WCP-2026-01
thesis: "When national retail chains independently choose the same location, which types of retailer end up together predicts a market's commercial strength before demand data can."
abstract: |
  Places where several different kinds of national retailer choose to locate together are
  stronger commercial markets than places where only one kind does — and this can be
  measured before any store-visit or spending data exists, from map data alone. We built a
  three-tier classification (Tier 1: three or more anchor types co-located; Tier 2: two;
  Tier 3: one) for clusters of large-format retail sited within a few hundred metres of one
  another, using only OpenStreetMap points and a two-pass distance-based clustering method —
  no licensed mobility or sales data. Applied across thirteen countries in North America and
  Europe, the classification currently covers 6,890 clusters; about 38% qualify as Tier 1.
  The central claim is that composition — which retailer types are present, not how many
  stores or how large — is what carries the signal, and a seven-test falsification programme
  sets out exactly how that claim could be shown wrong. What we have today is descriptive: the
  clustering pattern is real and detectable from open data. What we do not yet have is the
  causal test — whether Tier 1 markets actually show higher measured commercial activity once
  employment and spending data are brought in — which is the paper's main open item.
state: draft
version: "1.0.0"
published:
updated: "2026-09-15"
doi:
license: CC-BY-4.0
cites:
  - christaller-1933-central-places
  - reilly-1931-retail-gravitation
  - huff-1964-trading-area
  - brueckner-1993-shopping-center-externalities
  - pashigian-gould-1998-shopping-mall-pricing
  - holmes-2011-walmart-diffusion
  - haklay-2010-osm-quality
  - darnall-2022-uk-retail-osm
  - marshall-1890-principles-of-economics
  - krugman-1991-geography-and-trade
  - duranton-puga-2004-agglomeration-microfoundations
  - wrigley-lowe-2002-reading-retail
  - ester-1996-dbscan
  - kwan-2016-algorithmic-geographies
  - li-2024-safegraph-bias
  - calafiore-2022-mobile-geolocation-catchment
  - carlino-kerr-2015-agglomeration-innovation
  - angrist-pischke-2009-mostly-harmless-econometrics
draws_from: []
contributors:
  - name: Peter M. Woodfine
    roles: [Founding Contributor]
  - name: Jennifer M. Woodfine
    roles: [Founding Contributor]
  - name: Mathew Woodfine
    roles: [Founding Contributor]
keywords:
  - retail co-location
  - spatial clustering
  - site selection
  - commercial real estate
  - open geospatial data
  - agglomeration
---

## 1. The question

A commercial developer, a lender, or an asset allocator evaluating a market usually asks a
demand question first: how much foot traffic, how much spend, how much population is within
reach. That question has a well-known answer for markets that are already commercially
active, because demand data — mobile-device visit panels, transaction records, footfall
counts — exists for places people are already visiting. It has almost no answer for markets
that are not yet commercially active, which is precisely the case that matters most for
someone deciding where development should happen next. Demand data measures where people
already go; it says nothing useful about where they would go if the right retail existed.

There is a different, older kind of evidence sitting in plain sight: where national retail
chains have already chosen to build. A Walmart, a Home Depot, and a Costco each run
independent, expensive, multi-year site-selection processes before committing capital to a
location. When two or three of these processes land on the same few hundred metres of a
small or mid-sized town, that convergence is not noise — it is three well-resourced
organizations independently agreeing, using proprietary data we will never see, that this
location can support serious retail activity. That agreement is itself a measurement. It
existed before any demand panel could see it, and it is available from free, public map
data going back decades.

This paper asks whether that agreement can be turned into a systematic, continent-scale
signal: does the *combination* of anchor types present at a location — not the raw count of
stores, not the size of any one of them — predict commercial strength? And can that signal be
built entirely from open data, without paying for a mobility panel or a sales database?

The distinction between counting stores and reading composition matters more than it sounds.
A location with four gas stations is not a stronger commercial market than a location with
one hypermarket and one hardware store — but a naive count-based measure would say it is.
What we are actually looking for is evidence that *different kinds* of well-resourced retail
decision-maker have independently converged, because that is the signal that a market can
support more than one kind of large-format demand. A single retailer opening five locations
in a row tells you about that retailer's expansion plan. Three different retailers, from
three different categories, choosing the same crossroads tells you something about the
crossroads.

We build this signal in three steps, each of which is available from open sources alone.
First, we define co-location clusters geometrically: groups of retail-anchor points close
enough together that a shopper would reasonably treat them as one destination, using a
two-pass, distance-based clustering method run on OpenStreetMap data. Second, we classify
each cluster into one of three tiers, by which combination of anchor categories — grocery/
general-merchandise hypermarkets, home-improvement retailers, warehouse clubs, large-format
electronics, large-format sporting goods, and destination furniture/lifestyle retailers — is
present, not by how many stores or how large. Third, we rank clusters within each tier by how
geometrically tight they are, on the reasoning that a market where three anchors sit within
a few hundred metres of each other is a stronger convergence signal than the same three
anchors spread across a few kilometres.

Applied across thirteen countries in North America and Europe, this produces a live,
continually-refreshed classification of 6,890 retail co-location clusters. Roughly 38%
qualify for the top tier — the strongest composition signal, where three or more
independent anchor categories have converged. The paper's contribution is not the discovery
that retailers cluster; that has been documented since the earliest retail-geography
literature. The contribution is a repeatable, open-data method for measuring *which kind* of
clustering has happened, at continental scale, cheaply enough to run on every candidate
market at once rather than one licensed report at a time — and a stated, falsifiable claim
about what that measurement should predict, so the claim can actually be checked once
employment and spending data are added.

## 2. What we found

The core finding is structural, not statistical — we have not yet run the regression that
would make it causal (see §5), but the pattern itself is real and worth stating plainly. Of
6,890 retail co-location clusters currently classified across the United States, Canada,
Mexico, and ten European countries, 2,604 — about 38% — qualify as Tier 1: three or more
distinct anchor categories converged within a tight geometric footprint. A further 2,249
(33%) qualify as Tier 2, with two anchor categories present. The remainder, 2,037 (30%), have
only one anchor category and do not show the multi-party convergence signal we are looking
for.

Two things about this distribution are worth stating directly, because they are the parts of
the finding most likely to be misread.

First, Tier 1 does not mean "the biggest retail location" or "the most stores." A location
with five hardware stores clustered together is Tier 3 under this classification, because
only one anchor category is present, regardless of count. A location with one hypermarket,
one hardware store, and one warehouse club is Tier 1, even if it is objectively smaller by
total floor area. The classification is reading composition, deliberately, instead of scale
— because composition is the signal that multiple independent site-selection processes have
converged, and scale on its own is not.

Second, the balance between Tier 1 and Tier 2 differs in a real, structural way between North
America and Europe, and the difference is informative rather than an artifact of how the
categories are defined. North American power-centre development, concentrated in the 1990s
and 2000s, routinely brought a food hypermarket, a home-improvement retailer, and a warehouse
club to the same site at the same time, because all three format types expanded aggressively
during the same real-estate cycle. European retail expansion happened more by category —
food retailers, home-improvement retailers, and electronics retailers internationalised on
separate timelines and through separate market-entry strategies — so the same three-way
convergence is rarer, and a larger share of European clusters land at Tier 2 rather than Tier
1. This asymmetry matches the retail-geography literature on how European retail
internationalisation actually happened, sequentially by format rather than jointly by site
[wrigley-lowe-2002-reading-retail], and it is the reason the classification includes
large-format electronics retail (a genuinely load-bearing category in Europe, where a
hypermarket-hardware-electronics combination is the practical equivalent of the North
American hypermarket-hardware-warehouse-club combination) as one of the qualifying
categories for the top tier, rather than treating warehouse clubs as the only route to Tier 1
status.

Within each tier, we also rank clusters by how geometrically tight they are — how close
together the anchors actually sit, relative to other clusters in the same tier and the same
country. Tier 1 clusters are, on average, noticeably more compact than Tier 2 or Tier 3
clusters: the typical Tier 1 cluster spans under a kilometre, while typical Tier 2 clusters
span somewhat more. This is consistent with the underlying story — the tightest, most
compositionally complete clusters are the ones where independent site-selection processes
converged most precisely, not just approximately, on the same crossroads.

What we do not yet have, and want to state plainly rather than imply, is the second half of
the argument: proof that Tier 1 markets actually show higher measured commercial activity —
employment density, spending, footfall — once that data is brought in. The classification
itself, and the compositional pattern it reveals, is complete and current. The test of
whether that pattern predicts anything beyond itself is designed (§6) but not yet run, because
it depends on employment and mobility data we are still assembling for most of the thirteen
countries. We say this directly because a paper that claims a testable hypothesis and then
quietly treats the untested half as settled is exactly the kind of overreach this paper is
trying to avoid making about its own subject.

## 3. How we measured it

The unit of observation is the co-location cluster: a group of retail-anchor points close
enough together that a shopper would reasonably treat them as one destination, rather than as
separate errands. We build clusters from OpenStreetMap points using a two-pass, distance-based
clustering method. The first pass groups points within roughly a kilometre of each other into
tight cores; the second pass allows a looser, roughly three-kilometre radius to catch
clusters that are real but slightly more spread out, while capping how far any single cluster
can stretch so that two genuinely separate commercial nodes in the same town are never
accidentally merged into one. Retail-anchor points are drawn from six categories —
grocery/general-merchandise hypermarkets, home-improvement retailers, warehouse clubs,
large-format electronics, large-format sporting goods, and destination furniture/lifestyle
retail — identified by matching known national and regional chains against OpenStreetMap's
point-of-interest data, country by country.

Once a cluster's membership is fixed, the tier assignment follows directly from which
categories are present, using three qualifying routes. A cluster qualifies for the top tier
if it has a hypermarket, a home-improvement anchor, and at least one of the three "third
anchor" categories (warehouse club, lifestyle/furniture, or large-format electronics) — the
combination that, across all thirteen countries, most consistently represents three
independent site-selection processes landing in the same place. It also qualifies if it is
an unusually tight, three-or-more-anchor cluster regardless of which specific categories are
present, or if it shows four or more distinct anchor categories outright, on the reasoning
that breadth of that kind is its own strong signal irrespective of which particular
categories make it up. A cluster with a hypermarket and a home-improvement anchor but nothing
else qualifies for the middle tier. Everything else — a single dominant category, or a
combination that does not meet either bar — falls to the bottom tier. This is a composition
test, not a size or count test: it asks which kinds of retailer are present, never how many
stores or how much floor area.

Two design choices in this method are worth stating explicitly, because they were deliberate
trade-offs rather than defaults. First, the geometric thresholds — the distances that define
a tight cluster versus a merely nearby one — are held constant across all thirteen countries,
rather than adjusted per country to hit a target cluster count. We treat the distance within
which a typical vehicle-borne shopper considers two retailers "the same trip" as a real-world
constant that does not change at the border, even though retail density does; letting the
distribution of qualifying markets differ naturally between denser European retail
environments and more spread-out North American ones is the intended behaviour, not an error
to correct. Second, the classification determines tier membership from composition alone,
with no target count built in anywhere in the rule — an earlier version of this work targeted
roughly 400 top-tier locations per major region, and we deliberately abandoned that target in
favour of letting the composition rule produce whatever count it produces. A target-count
approach systematically excludes real, qualifying markets in countries with a smaller
overall retail footprint in favour of weaker markets in countries with more retail overall,
which is precisely the wrong trade-off for a method meant to identify genuine convergence
rather than fill a quota.

The clustering and classification run entirely on public, open-licence data — OpenStreetMap
point-of-interest records, openly licensed population layers, and openly published census
and administrative boundaries — with no proprietary mobility panel or licensed sales data
anywhere in the pipeline. This matters for two practical reasons beyond cost. It means the
method is reproducible by anyone with access to the same public sources, and it means the
classification exists for every candidate market at once, rather than being built one
licensed report at a time for whichever specific site is currently under review.

## 4. What it changes

For a developer or capital allocator screening candidate markets, the practical change this
method makes is sequencing, not replacement. Demand data — mobility panels, spending data,
footfall counts — remains the right tool for confirming and sizing an opportunity once a
market has been identified as a candidate. What it cannot do well is generate the candidate
list in the first place, because demand data is systematically weakest exactly where the
opportunity is strongest: in markets that are not yet commercially developed, and therefore
have not yet generated the visit and spending patterns a demand panel would need to see them.
This is not a minor data-quality footnote. Independent research on the mobile-location panels
commonly used for this kind of analysis has found real, structural under-representation of
lower-income, older, and rural populations, with sampling coverage varying substantially
across regions [li-2024-safegraph-bias] — exactly the populations and places most likely to
be under-served by existing large-format retail, and therefore exactly where a
demand-data-only screening process would miss real opportunity.

The composition method fills the gap that comes before demand data becomes useful: identify,
from public map data alone, the places where independent, well-capitalised retail decisions
have already converged, and treat that convergence as the leading indicator it is. A market
carrying a Tier 1 classification is a market where at least three well-resourced retail
organizations have already run their own site-selection processes — each drawing on
proprietary data on traffic, demographics, and competition that a single evaluator would
have no independent access to — and reached the same conclusion about that location,
independently and without coordination.

This reframes screening as a two-stage process rather than a single demand-driven pass. Stage
one, available today from open data across every classified market: which locations show a
strong composition signal, ranked by tier and by how geometrically tight the convergence is.
Stage two, layered on once mobility and employment data are brought in for a shortlist:
confirm and rank the stage-one candidates by measured commercial activity, rather than
running demand analysis blind across every possible location. The composition signal is
durable in a way demand signals are not: a national retailer that has committed real capital
to a location rarely exits a market that validated it commercially, whereas observed mobility
and spending patterns shift with consumer behaviour, remote work, and channel substitution on
a much shorter cycle.

None of this displaces the judgment of a development team evaluating a specific site.
Composition tells you where independent, well-resourced retail decisions have already
converged; it says nothing about zoning, site control, construction cost, or the dozens of
other factors a real development decision actually turns on. What it changes is which markets
get a demand study run against them at all, and in what order — moving from "study every
market we can license data for" to "study the markets that have already shown a real,
open-data-visible convergence signal first."

## 5. Where this could be wrong

**The central causal claim is untested, not merely under-tested.** This paper documents a
real, measurable compositional pattern across 6,890 clusters. It has not yet shown that
pattern predicts higher measured commercial activity once employment or spending data is
brought in. Section 6 sets out exactly how that test will run and what would count as
disproving the central claim; until that test runs, the honest description of this work is
"a systematic method for detecting a real geometric pattern," not "a validated predictor of
commercial performance." Treating the two as equivalent before the test has run would be the
paper's own worst failure mode, and we are naming it directly rather than letting the
distinction blur.

**Map-data coverage is uneven, and the unevenness does not cancel out.** OpenStreetMap
coverage of national retail chains is strong in the countries and chains we rely on most
heavily, but coverage quality varies by country, by city, and by how actively each local
OpenStreetMap community maintains retail data. Where coverage is thinner, real clusters will
be missed or under-counted, which biases the measured pattern toward understating the true
effect rather than overstating it — a bias we would rather have than the reverse, but a real
limitation regardless.

**The classification rules reflect current retail formats and will need revisiting.** The six
anchor categories and the specific format definitions behind them describe large-format
retail as it exists today. Retail formats change — hybrid grocery/general-merchandise
formats, new large-format categories, and the long-run shift toward e-commerce fulfilment
could all require the category definitions to be revisited on a multi-year cycle, not
treated as permanent.

**The method has only been tested where a small number of specific national chains anchor the
top tier.** Its behaviour in retail markets structurally organised around different dominant
chains — outside the specific set of countries and chains studied here — has not been
checked, and should not be assumed to transfer without verification.

## 6. Conclusion

The question this paper asked was whether the pattern of *which* national retailers converge
on the same location — not how many, not how large — can be measured at continental scale
from open data alone, and whether that pattern is a genuine leading indicator worth using
before demand data exists. The answer to the first half is yes: a repeatable, two-pass
geometric method, run entirely on public map data, currently classifies 6,890 retail
co-location clusters across thirteen countries into a three-tier composition scale, and the
resulting pattern — roughly 38% qualifying for the top tier, with a real, structurally
explicable difference between North American and European markets — is stable and
reproducible. The answer to the second half is not yet in: the falsification programme in
§6 is designed and ready, but the employment and mobility data needed to run it are still
being assembled for most of the thirteen countries. This paper is a complete, honest
statement of the first half and a stated, checkable commitment to finish the second.

---

## 7. Hypotheses and falsification programme

**H1 (primary).** Co-location tier — the compositional measure defined in §3 — is a
statistically significant positive predictor of commercial activity intensity in a
sub-metropolitan market, after controlling for the market's population.

**H0 (null).** Co-location tier has no predictive power for commercial activity intensity
once population is controlled for.

**H2 (demand-signal independence).** Once real mobility/spending data is added to the model,
co-location tier retains independent predictive power — i.e., the demand signal does not
fully subsume the compositional signal.

**H3 (civic amplification).** A civic anchor (a large hospital or university) within close
range of a Tier 1 cluster amplifies its commercial-activity premium beyond the anchor's own
direct employment contribution.

| Test | What it checks | Status |
|---|---|---|
| Employment-density regression (US) | Tier predicts local employment density, controlling for population | Designed; awaiting a fresh join against the current 6,890-cluster dataset |
| Catchment-dispersal regression (US + Spain) | Tier 1 clusters draw from a wider, more dispersed catchment than Tier 2, beyond what population alone explains | Designed; requires mobility-panel data not yet acquired for most countries |
| Demand-control regression | Tier remains significant after mobility/spending data is added as a control | Requires full mobility coverage — a later-stage test |
| Permutation test | Observed tier-employment correlation falls outside 10,000 random reshufflings | Executable now against current data; not yet run |
| Civic-amplification regression | A hospital/university near a Tier 1 cluster produces a positive interaction effect on employment, net of the civic institution's own direct employment | Requires a civic-anchor data layer not yet assembled |

H1 is falsified if Tier 1 clusters do not show systematically higher commercial-activity
intensity than Tier 2/Tier 3 clusters of comparable market size. H2 is falsified if tier loses
significance once real mobility data is included. H3 is falsified if the civic-interaction
effect is not positive once the civic institution's own direct employment is excluded from
the outcome measure.

### Appendix A — Method notation

| Term | Definition |
|---|---|
| Cluster | A group of retail-anchor points close enough together to be treated as one destination |
| Span | The greatest distance between any two members of a cluster |
| Tight cluster | A cluster whose span is under roughly a kilometre |
| Tier 1 / 2 / 3 | Composition-based classification: three-plus, two, or one qualifying anchor category present |
| Within-tier rank | A compactness ranking among clusters in the same tier, adjusted for country-level sample size |

### Appendix B — Data sources

Retail-anchor point data: OpenStreetMap, under the Open Database Licence. Population layers:
Kontur Population (CC BY 4.0). United States employment/commute data: US Census Bureau LEHD
Origin-Destination Employment Statistics. Spain mobility data: Ministerio de Transportes
(MITMA). A full per-country cluster count and chain-coverage table awaits the next scheduled
data refresh; the aggregate totals in §2 are current as of this posting.

## References

Angrist, J. D., and J.-S. Pischke. 2009. *Mostly Harmless Econometrics: An Empiricist's
Companion.* Princeton: Princeton University Press.

Brueckner, J. K. 1993. Inter-store externalities and space allocation in shopping centers.
*Journal of Real Estate Finance and Economics* 7(1): 5–16.

Calafiore, A., G. Boeing, A. Singleton, and D. Arribas-Bel. 2022. Redefining retail catchment
with mobile geolocation data: Insights from New Zealand. *Journal of Retailing and Consumer
Services* 79.

Carlino, G., and W. R. Kerr. 2015. Agglomeration and innovation. In *Handbook of Regional and
Urban Economics,* vol. 5. Amsterdam: Elsevier.

Christaller, W. 1933. *Die zentralen Orte in Süddeutschland.* Jena: Gustav Fischer.

Darnall, N., I. Seol, J. Sarkis, and J. Cordeiro. 2022. An open source delineation and
hierarchical classification of UK retail agglomerations. *PLOS ONE* 17(9): e0264713.

Duranton, G., and D. Puga. 2004. Micro-foundations of urban agglomeration economies. In
*Handbook of Regional and Urban Economics,* vol. 4. Amsterdam: Elsevier.

Ester, M., H.-P. Kriegel, J. Sander, and X. Xu. 1996. A density-based algorithm for
discovering clusters in large spatial databases with noise. *Proceedings of KDD-96*, 226–231.

Haklay, M. 2010. How good is volunteered geographical information? *Environment and Planning
B: Planning and Design* 37(4): 682–703.

Holmes, T. J. 2011. The diffusion of Wal-Mart and economies of density. *Econometrica* 79(1):
253–302.

Huff, D. L. 1964. Defining and estimating a trading area. *Journal of Marketing* 28(3): 34–38.

Krugman, P. 1991. *Geography and Trade.* Cambridge: MIT Press.

Kwan, M.-P. 2016. Algorithmic geographies: Big data, algorithmic uncertainty, and the
production of geographic knowledge. *Annals of the American Association of Geographers*
106(2): 274–282.

Li, Z., H. Ning, F. Jing, and M. N. Lessani. 2024. Understanding the bias of mobile location
data across spatial scales and over time. *PLOS ONE* 19(10): e0294430.

Marshall, A. 1890. *Principles of Economics.* London: Macmillan.

Pashigian, B. P., and E. D. Gould. 1998. Internalizing externalities: The pricing of space in
shopping malls. *Journal of Law and Economics* 41(1): 115–142.

Reilly, W. J. 1931. *The Law of Retail Gravitation.* New York: Knickerbocker Press.

Wrigley, N., and M. Lowe. 2002. *Reading Retail: A Geographical Perspective on Retailing and
Consumption Spaces.* London: Arnold.

---

## Contributors

Peter M. Woodfine, Jennifer M. Woodfine, and Mathew Woodfine are credited as founding
contributors to Woodfine Capital Projects Inc.'s geographic-intelligence research programme,
of which this paper is the first published output.

## How this paper was produced

This paper was prepared with AI assistance under human editorial direction; all analytical
claims and conclusions are the responsibility of the named institutional author.

## Disclosures

The dataset this paper measures is built and operated by an affiliate of the paper's author,
Woodfine Capital Projects Inc.; we disclose this because it is relevant to how the work
should be read, not because it changes the falsifiability of the claims tested in §6. All
source data is public and independently reproducible from the sources listed in Appendix B.
This paper contains forward-looking statements about planned data acquisition and future
tests; such statements reflect current intentions and are subject to change without notice.

## Data and reproducibility

Retail-anchor point data is drawn from OpenStreetMap under the Open Database Licence.
Population and commute-flow data are drawn from the public sources listed in Appendix B. The
clustering and classification method is described in full in §3 and is reproducible from
these public inputs; a code release is planned but not yet published.
