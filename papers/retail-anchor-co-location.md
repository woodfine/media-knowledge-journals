---
schema: journal-v2
slug: retail-anchor-co-location
title: "Measuring Retail Anchor Co-location From Open Map Data"
subtitle: "Why the convergence of independent retailers is evidence a reader can check, and a forecast is not"
site: gis.woodfinegroup.com
imprint: WCP-001
thesis: "Where two or three independently operated national retailers have each committed real construction capital at the same node, that convergence is checkable evidence about a location, not a forecast anyone is asked to trust."
abstract: |
  Our thesis is that the best available evidence about a commercial location is not a
  forecast of what will happen there, but a record of what large, independently researched
  companies have already decided to do there. Co-location is the name for reading that
  record. A hypermarket operator, a membership warehouse club and a home-improvement chain
  each run their own site-selection process and each stake construction capital on the
  result; where two or three of them land at the same node without coordinating, each
  company's private judgment is corroborating the others', and the fact of the convergence
  is public. The measurement is built from openly licensed map data covering twenty-four
  countries in North America and Europe, and every node is sorted into one of four
  classes by tests that must each pass in turn rather than by a score in which a strong
  reading offsets a weak one. Two limits belong up front. Catchment population and a
  modelled spend estimate do enter the classification as a country-relative rank, so this
  is not a method with no demographic input at all — what it excludes is a demand forecast
  and any study commissioned by a party with an interest in the answer. And the number of
  nodes the method finds is a result of the clustering settings chosen: across the
  defensible range tested, the North American count moves by more than a factor of two on
  identical retailer data.
state: draft
version: "0.1.0"
published:
updated: "2026-09-16"
cite_as:
license: CC-BY-4.0
cites:
  - marshall-1890-principles-of-economics
  - christaller-1933-central-places
  - hotelling-1929-stability-in-competition
  - reilly-1931-retail-gravitation
  - huff-1964-trading-area
  - calafiore-2022-mobile-geolocation-catchment
  - pashigian-gould-1998-shopping-mall-pricing
  - brueckner-1993-shopping-center-externalities
  - holmes-2011-walmart-diffusion
  - ester-1996-dbscan
  - haklay-2010-osm-quality
  - kwan-2016-algorithmic-geographies
  - li-2024-safegraph-bias
  - brodsky-2018-h3
  - overture-maps
  - osm-odbl
draws_from:
  - co-location-methodology
  - co-location-intelligence-overview
  - co-location-anchors
  - co-location-ranking-system
  - co-location-tier-nomenclature
  - catchment-ranking-methodology
  - geographic-co-location-methodology
  - co-location-target-hierarchy
  - gis-data-overview
  - trade-area-data-sources
  - spend-population-provenance
  - od-catchment-methodology
  - gis-cluster-scoring-glossary
  - power-centres
  - retail-centres
prepared_by: "Woodfine Management Corp."
keywords:
  - retail co-location
  - site selection
  - open map data
  - anchor tenants
  - commercial real estate
---

# Measuring Retail Anchor Co-location From Open Map Data

*Why the convergence of independent retailers is evidence a reader can check, and a forecast is not*

> Nothing in this paper constitutes an offer to sell, or a solicitation of an offer to buy,
> any interest in a Woodfine direct-hold solution; any offering is made only by the
> applicable Private Placement Memorandum. Statements marked "planned," "intended,"
> "targeted," "may," or "expected" are forward-looking and subject to change. Full
> disclosures appear at the end of this paper.

Working Paper WCP-001 · v0.1.0 · CC BY 4.0

Our thesis is that the strongest available evidence about a commercial location is not a
forecast of what will happen there, but a record of what large, independently researched
companies have already decided to do there. When somebody asks you to believe a location is
a good one, they will usually hand you a projection: a study of how many people live nearby,
how much they earn, how many of them are expected to move in over the next ten years, and
what all of that implies for a business placed at that corner. You are being asked to trust
a forecast. You cannot re-run it, the assumptions behind it are rarely published, and by the
time it has been shown to be right or wrong your money has been in the ground for years.

There is a different kind of evidence available, and it has been sitting in plain view. A
national grocery and general-merchandise chain, a membership warehouse club and a
home-improvement chain each maintain their own real-estate research function, each apply
their own criteria, and each commit tens of millions of dollars of construction capital to a
site before a single customer walks in. When two or three of those companies independently
choose to build within about a kilometre of one another, each one's private judgment is
corroborating the others'. **Co-location** is the name for the strategy of reading that
convergence: a proximity test that validates a location by the physical footprints major
retailers have already put there.

This paper sets out why we treat that convergence as the primary site-selection signal, how
it is measured from map data anybody can download, and — just as importantly — what it does
not tell you. The method describes a pattern that has already happened. It makes no claim
about what will happen next at a site where the pattern is absent, and it is not a
prediction that any particular converged node will perform well. Two of the real limits sit
in the middle of the method rather than at its edges, and they are stated in full in Section
Four rather than buried.

## 1. The thesis

Three things make a national retailer's site decision worth reading.

The first is that it is expensive. Opening a large-format store is not a lease on an office
floor that can be walked away from at the next break clause. It is land assembly, municipal
approval, a building, parking, servicing, and a supply chain reconfigured to reach it. A
company that has done this has put capital at risk that it cannot recover quickly if it was
wrong.

The second is that it is researched. These companies employ real-estate analysts whose
entire job is to decide where the next store goes, using traffic counts, road-network
studies, competitive positioning, and proprietary consumer data drawn from their own
transactions across thousands of existing stores. They are not guessing, and they are not
publishing what they know.

The third, and the one that carries the argument, is that the decisions are **independent**.
A hypermarket operator does not consult a warehouse club before choosing a site, and neither
consults the home-improvement chain. Each runs its own process against its own criteria and
its own customer data. When three separate processes, run by three separate companies with
three separate business models, converge on the same corner of the same town, that is three
independent confirmations of the same underlying fact about that place.

That is the whole claim. Convergence is corroboration. It is not a new forecast built on top
of the retailers' forecasts; it is a reading of the decisions they have already made and
paid for. The economics literature has understood for well over a century why firms cluster
rather than spread out — the shared labour pool, the shared suppliers, and the shared flow
of customers that make a group of businesses in one place worth more than the same
businesses scattered [marshall-1890-principles-of-economics]. The retail case has its own
long-standing account of why a shopping centre's anchor tenants generate traffic the smaller
tenants cannot generate for themselves, which is why anchors are courted and subsidised
rather than charged the going rate [pashigian-gould-1998-shopping-mall-pricing]
[brueckner-1993-shopping-center-externalities]. And there is a body of work on why
competitors position themselves close to one another rather than apart, which is the reason
a hardware chain's presence tends to draw its rival rather than repel it
[hotelling-1929-stability-in-competition].

What we are adding is not the theory. It is the discipline of treating the convergence as
the *measurement* rather than as a supporting illustration for a conclusion reached some
other way — and of taking that measurement from data the reader can obtain and check.

## 2. The problem, in the reader's terms

Consider how you would normally be persuaded that a piece of commercial property is worth
buying.

You would receive a package. In it would be a market study: population within five, ten and
twenty kilometres; median household income; projected growth; retail spending per head;
perhaps a traffic count. The study would be prepared by a consultancy, commissioned and paid
for by whoever wants you to buy the property. It would be competent and it would be sincere.
It would also be, structurally, an argument for the transaction, and its assumptions — the
growth rate chosen, the catchment boundary drawn, the comparable properties selected —
would not be shown to you in a form you could vary and re-run.

Now consider a different document in the same package: a building inspector's report. You
commission it, not the seller. It does not tell you what the building will be worth in ten
years. It tells you the condition of the roof, the age of the furnace, the state of the
wiring — facts about the building as it stands, each of which you can go and look at
yourself if you want to, and each of which a second inspector would find the same way. You
do not have to trust the inspector's judgment, only their eyesight. The report is weaker
than the market study in the sense that it predicts nothing, and stronger in the sense that
nothing in it depends on the report's author wanting you to buy.

What we are proposing is a building inspector's report for a *location* rather than a
structure. It tells you nothing about how the location will perform. It tells you which
national retailers have already built there, how close together, and what kinds of company
they are — facts that are on the public record, that any reader can confirm on a map, and
that were established by parties with no interest whatever in whether you buy the parcel
next door.

The traditional objection is that this is a thin kind of evidence: it says only that some
big shops are near each other. We think the objection has it backwards. The thinness is the
point. A thin fact that is checkable by anyone beats a rich conclusion that is checkable by
nobody, because the rich conclusion's richness comes entirely from assumptions the reader
never sees.

## 3. What a large-format retailer is, and why its choices are readable

Before the measurement, the vocabulary — because the whole argument rests on a distinction
between kinds of store that is not obvious from the outside.

A **Power Centre** is a retail development anchored by several large-format, national-chain
stores — typically a warehouse club, a home-improvement superstore and a general-merchandise
retailer — each operating a store of sixty thousand square feet or more. This is the format
familiar from the edge of almost any mid-sized town in North America and, increasingly, in
Europe: a cluster of very large buildings around a shared surface car park, on an arterial
road, with its own traffic signal. It is not a shopping mall — there is no enclosed concourse
and no small-tenant corridor — and it is not a neighbourhood plaza with a supermarket and a
dry cleaner. It is a group of destinations, each large enough to pull a customer out of their
way on its own.

Four kinds of anchor carry weight in the measurement, and each says something different
about the place it sits in.

**Hypermarket** anchors are the general-merchandise chains that also sell groceries —
Walmart and Target in North America, Mercadona in Spain, Tesco in Britain, Carrefour across
much of Europe. This format is the one an operator deploys only where it has satisfied
itself that a single site can support a full grocery *and* a full general-merchandise
business at institutional scale. It is also, in practice, the first to arrive: the
hypermarket brings the road improvements, the utility connections and the site preparation
that the others need in order to follow.

**Warehouse** anchors are the membership clubs — Costco, Sam's Club, Makro. Their business
model contains a built-in screen. A customer must pay an annual fee before buying anything,
and must then buy in quantities that assume storage space at home and cash to spend in
advance. A club that trades profitably in a town has established that enough households
there have both.

**Hardware** anchors are the home-improvement chains — Home Depot, Lowe's, Leroy Merlin.
They serve two customers at once: the homeowner doing work on a house they own, and the
trade contractor buying materials for a job. Their presence therefore indicates both an
owner-occupier base and an active construction and renovation trade — a working local
economy, not just a residential one.

**Lifestyle** anchors are the large-format home-and-furnishings retailers. In this
measurement IKEA is the only chain in the class, which is a statement about how few
operators run that format at that scale rather than a preference.

Two categories of store are deliberately left out. Neighbourhood-format grocery chains are
excluded because they are almost everywhere; including them would produce a map covered in
clusters that carry no development signal at all. Food retailers more broadly appear as
context but do not enter the tests. The classification is looking for the presence of
*independent* anchor categories, not for a count of shops: four hypermarket banners at one
node still represent one category of judgment, repeated.

One consequence is worth stating plainly for a reader who has not worked in this industry.
The relationship that matters is between the anchors and *each other*, not between the
anchors and the site we might build on. A professional office building sited within one
kilometre of a Power Centre perimeter shares the traffic and the servicing that the retailers
created; a building further away has to create its own reason for anyone to drive there. That
one-kilometre figure is a fixed siting rule for the building type, applied to the perimeter
rather than to any single store, and it is the reason proximity is measured at all.

## 4. What the measurement is, and what it is not

### The raw material

The store locations come from OpenStreetMap, the openly licensed map of the world built by
volunteer contributors, published under the Open Database Licence [osm-odbl]. Records are
selected by a canonical brand identifier rather than by the store's name text, so that a
chain trading under different spellings, different local formats, or different scripts across
several countries still resolves to one company. Civic records — hospitals, and higher-education
sites — come from the Overture Maps Foundation's open Places dataset [overture-maps].
Population comes from an openly licensed gridded population estimate, which models where
people live from census microdata and satellite imagery rather than reporting them by
administrative boundary; it is delivered on a single worldwide hexagonal grid, so a figure
computed for a cluster in Norway is computed exactly the way one in Mexico is
[brodsky-2018-h3].

The material point about all of this is the licence. Every layer named above can be
downloaded by the reader, under terms that permit commercial use, without asking us or
anyone else for permission. A researcher who wants to disagree with the classification has
access to the same inputs we do.

That openness has a well-documented cost, and it would be dishonest to leave it out.
Volunteer-contributed map data is uneven: its completeness varies by country, by region,
and by category, and it has been studied precisely for that reason
[haklay-2010-osm-quality]. A chain that is thinly mapped in one country will appear to have
fewer stores there than it does. Coverage grows by ingest rather than arriving complete, and
each expansion changes what the map shows.

The co-location footprint currently spans **twenty-four countries** in North America and
Europe, as of the most recent full processing run. That is this method's own count, and it
is worth stating precisely because it is not the only country count in this field of work:
the population and consumer-spend layer described below is built for thirteen of those
twenty-four, and the published market list that draws on this dataset covers a different,
smaller set again. Three numbers, three different things.

### Forming a node

Individual store records are grouped into a **cluster** — the node against which everything
downstream is measured — when they fall within a defined span of one another. The grouping
uses a density-based clustering procedure of a standard and long-established kind: points
that sit close together in sufficient number form a group, and isolated points are left out
rather than forced into the nearest one [ester-1996-dbscan]. The span conventions themselves
are platform parameters, re-tuned between rebuilds as chain coverage changes, and are not
published.

Here is the first limit, and it is a real one. **The number of clusters is a result of the
settings, not a count of things that exist in the world.** Clustering partitions the
locations observed under a chosen density model; it does not recover a true,
setting-independent number. Parameter sweeps run during development show this directly:
across the defensible range tested, the North American cluster count varies by more than a
factor of two with no change whatsoever to the underlying retailer data. Any cluster count
is therefore a figure produced under one parameterisation, and an unqualified count would
invite a reader to treat a modelling choice as an observed fact. This is the general problem
with deriving geographic conclusions from an algorithm — the algorithm's own choices become
invisible in its output, and the output looks like a finding [kwan-2016-algorithmic-geographies].

### Classifying it

Every cluster is assigned one of four classes, from highest to lowest: **Regional**,
**District**, **Local**, and **Fringe**. The names follow the retail property hierarchy used
by the International Council of Shopping Centres, though only "Regional" is genuinely that
body's term; the other three are our own naming choices, adopted because a planner who opens
the map without reading anything already knows roughly what "Regional" means.

A cluster earns its class by passing every test that class requires — not by accumulating
points toward a threshold. Five families of test apply:

**Composition.** Which independent anchor categories are present. Regional requires a
hypermarket anchor paired with a warehouse or lifestyle anchor. District requires a
hypermarket paired with hardware or warehouse. Local requires a hardware or warehouse anchor.

**Catchment rank.** Where the cluster's trade-area population stands against every other
cluster **in its own country**, expressed as a percentile. Ranking within a country rather
than against one global bar is what keeps a nationally significant node in a small country
from being swamped by the sheer scale of a larger one.

**Spend rank.** The same idea applied to a modelled estimate of consumer spending in the
trade area, required at some classes as a separate test from population.

**Civic.** Whether a hospital of the required classification sits within a surrounding ring.
The requirement tightens as the class rises: the highest class requires a hospital serving a
regional catchment, and a walk-in clinic does not satisfy it.

**Non-overlap.** Whether a stronger nearby cluster already dominates the same node. Two
clusters are compared using a fixed-radius disk centred on each; where the overlap exceeds
the limit, the weaker one is held below the class its composition would otherwise earn. This
prevents one genuinely strong node from being counted several times as separate nodes.

The trade area those population and spend figures are drawn from is defined by two
straight-line bands: a primary zone within thirty-five kilometres of the node, and a
secondary zone from thirty-five to one hundred and fifty. These are distance bands, not
measured catchments, and they are labelled that way. A distance band approximates where
customers come from; it does not observe where they actually come from. The move to
reachability along the road network, and to observed origin data, is planned and not built.
The classical models for estimating where a shopper will choose to go — the gravity
formulations that still underpin most commercial trade-area work — assume exactly the kind
of observed behaviour this layer does not yet have [reilly-1931-retail-gravitation]
[huff-1964-trading-area].

Tests replaced a points-based composite score in May 2026, and the reason is worth a
sentence, because it is the same reason this paper prefers convergence to a forecast. Under
the old scale a node could reach a high class on a strong reading of one term while lacking
the catchment reach or the civic infrastructure that the class was supposed to signal. The
signals are not interchangeable — a hypermarket validates consumer volume, a hardware anchor
validates trade activity, a regional hospital validates institutional employment that does
not depend on retail at all — and a system that adds them together treats them as though
they were. The retired scale and its numeric labels describe no current cluster.

### What does not enter, and what does

Three statements about the classification's inputs, in descending order of how flattering
they are.

**No consumer survey, demand forecast, or commissioned market study enters the
classification anywhere.** There is no growth projection, no income-trend assessment, and no
estimate of future demand at any node. That is the discipline the whole method exists to
hold.

**Sales performance does not qualify a node.** A modeled retail-productivity estimate for
the hypermarket at a node — drawn from a commercial location-intelligence provider, not from
any figure the retailer discloses itself — is a ranking measure used later, when
already-qualified nodes are ordered into a shortlist. It carries no weight in whether a node
passes any test. Nor is it open map data: it comes from a commercial data provider rather
than from the openly licensed layers described above, and a reader cannot reconstruct it
from a map.

**Population and modelled spend do enter, as a country-relative rank.** This needs saying
directly, because a shorter version of this argument would leave the impression that the
method touches no demographic data at all, and that is not true. Catchment population, and a
spend figure derived from it, are two of the five test families. What is excluded is a
*forecast* and any study produced by a party with an interest in the result — not
demographic measurement as such.

And the spend figure carries its own weakness, which we would rather name than have found.
It is population multiplied by a single national per-capita expenditure rate drawn from a
household budget survey. Every resident of a country is assigned the same spending rate
regardless of where they live: a household in central London and a household in a Welsh
market town receive the identical grocery multiplier. Affluent catchments are therefore
systematically understated and lower-income catchments systematically overstated, and
because the error tracks the local income gradient it does not average out across a trade
area — it pushes the whole total one way. Varying the rate below the national level using
local income data is planned and not built. Multipliers are also expressed in local currency
with no exchange-rate normalisation, so a spend comparison is defensible within one country
and not between two.

Two further gaps belong here rather than in a separate confession. Universities and colleges
are collected in the same civic layer as hospitals and genuinely inform the case for
professional-services demand around a node, but in the current tests they satisfy no
requirement on their own — the civic tests read hospital classification only. And a
per-market confidence flag is computed for every entry, reflecting how cleanly a place name
resolved; at the most recent full run roughly ninety-nine per cent of entries carried the
high-confidence value. That flag is not yet drawn on the map. Every node renders identically,
so a lower-confidence estimate is visually indistinguishable from a higher-confidence one.
Encoding it — by opacity, or by a hollow rather than filled marker — is intended and not
built.

## 5. Sorting a qualifying list without predicting anything

Classification answers "does this node qualify?" It does not answer "which of the qualifying
nodes should be looked at first?" That second question is a separate step, and keeping the
two apart is what stops the method from quietly turning into the forecast it was meant to
replace.

Once a node has passed its tests, the ordering within a class and a country runs through a
fixed sequence of criteria and ends in a tiebreak that cannot produce a tie. The consequence
is that the ordering is fully deterministic: the same data returns the same order on every
run, so a position cited in one review can be reproduced in the next. Nobody exercises
discretion at the point of ordering, and there is no adjustment for a site somebody happens
to favour.

What the resulting order is *for* is deliberately modest. It produces a shortlist from which
real-estate professionals are engaged in each identified market to assess whether land is
actually available and what the development timeline would be. The shortlist must be
substantially longer than the number of sites required, because not every high-ranked node
has developable land beside it, and some available parcels carry rezoning or permitting
timelines running three to seven years. The ranking narrows a continent to a list of places
worth a phone call. It does not select a site.

A position on that list is a description of where convergence has already occurred. It is not
a forecast of performance, not a recommendation, and not an indication that anything has been
acquired, optioned, or developed anywhere.

## What this changes for the reader

The first change is that a claim about a location becomes checkable. Told that a site sits in
a validated commercial node, a reader can go to the same public map, look at the same
anchors, and see for themselves whether a hypermarket, a warehouse club and a
home-improvement chain are actually there and actually close together. Nothing in that check
requires our cooperation. That is a materially different relationship to evidence than
reading a study and deciding whether to believe it.

The second is that the reader learns what kind of claim is being made. Convergence is
backward-looking by construction. It reports that several well-capitalised companies have
already committed, and it is silent about what happens next. A reader who wants a forecast
should know they are not getting one here, and should treat any number in this method as a
description of the present rather than a projection.

The third is a sharper set of questions to ask of anyone else's site analysis. Which of these
inputs did you observe, and which did you model? Is your spending figure measured or is it a
national average multiplied by a headcount? Is your trade area drawn from where customers
actually come from, or from a circle on a map? Would your conclusion survive somebody else
re-running it on data they downloaded themselves? We ask those questions of our own work in
Section Four, and we think a reader is entitled to ask them of anyone.

The trade-offs are real and belong in the same paragraph as the benefits. A backward-looking
method is systematically late: it can only find a place after the retailers have already
arrived, which means it cannot find the town that is about to become interesting. It is
blind wherever the open map is thin, and the open map is thinner in some countries than
others. Its cluster count moves with its own settings. And its spend layer is an
approximation that is wrong in a predictable direction. None of this makes the method
useless; all of it makes it a filter rather than an oracle.

## An open invitation

We hold the position in this paper with some confidence and hold several of the questions
around it open. Most of them belong to people who do not work here.

To retail and economic geographers: the central untested question is whether anchor
convergence measured this way predicts anything about *non-retail* uses built nearby.
Everything above concerns where shops are. The reason we care is professional office
tenancy, which is a different market with different drivers, and we have not demonstrated
that a node validated by retail convergence is therefore a good location for an office
building. That is a testable proposition and we have not tested it. We would rather see it
tested by someone with no stake in the answer.

To specialists in spatial clustering: the parameter sensitivity described in Section Four —
a better-than-twofold swing in the North American cluster count across a defensible settings
range — is stated as a caution, but the more useful thing would be a principled way to choose
the settings, or a way of reporting a node's existence that is robust to them. We do not
currently have one, and we would be glad of the argument.

To researchers in volunteered geographic information: the classification inherits whatever
coverage bias the underlying map carries, and inherits it silently. A method for estimating
per-country, per-chain completeness, so that a class assigned in a thinly mapped country
could be qualified rather than presented on the same footing as one in a densely mapped
country, would materially improve this work. The comparable problem in commercial
mobile-location data has had recent attention, and some of it may transfer
[li-2024-safegraph-bias].

To trade-area practitioners: the straight-line bands are an admitted approximation to a real
catchment. Where observed movement data exists, we would like to know how far the band
approximation sits from the observed answer, and whether the gap is systematic enough to
correct for rather than merely to disclose — work redefining catchments from observed
movement rather than distance is the obvious place to start
[calafiore-2022-mobile-geolocation-catchment].

And to anyone who studies retail location behaviour directly: the assumption running under
everything here is that the arrival sequence is real — that a hypermarket establishes a node
and that hardware and warehouse operators follow rather than precede it
[holmes-2011-walmart-diffusion]. We read that pattern from observed site behaviour. Whether
it holds outside North America, and whether it still holds as retail formats change, is a
genuine empirical question that a body of work on chain expansion is better placed to answer
than we are. The classical central-place account of why some settlements support more
functions than others would be the natural frame for asking it
[christaller-1933-central-places].

## Conclusion

Where two or three independently operated national retailers have each committed real
construction capital at the same node, the convergence is evidence a reader can check, and a
forecast is not. That is the discipline this method exists to hold: measure what independent,
well-capitalised parties have already done, from data anyone can download, and refuse to
dress the result up as a prediction. The measurement has real limits — it is backward-looking,
its node count moves with its own settings, its spending layer is a national average applied
uniformly, and its trade areas are circles rather than observed journeys. We would rather
publish those limits beside the method than let a reader discover them later. The method's
worth is not that it is complete. It is that every part of it can be taken apart by somebody
who does not work for us.

## References

Brodsky, I. 2018. *H3: Uber's hexagonal hierarchical spatial index.* Uber Engineering.
[https://www.uber.com/en-US/blog/h3/](https://www.uber.com/en-US/blog/h3/)

Brueckner, J. K. 1993. Inter-store externalities and space allocation in shopping centers.
*Journal of Real Estate Finance and Economics* 7(1): 5–16.

Calafiore, A., Boeing, G., Singleton, A., and Arribas-Bel, D. 2022. Redefining retail
catchment with mobile geolocation data: insights from New Zealand. *Journal of Retailing and
Consumer Services* 79.

Christaller, W. 1933. *Die zentralen Orte in Süddeutschland.* Gustav Fischer.

Ester, M., Kriegel, H.-P., Sander, J., and Xu, X. 1996. A density-based algorithm for
discovering clusters in large spatial databases with noise. *Proceedings of KDD-96*, 226–231.

Haklay, M. 2010. How good is volunteered geographical information? *Environment and Planning
B: Planning and Design* 37(4): 682–703.

Holmes, T. J. 2011. The diffusion of Wal-Mart and economies of density. *Econometrica* 79(1):
253–302.

Hotelling, H. 1929. Stability in competition. *Economic Journal* 39(153): 41–57.

Huff, D. L. 1964. Defining and estimating a trading area. *Journal of Marketing* 28(3): 34–38.

Kwan, M.-P. 2016. Algorithmic geographies: big data, algorithmic uncertainty, and the
production of geographic knowledge. *Annals of the American Association of Geographers*
106(2): 274–282.

Li, Z., Ning, H., Jing, F., and Lessani, M. N. 2024. Understanding the bias of mobile
location data across spatial scales and over time. *PLOS ONE* 19(10): e0294430.

Marshall, A. 1890. *Principles of Economics.* Macmillan.

OpenStreetMap contributors. *Open Database Licence (ODbL) 1.0.*
[https://opendatacommons.org/licenses/odbl/](https://opendatacommons.org/licenses/odbl/)

Overture Maps Foundation. *Open map data — places, buildings, transportation, addresses.*
[https://overturemaps.org/](https://overturemaps.org/)

Pashigian, B. P., and Gould, E. D. 1998. Internalizing externalities: the pricing of space in
shopping malls. *Journal of Law and Economics* 41(1): 115–142.

Reilly, W. J. 1931. *The Law of Retail Gravitation.* Knickerbocker Press.

## Contributors

Prepared by Woodfine Management Corp.

## How this paper was produced

This paper is grounded in the operating and development work the preparing staff do themselves, and in what they have learned from the people they work with routinely: the graphic designers, web developers, and software developers and engineers who build the platform alongside them, and the architects and structural, building-services, and civil engineers they develop buildings with. No outside professional reviewed or approved this paper, and nothing in it is professional advice. It was drafted and edited with AI assistance under editorial direction, and the analysis and conclusions are Woodfine's own.

## Disclosures

Woodfine Capital Projects Inc. ("Woodfine") is the author of record and owns the framework
and the resulting dataset described in this paper; Woodfine Management Corp. maintains the
data and runs the analysis. Woodfine develops and promotes commercial property using this
method to select where it builds, so this paper argues for an approach in which we have a
direct commercial interest. This work was funded internally; no external research funding was
received. Nothing in this paper constitutes an offer to sell, or a solicitation of an offer
to buy, any interest in a Woodfine direct-hold solution; any offering is made only by the
applicable Private Placement Memorandum, which prospective investors should review with their
own professional advisors. Inclusion of any location in the dataset described reflects the
screening criteria discussed and does not indicate acquisition, option, or development
activity, committed or planned, in any market. Some statements above describe planned or
intended future work; language such as "planned," "intended," "targeted," "may," and
"expected" marks this forward-looking content, which is subject to change and does not
constitute a commitment regarding future performance.

## Data and reproducibility

The store, civic, and population layers this method runs on are all openly licensed and can
be obtained directly from their publishers by any reader: the store locations from
OpenStreetMap under the Open Database Licence, which permits commercial use and requires that
derived databases be shared on the same terms; the hospital and university records from the
Overture Maps Foundation's Places dataset under a permissive open data licence; and the
population estimates from an openly licensed gridded population dataset under a licence
requiring only attribution. The per-head spending rates applied to that population are drawn
from the published household expenditure surveys of national statistical agencies. The
classification tests, the four class definitions, and the current pass and fail thresholds
are published on the platform that renders the map, so that a reader with the source data can
reproduce a classification rather than take it on trust. Two figures in this paper come from
sources a reader cannot reconstruct from open data and should treat accordingly: the
retail-productivity estimate named in Section Four, which is a modeled figure from a
commercial location-intelligence provider, and the parameter-sensitivity result, which comes from development sweeps run
against the platform's own pipeline. Coverage grows by ingest rather than arriving complete,
so any count in this paper describes one dated processing run and not a permanent state. No
independent party has audited this dataset, reproduced these results, or reviewed these
claims.

Woodfine Capital Projects™ is a trademark of Woodfine Capital Projects Inc.
