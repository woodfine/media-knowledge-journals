---
schema: journal-v2
slug: regional-markets
title: "What Qualifies a Regional Market"
subtitle: "Reading the validation a national retailer has already paid for, instead of re-deriving it from population"
site: gis.woodfinegroup.com
imprint: WCP-004
thesis: "A geography qualifies as a Regional Market on the commercial performance of the national retailers already operating there and on which independent anchor categories have converged — not on how many people live there."
abstract: |
  Our thesis is that the useful test of a smaller market is not its population but the
  trading performance of the national retailers who already chose it. A Regional Market
  qualifies on two kinds of evidence, and neither is a population threshold. The first is
  retail productivity: a modeled estimate, drawn from commercial location-intelligence data
  rather than from any figure a retailer discloses itself, of a national hypermarket
  operator trading above its own chain median in that geography, reinforced by strong
  secondary trade indicating the node draws from a wider area than its own town. The second
  is anchor composition: which independent categories of large-format retailer have
  converged there. Population is not merely excluded from the published selection — it is
  negatively correlated with the composition measure in every country tested, so selecting
  on it would systematically replace genuine regional markets with dense metropolitan-fringe
  suburbs. The arithmetic is worth stating plainly: 1,771 markets currently clear the
  composition gates across both continents — 1,121 in North America and 650 in Europe — and
  800 are published, 400 per continent. The published set is a deliberate editorial cut, not
  a claim that exactly 800 markets qualify. The main limit: the retail-productivity estimate
  is a modeled figure from a commercial data provider rather than open map data, so it is
  the one input in this method a reader cannot independently reconstruct.
state: draft
version: "0.1.0"
published:
updated: "2026-09-16"
cite_as:
license: CC-BY-4.0
cites:
  - christaller-1933-central-places
  - reilly-1931-retail-gravitation
  - huff-1964-trading-area
  - holmes-2011-walmart-diffusion
  - nber-w17220-costco
  - marshall-1890-principles-of-economics
  - duranton-puga-2004-agglomeration-microfoundations
  - wrigley-lowe-2002-reading-retail
  - krugman-1991-geography-and-trade
  - ester-1996-dbscan
  - haklay-2010-osm-quality
  - osm-odbl
draws_from:
  - regional-market-demographic-threshold
  - about-regional-markets-system
  - atlas-top-400-north-america
  - atlas-top-400-europe
  - co-location-target-hierarchy
  - geographic-co-location-methodology
  - co-location-methodology
  - power-centres
  - national-tenants
  - gis-data-overview
  - trade-area-data-sources
prepared_by: "Woodfine Management Corp."
keywords:
  - regional markets
  - retail productivity
  - market qualification
  - anchor composition
  - site selection
---

> Nothing in this paper constitutes an offer to sell, or a solicitation of an offer to buy,
> any interest in a Woodfine direct-hold solution; any offering is made only by the
> applicable Private Placement Memorandum. Statements marked "planned," "intended,"
> "targeted," "may," or "expected" are forward-looking and subject to change. Full
> disclosures appear at the end of this paper.

Working Paper WCP-004 · v0.1.0 · CC BY 4.0

Our thesis is that the useful test of a smaller commercial market is not how many people live
there but how well the national retailers who already chose it are trading. **Regional
Markets** is the name for the geographies this test selects: named towns and satellite
municipalities that qualify on the commercial performance of the national retailers already
operating there — not on population alone.

That distinction is the whole paper, and it is not a technicality. Almost every conventional
account of a smaller market reaches for a population band: a regional market is a place with
between so many and so many thousand residents. It is an intuitive shortcut and it is the
wrong instrument, for a reason that turns out to be measurable rather than philosophical.
Population, as we set out below, is *negatively* correlated with the measure that actually
distinguishes a regional market from its neighbours — which means a method that selected on
population would systematically discard the genuine regional centres and fill the list with
dense suburbs on the edge of big cities instead.

The test that works has two parts, and they answer different questions. One characterises the
geography: is a national hypermarket operator trading above its own chain median here, and
does the node draw shoppers from beyond its own town? The other decides entry to the published
list: which independent categories of large-format retailer have actually converged here? Both
read a decision that somebody else, with far better data than ours, has already made and paid
for. This paper explains both, states what the method deliberately does not attempt, and
publishes the arithmetic of the gap between how many markets qualify and how many are actually
listed.

## 1. The thesis

A large national retailer deciding where to put a store has three things nobody outside it
has: transaction data from thousands of existing stores, a research function whose entire job
is site selection, and capital genuinely at risk on the answer. We do not have access to that
transaction data ourselves — no retailer discloses store-level sales, and none of what follows
depends on pretending otherwise. What we read instead is a modeled retail-productivity
estimate, built by a commercial location-intelligence provider from device-based foot-traffic
and transaction-adjacent signals, which — when it places a given store *above the chain's own
median* for that geography — is the closest checkable proxy for the two facts that actually
matter, established far more cheaply than any external study could establish them directly.

The first fact is that the company believed in the location strongly enough to build. The
second, and the more informative one, is that the belief appears to have been borne out. A
store estimated above the chain median is operating in a trade area where modeled consumer
purchasing volume exceeds the company's own average expectation — which has only two
structural explanations. Either the local population has above-average purchasing capacity, or
the site draws customers from a wide area beyond its own community. Or both.

This modeled estimate is a useful instrument here precisely because it is a composite. It is
built to reflect trade-area income, how often people visit, and what households actually have
to spend — not a raw demographic projection of what they might spend. It is, in other words, a
serious commercial proxy for the retailer's own performance, not the retailer's own reported
number, and this paper is explicit about that distinction throughout.

Our position is that reading this is better than re-deriving it. A geography that passes this
test has been validated by an institution with decades of site-selection experience and full
access to proprietary consumer data. The alternative — commissioning our own demand study,
projecting our own population growth, modelling our own income trends — would be an attempt to
reproduce, with worse inputs, an analysis somebody has already completed at their own expense.
The composition is the claim: read the validation, do not repeat it.

There is one further piece. A strong hypermarket alone establishes consumer volume and nothing
more. The presence of a home-improvement superstore about a kilometre away adds a different
fact — that the area supports a working trade-contractor base, and therefore an active
construction and renovation economy. The presence of a membership warehouse club adds a third
— that enough households have the income and the storage space to make an annual membership
fee and bulk buying worth it. Each of these is a different institution reaching a different
conclusion about the same place. The economics of why firms benefit from being near one
another is well established [marshall-1890-principles-of-economics]
[duranton-puga-2004-agglomeration-microfoundations]; the point here is narrower, and it is
evidential rather than economic. Three independent verdicts are better evidence than one, and
much better evidence than a forecast.

## 2. The problem, in the reader's terms

The intuitive definition of a regional market is "a smaller city." It has a population range
attached to it, and it is used constantly, and it fails in a specific way.

Think about how a property is actually valued. A surveyor can produce an estimate from the
characteristics of a building — its size, its age, its condition, comparable rents in the
area. That estimate is useful. But if the building sold last month in an arm's-length
transaction, the price it fetched is better evidence than the estimate, and no competent
appraiser would prefer the model to the transaction. The price is what buyers with real money
at stake actually concluded, after doing their own work, in the actual market. The model is
what someone thinks they would conclude.

Population is the model. Retail productivity is the transaction.

A population figure tells you how many people are within a boundary. It does not tell you what
they earn, how often they shop, whether they shop locally or drive somewhere better, or
whether anyone from outside the boundary comes in. Two towns of sixty thousand people can be
entirely different commercial propositions: one where residents drive forty minutes to a
bigger centre for anything substantial, and one that is itself the place people drive forty
minutes *to*. The population figure is identical. The commercial reality is opposite.

Which brings us to the finding that settles the argument. When the qualifying composition
measure was tested against population, country by country, the correlation came out
**negative in every country tested**. Not weak — negative. Selecting on population would
systematically swap out the genuine regional centres and swap in dense metropolitan-fringe
suburbs, which have large populations precisely because they are extensions of a bigger city
and which therefore do not function as regional commercial hubs at all. The intuitive
shortcut does not merely fail to help. It actively selects against the thing it is meant to
find.

A related correction is worth recording, because it is the same mistake in a different
costume. An earlier version of the selection method included a bonus for distance from a
major metropolitan centre, on the reasonable-sounding theory that a place further out is more
likely to be a genuine regional market. In practice that term caused standalone secondary
cities to outrank real suburbs of major metropolitan areas, which was not the intent. The term
was removed. Distance from a metropolitan centre is now recorded against each market as
descriptive context and takes no part in whether it qualifies.

## 3. What is actually being classified

Three pieces of vocabulary carry this section, and a reader who has not worked in commercial
property will not have met them in this sense.

A **National Retailer** here means a large-format chain operating at national scale — the
hypermarket groups, the home-improvement superstores, the membership warehouse clubs. The word
"national" is doing real work: these are companies whose balance sheets, credit standing and
site-selection processes are national rather than local, which is what makes any single store
decision a reading of something more than local opinion.

A **Power Centre** is a retail development anchored by several of them at once — typically a
warehouse club, a home-improvement superstore and a general-merchandise retailer, each
operating a store of sixty thousand square feet or more. This is the large-format cluster on
the edge of a town, with the shared surface car park and its own traffic signal. It is not a
shopping mall and not a neighbourhood plaza.

A **Regional Market**, then, is a named municipality or equivalent administrative unit that
contains one or more of these co-location clusters and passes the tests below. It is a *place*,
not a site: a town, not a parcel.

### The characterising test: retail productivity and secondary trade

The most direct indicator that a geography is a qualifying Regional Market is a modeled
retail-productivity estimate for the national hypermarket operating there — specifically,
an estimated performance above the chain's own median.

That measure is then reinforced by a second: **secondary trade** at the principal anchor.
Secondary trade is purchasing activity generated by people who travel to the retail node from
*outside* the immediately local community — shoppers who live in towns without a hypermarket of
their own and drive in for major purchases. Strong secondary trade indicates the node is
functioning as a regional commercial hub rather than as a local convenience, drawing from a
catchment wider than its own neighbourhood. This is the oldest question in retail geography —
how far a place draws from, and why some places draw further than others
[reilly-1931-retail-gravitation] [huff-1964-trading-area]
[christaller-1933-central-places].

The secondary-trade characteristic is the one that matters most to what gets built afterwards,
and it is worth spelling out because it is not obvious. The effective customer base for a
professional-services tenant — a law firm, an accounting practice, a dental group, a medical
specialist — is the same wider catchment that generates the secondary trade for the retail
anchor. A professional building co-located with a strong regional anchor is reachable by
clients who drive in from the surrounding smaller communities, not just by the residents of its
own town. That is the mechanism by which a Regional Market of thirty to eighty thousand people
can support the same professional operators who would normally take space in a city of several
hundred thousand: the secondary-trade catchment extends the effective population base well
beyond the resident count.

Note what has just happened to the population figure. It has not vanished — a range does appear
— but it has changed status. It is an observation about the kinds of place this test selects,
not a threshold the test applies.

Two further anchors add confirmation of a specific kind. A home-improvement superstore within
about a kilometre indicates a trade-contractor base, and therefore commercial construction and
renovation activity — which in turn means local professionals in legal, accounting and
financial advisory work have clients engaged in property transactions, business formation and
estate planning. A membership warehouse club within the same distance indicates a concentration
of households whose income supports discretionary spending; the entry of a warehouse club into
a market is a substantial enough event to have measurable effects on the incumbents around it
[nber-w17220-costco]. Neither is a proxy for the other, and neither substitutes for the
hypermarket's own performance.

### The entry test: anchor composition

The characterising test above describes what a qualifying Regional Market *looks like*. What
actually decides entry to the published list is composition — which independent anchor
categories are present across all the co-location clusters inside the named settlement.

A market qualifies under one of three gates. A **Regional Market** carries a hypermarket anchor
plus at least two of hardware, price club, lifestyle, electronics or sport, combined across its
member clusters. A **District Anchor** carries a hypermarket and a hardware anchor and no other
optional category, across at least two distinct clusters. A **Standalone Regional Centre** meets
that same condition in a market isolated from any other qualifying market — a gate that exists
so that a genuine regional centre is not excluded merely for having no qualifying neighbours.

The two tests are consistent rather than competing, because they are answers to different
questions. Composition asks whether independent institutions have converged. Retail
productivity asks how well the resulting node is estimated to be trading. The modeled
productivity estimate ranks and characterises; it does not gate. A top-performing hypermarket in a geography that lacks
the anchor composition does not produce a qualifying market, and a market that clears the
composition gate is not thereby claimed to be trading well.

One more piece of discipline belongs here. Settlements whose member clusters are scattered too
widely to form one trading location are excluded as name-collision artefacts rather than
treated as enormous markets — the constraint is that all of a settlement's clusters lie within
a 200-kilometre bounding box. Clustering of the underlying store locations is done by a
standard density procedure [ester-1996-dbscan], on store records drawn from the openly
licensed world map maintained by volunteer contributors, under the Open Database Licence
[osm-odbl], whose coverage is uneven between countries in ways that have been studied
[haklay-2010-osm-quality].

## 4. What this method deliberately does not do

The qualifying test is a characterisation of what national retailers have already validated.
It is not a set of inputs used to replicate their site-selection analysis, and three specific
things follow.

We do not conduct our own consumer-demand forecasts. We do not produce our own population
growth projections. We do not run our own assessment of income trends in candidate
geographies. Those inputs are treated as already implicit in the trading performance of the
anchor: if a national operator's store is achieving above-median productivity in a geography,
that operator has already established that demand is sufficient, using data we do not have.

This is a real constraint and not a rhetorical one, and it has a cost. A backward-looking
method cannot find the town that is *about to* become interesting. It can only find the town
where the evidence has already arrived. We accept that cost deliberately, on the view that a
late, checkable answer is worth more than an early, unverifiable one — but a reader should
know that is the trade being made, and that a method built this way will always be behind a
genuinely prescient one.

There is a second cost, and it is the one input in this paper a reader cannot check. The
retail-productivity estimate is a modeled figure from a commercial location-intelligence
provider — built from device-based foot-traffic and transaction-adjacent signals rather than
from sales figures any retailer actually discloses — not from the openly licensed map layers
the rest of the method runs on. Everything else described here — the store locations, the
anchor categories, the composition — a reader can download and reconstruct. That one figure
they cannot, and it should not be read as a retailer's own reported number, because it is
not one.

## 5. Why the published list is smaller than the qualifying one

The published output is two lists of four hundred markets, one for each continent, ordered
alphabetically. The arithmetic behind that number has not previously been set out plainly, and
it should be.

Across both continents, **1,771 markets currently clear the composition gates**: 1,121 in North
America, drawn from three countries, and 650 in Europe, drawn from fifteen. **Eight hundred are
published** — four hundred per continent. Nine hundred and seventy-one qualifying markets are
therefore held back by the publication cut.

That gap is not a defect and it is not a hidden failure rate. It is an editorial decision about
how long a usable published list should be, and the only thing wrong with it would be leaving
it unstated, because an unstated cut invites a reader to assume that four hundred is the number
of markets that qualify. It is not. Four hundred is the number published.

The cut falls unevenly by country, and the unevenness is itself informative. The United States
publishes 298 of its 916 qualifying markets — under a third, the deepest reserve in either
continental set. Canada publishes 56 of 112 and Mexico 46 of 93, roughly half each. In Europe
the United Kingdom has by far the deepest pool, 161 qualifying against 55 published, while
Hungary, Bulgaria, Norway and Greece publish their entire qualifying pool, having nothing held
back by the cap at all. There is no per-country quota; a small minimum floor prevents a country
with genuine qualifying markets from being excluded outright, and beyond that the per-country
counts are an observed result of one continental cutoff rather than a target set in advance.

Three further facts about the published sets belong here, because each corrects an assumption
a reader might otherwise make.

**No rank or score is published for any market.** The lists are alphabetical. A composite
measure exists internally to support the selection, and it is not published and is not a
market-facing ranking. There is no first place.

**The composition classes fall very differently on the two continents.** Of the four hundred
North American entries, 382 qualify as Regional Markets and 18 as Standalone Regional Centres —
nine in Mexico, five in Canada, four in the United States — and none as a District Anchor. Of
the four hundred European entries, 399 qualify as Regional Markets and exactly one as a
District Anchor, with no Standalone Regional Centres at all. The standalone class is where the
North American set reaches genuinely isolated regional centres rather than settlements in a
metropolitan orbit, and Europe's settlement geography simply does not produce them.

**Europe's coverage is a scope decision in one respect and a data gap in another, and the two
should not be confused.** Germany, France and the Netherlands are excluded from the current
European methodology under a deliberate lock, not because data is missing. Separately, catchment
population is genuinely absent for 141 of the 400 European markets, and consumer-spend figures
for 178 — with Sweden, Finland, Romania, Bulgaria, Croatia and Norway carrying no catchment
population for any market at all. Those are disclosed gaps in the underlying census and spend
sources. A market without a figure is stated as having none rather than presented as zero. The
North American set has no such gaps.

A last observation that looks like a difference in quality and is not. European markets carry
fewer co-location clusters each than North American ones — 1.36 against 1.77 on average. That
reflects the size of the administrative units, not the strength of the markets: a European
municipality is a considerably smaller geographic unit than a United States incorporated place,
so a European settlement typically contains fewer clusters even where the underlying retail
density per square kilometre is comparable. Reading the two figures as a quality comparison
would be a straightforward error, and it is the kind of error that cross-border retail
comparison invites [wrigley-lowe-2002-reading-retail] [krugman-1991-geography-and-trade].

## What this changes for the reader

The first change is that "is this a Regional Market?" becomes a question with a checkable
answer rather than an impression. A reader with a candidate town can ask: is there a national
hypermarket here, and is there a home-improvement superstore and a warehouse club near it? The
composition half of the test is visible on any public map. The productivity half is not, and a
reader should treat it as the part they are taking on trust.

The second is a correction to a habit. Population is the number everyone reaches for when
sizing a market, and this work says it is the wrong number — not merely a weak one, but one
that runs the wrong way against the thing being measured. That is worth carrying into any
market assessment, not just this one.

The third is a clearer read on what a published list actually is. Eight hundred markets are
listed; 1,771 qualify. An alphabetical list with no rank is not a ranking with the rank hidden.
And a market's presence on the list says that independent anchors have converged there — it
says nothing about whether anything has been acquired, optioned or developed anywhere.

The trade-offs belong in the same paragraph. The method is backward-looking and therefore
structurally late. Its central measure — anchor trading performance — is not reconstructible by
the reader. Its coverage is genuinely uneven, with more than a third of European entries
missing a catchment population figure. And the two-part test described in Section Three, one
part characterising and one part gating, is a real complication rather than an elegance: a
reader who only remembers one of the two will get the method wrong in one direction or the
other.

## An open invitation

Several of the questions here are properly the business of people who study regional economies
rather than build in them.

To regional economists: the load-bearing assumption in this paper is that anchor retail
productivity is a durable proxy for the underlying economic health of a smaller market. That
assumption has held well through the period the method was built in. Whether it survives the
next decade of change in retail formats — as more of a household's purchasing moves away from
the physical store, and as the store's role shifts toward fulfilment and collection — is a real
question we do not resolve. If the hypermarket's modeled retail-productivity estimate ceases to be a good
reading of a town's economy, this method degrades quietly rather than failing loudly, which is
the more dangerous mode. We would welcome work that tests when and where the proxy breaks.

To retail-location researchers: the arrival-sequence assumption — hypermarket first, then
hardware and warehouse operators following — is read from observed site behaviour rather than
demonstrated here. The literature on chain expansion and density economics is much better
placed to say whether the sequence is general, whether it differs between North America and
Europe, and whether it is changing [holmes-2011-walmart-diffusion].

To anyone working on secondary trade: the secondary-trade characteristic in Section Three is
doing a great deal of work in this argument and is the least directly measured thing in it. A
method for estimating how much of a node's trade comes from beyond its own community, from
open data, at continental scale, would improve this work more than any other single addition.
We do not have one.

And to statistical agencies and researchers in the six European countries with no catchment
population coverage: the gaps reported in Section Five are gaps in what we could source, not
claims that the data does not exist. If a national or regional open source would close one of
them, we would rather be told than continue publishing the absence.

## Conclusion

A Regional Market qualifies on what the national retailers already there are actually doing —
trading above the chain's own median, drawing from a catchment wider than the town, and
converging with other independent anchor categories at the same node — and not on how many
people live within a boundary. That is a narrower claim than it sounds, and a more checkable
one. It rests on reading validation that a large, well-informed institution has already paid
for, rather than re-deriving it from worse inputs. The population shortcut is not just less
precise than this test; it points the other way, which is why the published lists exclude it
from selection entirely. And the published lists are a cut: 1,771 markets qualify, 800 are
listed, and saying so is part of what makes the list worth reading.

## References

Christaller, W. 1933. *Die zentralen Orte in Süddeutschland.* Gustav Fischer.

Duranton, G., and Puga, D. 2004. Micro-foundations of urban agglomeration economies. *Handbook
of Regional and Urban Economics*, vol. 4. Elsevier.

Ester, M., Kriegel, H.-P., Sander, J., and Xu, X. 1996. A density-based algorithm for
discovering clusters in large spatial databases with noise. *Proceedings of KDD-96*, 226–231.

Haklay, M. 2010. How good is volunteered geographical information? *Environment and Planning B:
Planning and Design* 37(4): 682–703.

Holmes, T. J. 2011. The diffusion of Wal-Mart and economies of density. *Econometrica* 79(1):
253–302.

Huff, D. L. 1964. Defining and estimating a trading area. *Journal of Marketing* 28(3): 34–38.

Krugman, P. 1991. *Geography and Trade.* MIT Press.

Marshall, A. 1890. *Principles of Economics.* Macmillan.

National Bureau of Economic Research. *Competing with Costco and Sam's Club: warehouse club
entry and grocery prices.* NBER Working Paper 17220.
[https://www.nber.org/system/files/working_papers/w17220/w17220.pdf](https://www.nber.org/system/files/working_papers/w17220/w17220.pdf)

OpenStreetMap contributors. *Open Database Licence (ODbL) 1.0.*
[https://opendatacommons.org/licenses/odbl/](https://opendatacommons.org/licenses/odbl/)

Reilly, W. J. 1931. *The Law of Retail Gravitation.* Knickerbocker Press.

Wrigley, N., and Lowe, M. 2002. *Reading Retail: A Geographical Perspective on Retailing and
Consumption Spaces.* Arnold.

## Contributors

Prepared by Woodfine Management Corp.

## How this paper was produced

This paper is grounded in the operating and development work the preparing staff do themselves, and in what they have learned from the people they work with routinely: the graphic designers, web developers, and software developers and engineers who build the platform alongside them, and the architects and structural, building-services, and civil engineers they develop buildings with. No outside professional reviewed or approved this paper, and nothing in it is professional advice. It was drafted and edited with AI assistance under editorial direction, and the analysis and conclusions are Woodfine's own.

## Disclosures

Woodfine Capital Projects Inc. ("Woodfine") is the author of record and owns the framework and
the resulting dataset described in this paper; Woodfine Management Corp. maintains the data and
runs the analysis. Woodfine develops and promotes commercial property in the markets this
method selects, so this paper argues for an approach in which we have a direct commercial
interest. This work was funded internally; no external research funding was received. Nothing
in this paper constitutes an offer to sell, or a solicitation of an offer to buy, any interest
in a Woodfine direct-hold solution; any offering is made only by the applicable Private
Placement Memorandum, which prospective investors should review with their own professional
advisors. Inclusion of any market in the published sets reflects the screening criteria
described here and does not indicate acquisition, option, or development activity, committed or
planned, in any market. The named retail chains discussed appear as the subject of a
site-selection method and their inclusion is not a statement about their businesses. Some
statements above describe planned or intended future work; language such as "planned,"
"intended," "targeted," "may," and "expected" marks this forward-looking content, which is
subject to change and does not constitute a commitment regarding future performance.

## Data and reproducibility

The store locations behind the composition test come from OpenStreetMap under the Open Database
Licence — freely downloadable, usable commercially, on terms requiring that a derived database
be shared on the same basis — matched to chains by a canonical brand identifier rather than by
name text, so the same company resolves consistently across borders. Civic records come from an
openly licensed global places dataset and population from an openly licensed gridded population
estimate. A reader with those sources can reconstruct the composition assessment for any
market. One figure in this paper cannot be reconstructed that way and should be read
accordingly: the retail-productivity estimate central to Section Three is a modeled figure
from a commercial location-intelligence provider rather than a figure any retailer
discloses itself or a reader can derive from any open layer. Every count quoted — the 1,121 and
650 qualifying pools, the 400-per-continent publication cut, the 382/18 and 399/1 composition
splits, the per-country published and qualifying figures, the 1.77 and 1.36 cluster densities,
and the European catchment gaps of 141 and 178 markets — is drawn from the current published
dataset build and describes one dated processing run, not a permanent state. The published sets
are a curated editorial selection derived from the live market layer; they do not replace or
alter that layer, which remains unranked and uncurated at its full qualifying count. Coverage
grows as new chain data is ingested. No independent party has audited this dataset, reproduced
these figures, or reviewed these claims.

Woodfine Capital Projects™ is a trademark of Woodfine Capital Projects Inc.
