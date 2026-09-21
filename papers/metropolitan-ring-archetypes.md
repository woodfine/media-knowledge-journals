---
schema: journal-v2
slug: metropolitan-ring-archetypes
title: "Two Non-Retail Commercial Archetypes in the Metropolitan Ring"
subtitle: "Why the band around a city holds two different commercial patterns, and what goes wrong when they are read as one"
site: gis.woodfinegroup.com
imprint: WCP-002
thesis: "The ring around a metropolitan core holds two distinct commercial patterns — one organised around people passing through, one around trades and goods movement — and treating them as one category produces worse site decisions than treating them as two."
abstract: |
  Our thesis is that "outside the city centre" is not one place. Two commercial patterns sit
  in the ring around a metropolitan core, they look similar from a distance, and they are
  driven by entirely different things. A Commuter node exists because people drive to it,
  leave a car, and travel onward; its operative variable is the journey, and its most
  reliable commercial marker is a car-rental counter. An Urban Fringe node exists because
  trades and logistics need land, highway access and a labour pool; its operative variable
  is the land, and it is identified partly by what is *absent* — no grocery hypermarket.
  Both are measured from openly licensed map data and both are live classifications: 6,953
  Commuter clusters and 6,368 Urban Fringe clusters, published across seventeen countries
  on the map and drawn from an eighteen-country study geography. The honest complication is
  that the two are not cleanly separated by distance from the city. Commuter nodes sit
  roughly 15 to 150 kilometres out and Urban Fringe nodes roughly 5 to 80; the bands
  overlap across most of their length, and the classification separates the two on what is
  present at the node rather than on how far out it is. We state the ranges rather than
  publish a single boundary figure that would imply a precision the method does not have.
state: draft
version: "0.1.0"
published:
updated: "2026-09-16"
cite_as:
license: CC-BY-4.0
cites:
  - von-thunen-1826-isolated-state
  - christaller-1933-central-places
  - hotelling-1929-stability-in-competition
  - calthorpe-1993-next-american-metropolis
  - cervero-kockelman-1997-travel-demand-3ds
  - cidell-2010-logistics-sprawl-chicago
  - kasarda-lindsay-2011-aerotropolis
  - duranton-puga-2004-agglomeration-microfoundations
  - ester-1996-dbscan
  - haklay-2010-osm-quality
  - kwan-2016-algorithmic-geographies
  - osm-odbl
draws_from:
  - location-intelligence-archetypes
  - commuter
  - urban-fringe
  - retail-centres
  - co-location-methodology
  - gis-data-overview
  - od-catchment-methodology
  - about-regional-markets-system
prepared_by: "Woodfine Management Corp."
keywords:
  - metropolitan fringe
  - commuter belt
  - industrial co-location
  - park and ride
  - site classification
---

> Nothing in this paper constitutes an offer to sell, or a solicitation of an offer to buy,
> any interest in a Woodfine direct-hold solution; any offering is made only by the
> applicable Private Placement Memorandum. Statements marked "planned," "intended,"
> "targeted," "may," or "expected" are forward-looking and subject to change. Full
> disclosures appear at the end of this paper.

Working Paper WCP-002 · v0.1.0 · CC BY 4.0

Our thesis is that the ring of territory around a big city holds two quite different
commercial patterns, that they look alike from a distance, and that anyone who reads them as
one category will make worse decisions than someone who reads them as two. This paper is
about two things that get called the same thing.

The first pattern exists because of a journey. Somewhere between a regional town and the
major city it relates to, there is a point where driving the whole way stops making sense
and driving part of the way, leaving the car, and taking a train or a plane starts making
sense. Commerce accumulates at that point — parking first, then car rental, then hotels,
then the fuel and food that travellers buy. The operative variable is the route, not the
housing around it.

The second pattern exists because of land. Trades contractors, builders' merchants,
industrial suppliers and distribution operators all need large buildings, heavy vehicle
access, and enough population within a half-hour drive to staff a warehouse. They cannot
afford, and do not want, a city-centre address. They settle in the band where land is
cheaper, the motorway is close, and residential streets are far enough away that lorries
are not a planning fight. The operative variable is the land and the access to it.

Both patterns sit in the same broad band of territory. Neither is the retail centre that
most people picture when they think of "the suburbs." Both are live, measured classifications
in this platform's dataset rather than proposals. And the practical stake in telling them
apart is direct: a site that scores well on one pattern's logic can score poorly on the
other's, so a reader who has only one category to think with will read a good site as a bad
one, or the reverse.

## 1. The thesis

The distinction is not a matter of taste. It is a distinction between two different
questions a location can be the answer to.

A Commuter node answers: *where does a journey change mode?* Its value comes from the fact
that a large number of people, on a repeating basis, stop driving and start travelling by
some other means at that point. Everything commercially interesting there — the parking
capacity, the car-rental counter, the hotel, the fuel station — is downstream of that single
behaviour. If the train service is withdrawn, the node loses its reason to exist, however
much land and however good the road access.

An Urban Fringe node answers: *where can a business that needs space, trucks and workers
afford to be?* Its value comes from land economics and highway geometry. Nobody travels
*through* it; they travel *to* it, to buy materials, collect stock, or work a shift. If a
train service arrived tomorrow it would change very little.

Two different questions, two different sets of evidence, two different reasons a site is
worth what it is worth. The urban-economics tradition has been making this kind of
distinction for two centuries — the oldest formal account of why different activities settle
at different distances from a centre reasoned it from the cost of moving goods, which is
exactly the logic that still puts a distribution warehouse where it sits
[von-thunen-1826-isolated-state]. What we are adding is not the observation that the ring is
differentiated. It is a working classification that makes the difference operational: two
separately measured patterns, built from public data, each with its own qualifying evidence
and its own disqualifying evidence, both published on the same map.

## 2. The problem, in the reader's terms

Ask most people what is outside a city and you will get one word: suburbs. It is a single
category covering an enormous variety of places, and its flatness is exactly the problem.

A comparable flatness would be describing every building in a city as "an office." The word
is not wrong. It simply does not distinguish a trading floor from a dental surgery from a
back-office processing centre, and a landlord who thought in that category would make
expensive mistakes about who might lease from them, at what rent, on what lease length, and
what the building would need to have in it.

"The suburbs" is the same kind of category error applied to geography. Inside the ring around
a major metropolitan area there are dormitory towns whose entire commercial life is a
supermarket and a row of shops; there are trade parks where nobody lives and forty
contractors' vans arrive before seven in the morning; there are transit towns where the
morning peak is one direction only and the car park is the largest single land use; and there
are genuine regional centres that happen to be near a big city but do not depend on it. A
reader with one word for all of these has no way to ask the question that actually decides
whether a site is any good, which is: *what is this place for?*

The consequence for a property decision is concrete. Imagine two parcels, both twenty-five
kilometres from a city, both on a main road, both apparently similar. One sits beside a
station where four thousand people leave a car every weekday morning. The other sits beside
a motorway junction between two builders' merchants and a tool-hire depot. The first is worth
what it is worth because of a timetable; the second because of a planning designation and a
slip road. Their tenants are different, their peak hours are different, their vulnerability
is different, and the questions a buyer should ask about each are almost entirely different.
Averaging them into "suburban commercial" destroys the only information that matters.

## 3. Reading a place by what is actually at it

Before the two patterns, the method that finds both — because in each case the classification
works from the same principle, and it is a principle worth stating on its own.

A **cluster**, in this work, is a group of business locations close enough together to be
treated as one commercial node rather than as several separate places. The grouping is done
by a standard density procedure: where enough qualifying locations sit close together, they
form a group; isolated locations are left ungrouped rather than forced into the nearest one
[ester-1996-dbscan]. The locations themselves come from OpenStreetMap, the openly licensed
world map maintained by volunteer contributors, published under the Open Database Licence, and
are matched to chains by a canonical brand identifier rather than by name text so that the
same company resolves consistently across borders [osm-odbl].

What distinguishes the two patterns in this paper from the base retail map is that neither is
identified by a grocery anchor. The platform's base classification finds **Retail Centres** —
the everyday-needs commercial centre built around a grocery hypermarket, with a pharmacy, a
bank branch and casual dining accumulating around it. That pattern organises residential
commercial life almost everywhere, which is precisely why it makes a good base map and a poor
instrument for finding anything else. The two patterns here are overlays: they find market
structures the grocery-anchored map does not capture, and they sit on top of it rather than
replacing it.

Each classification works by naming three sets of evidence in advance and then testing for
them, rather than by scoring a site and setting a cutoff.

**Essential signals** are the conditions without which the pattern does not exist at all. For
a Commuter node, transit that actually reaches a metropolitan destination. For an Urban Fringe
node, a highway interchange within reach of heavy vehicles.

**Significant signals** are the commercial evidence that the pattern is mature rather than
latent — the businesses that only appear once the underlying behaviour is real and repeating.

**Disqualifying signals** are the conditions that rule a site out regardless of how well it
reads on everything else. These do the most work in practice, and they are the part of a
classification that is usually missing. A test with no way to fail is not a test.

Both classifications then sort qualifying nodes into three levels, on the same principle: how
much of the commercial ecosystem that the pattern eventually produces is actually present yet.
The top level is a fully formed node; the middle is a node with direct evidence of the
behaviour but an incomplete commercial ring around it; the bottom is a node where the
underlying infrastructure exists and the commerce has not arrived. The bottom level is, in
both datasets, the largest — which is what you would expect, and a classification that
returned mostly top-level results would be suspect rather than encouraging.

One honest note about all of this, stated once and applying to every figure in the paper.
Counts produced by a clustering procedure are results of the settings chosen, not of a number
of nodes that exists independently in the world; and the underlying volunteer-maintained map
is uneven in coverage between countries and between categories [haklay-2010-osm-quality]
[kwan-2016-algorithmic-geographies]. Every count below describes one dated processing run
under one parameterisation.

## 4. The Commuter pattern: a place defined by a journey

### What the pattern is

A Commuter node sits at the hinge between two markets. On one side is the regional town or
suburb where the people using it live and shop. On the other is the major city they travel
to. The node exists because the journey between them is long enough that driving to a transit
point and parking beats driving the whole way, and short enough that people make the trip
regularly rather than occasionally.

The defining physical feature is not the station. It is the **parking**. A busy urban station
where everyone walks or takes a bus generates almost no commercial opportunity of this kind,
because nobody arrives by car and nobody leaves one. A station where a thousand cars sit all
day is a different animal entirely: it has a land use, a peak flow that requires arterial road
capacity, and a population of travellers with predictable needs at both ends of the day.

The transit that anchors the pattern takes a few forms. Commuter and intercity rail stations —
trains that go *to* a metropolitan centre, as distinct from the metro and tram stops that move
people *within* one. Regional airports and transit hubs serving mostly domestic and short-haul
routes. Park-and-ride facilities, which are the purest form of the pattern because they are
nothing but the car-to-transit transition itself. And highway-exit commercial: the fuel, food
and convenience retail that serves drive-to travellers at the interface.

### The evidence that says the pattern is real

The essential conditions are a regional transit anchor within three kilometres with direct
service to a metropolitan centre; a metropolitan separation in a band running roughly 15 to
150 kilometres; a qualifying retail centre of the upper two levels within ten kilometres, being
the regional market whose residents generate the parking demand; multi-lane road access within
a kilometre, because a car park that fills and empties twice a day needs arterial capacity; and
a regional population of at least 150,000.

The separation band deserves its own paragraph, because the shape of it is the argument. Under
about fifteen kilometres, the pattern does not form: the destination is close enough that
driving all the way beats parking and transferring, and the place is a suburb rather than a
commuter origin. Between roughly fifteen and a hundred kilometres is where the pattern is
strongest — a one- to two-hour drive, where transit saves meaningful time. Between a hundred
and a hundred and fifty it still works where the transit is fast enough, a high-speed line or a
direct flight. Beyond about a hundred and fifty kilometres a place is generally a standalone
market with a relationship to a different centre, or with none.

The commercial evidence that a node has matured is more specific, and the strongest single
marker is one most people would not guess: **car rental**. A car-rental counter within a
kilometre is the highest-confidence commercial signal in the whole classification, because a
rental counter is a business that only makes sense where a substantial number of people
arrive at a place without a car and need one. Nobody opens one on a hunch. A hotel cluster
within five hundred metres is the second marker — business travel, and the multi-day parking
that comes with it. A second, genuinely distinct transit mode within five kilometres — rail
plus an airport, rather than two kinds of rail — marks the highest-value sites.

And the disqualifying conditions: a major international airport within fifteen kilometres, a
population under a hundred thousand, or no direct service to a major metropolitan centre.

### Two design decisions worth explaining

Two parts of this classification exist to stop it from fooling itself, and both are worth
naming because they are the sort of thing that is usually left implicit.

The first is how transit modes are counted. A station offering both intercity and local
commuter rail from the same platform is one kind of transit, not two. Counting it as two would
make an ordinary station look like a multi-modal interchange. Modes are therefore collapsed
into four groups — air, rail, urban transit, and bus — and a genuine multi-modal hub has to
show distinct groups, not two flavours of the same one.

The second is the major-hub filter. The very largest international airports generate their own
retail gravity: people go there to fly, and the commerce around them is airport commerce, not
park-and-travel commerce. Transit anchors sitting beside a top-level retail cluster are
therefore reviewed as likely major commercial hubs, and the filter removes the obvious cases —
the largest airports in Los Angeles, New York, London and Paris among them. The airport-centred
development literature treats those places as a category of their own for exactly this reason
[kasarda-lindsay-2011-aerotropolis].

### Where the classification stands

Commuter classification is production-grade. Park-and-ride records — 23,117 of them — serve as
the primary geographic anchor, which is a deliberate choice: they are the actual car-to-transit
transition points, and they are distributed independently of where the rail network happens to
run, so anchoring on them avoids inheriting the shape of the railway as if it were the shape of
the demand.

The current dataset holds **6,953 clusters across seventeen countries** on the map. Of those,
691 — just under a tenth — reach the top level, combining multiple transit modes with a full
commercial ecosystem. 2,658, a little under two-fifths, sit at the middle level with transit
plus at least one commercial signal. The remaining 3,604, a little over half, have transit
present and the commercial opportunity unproven.

Rail stations dominate across every country in the set. The European habit of driving to a
train rather than to a plane means intercity and commuter rail sites substantially outnumber
airport sites there, and a railway station serving a regional city is a reliable candidate
almost wherever regional service reaches one. The relationship between transit provision and
the commercial development that follows it has been studied for decades, most systematically
in the transit-oriented-development tradition [calthorpe-1993-next-american-metropolis]
[cervero-kockelman-1997-travel-demand-3ds]; what this classification adds is a way of locating
the cases from open data at continental scale rather than one corridor at a time.

Two capabilities named in the design are planned and not built: airport passenger-volume data,
intended to replace the current adjacency-based hub filter with a direct traffic-based test,
and a directory of the parking operators active in each market.

## 5. The Urban Fringe pattern: a place defined by land and access

### What the pattern is

An Urban Fringe node sits in the transition zone where a metropolitan area's continuous
built-up fabric gives way to industrial land and open ground. Its tenants are not serving
households doing a weekly shop. They are serving trades and goods movement: big-box hardware
and home-improvement warehouses, builders' merchants and trade counters, industrial
maintenance and repair suppliers selling fasteners and tools and consumables, tool-hire
depots, regional distribution hubs and last-mile sortation operations, auto-parts and
flooring and tile supply.

The single most useful thing to know about this pattern is that it is partly defined by an
**absence**. Where a retail centre is organised around a grocery hypermarket, an Urban Fringe
node is identified by the hypermarket *not* being there. Grocery anchors, lifestyle anchors
and consumer price clubs in their retail role are what the pattern is not. That negative test
is what keeps the classification from simply re-finding the retail map with extra steps.

The spatial signature is consistent and recognisable from a car window: the metropolitan ring,
along multi-lane arterial roads, clustered around motorway interchanges with direct truck
access, on land zoned industrial or light industrial with more of the same next door. The built
form spans the single-storey retail warehouse and the multi-storey light-industrial and
distribution building, and both depend on the same two things — the junction and the labour
catchment.

### The evidence

The essential conditions are a highway interchange within two kilometres, because heavy goods
vehicles cannot be routed down residential streets; industrial land use adjacent or within five
hundred metres, for zoning compatibility and for the supplier ecosystem that already sits
there; a labour catchment of 300,000 or more people within a thirty-minute drive, because
retail, distribution and trade roles all need staff who can actually get to work; and, where it
exists, freight rail access within two kilometres.

The value-adding conditions are an air-cargo airport within twenty kilometres, for the
electronics and components that move by air; a logistics hub within five kilometres, for shared
last-mile infrastructure; and a transit corridor within five hundred metres, so that staff
without cars can reach the site.

The disqualifying conditions are as informative as the qualifying ones. Dense residential
immediately adjacent rules a site out, because the truck traffic will eventually become a
planning fight the operator loses. A flood plain rules it out, because the capital at risk is
large and the insurance is prohibitive. A heritage or environmentally protected designation
rules it out, on height and access grounds. And a location inside an existing retail centre
cluster rules it out, because that is the wrong land use entirely — it is the grocery-anchored
consumer pattern wearing similar clothes.

### One rule that does most of the work

Levels here are assigned on the number of *distinct trade-supply categories* present, not on
how many businesses are in the cluster. A node with six hardware stores and nothing else does
not reach the top level. A node with a hardware anchor and an industrial-supply distributor
does, because two distinct categories indicate a genuine contractor and logistics ecosystem
rather than a single-category commercial strip that happens to have repeated itself.

This is the same reasoning that runs through the retail work: independent categories are
evidence, and repetition within one category is not. It also explains the shape of the results.
A full trade hub combining industrial supply, tool hire, a builders' merchant and auto parts is
legitimately rare, so a classification that found them everywhere would be measuring something
other than what it claims to.

### Where the classification stands

Urban Fringe classification is production-grade. Hardware stores — 10,338 locations across 45
chains — were profiled as the proxy anchor for the pattern, and the grouping rules were
validated before promotion to production: across the top two levels, 73.4 per cent of clusters
showed genuine hardware co-location, against an acceptance threshold set in advance at 55 per
cent.

The current dataset holds **6,368 clusters** across the eighteen-country study geography. 852
of them, a little over a tenth, reach the top level as full trade hubs. 1,327, about a fifth,
sit at the middle level. The remaining 4,189 — very nearly two-thirds — are emerging or thin.

The geographic concentration is heavily American: the United States accounts for 2,207
clusters, or 34.7 per cent of the total, followed by Germany at 848 (13.3 per cent), France at
612 (9.6 per cent), Mexico at 321 (5.0 per cent), Italy at 287 (4.5 per cent), the United
Kingdom at 263 (4.1 per cent), and the Netherlands at 198 (3.1 per cent). The remaining
eleven countries in the study carry 1,632 between them, just over a quarter of the total, and
are not individually broken out in the current source data. The concentration of freight and
distribution activity in particular metropolitan rings, and its movement outward over time, is
a documented phenomenon in its own right [cidell-2010-logistics-sprawl-chicago].

One finding is worth reporting because it complicates the neat picture above. In 3,048
clusters — 47.9 per cent, nearly half — a grocery hypermarket does sit within a kilometre of
the cluster centre. These are flagged separately rather than excluded. They are dual-use
commercial parks: genuine trade-supply co-locations that also happen to include grocery
retail, which is a common arrangement in Europe, where industrial parks and retail parks
frequently share the same access roads. The absence rule that defines the pattern operates
within the cluster, not over the whole neighbourhood, and nearly half the dataset sits in that
grey area.

## 6. Where the two patterns meet, and what is not yet settled

The cleanest version of this paper would give you a distance at which one pattern ends and the
other begins. We are not going to, because the data does not support one.

The Commuter band runs roughly 15 to 150 kilometres from a metropolitan centre. The Urban
Fringe band runs roughly 5 to 80. Those are the ranges the two classifications work in, and
they overlap across most of their length — from about fifteen kilometres out to about eighty,
either pattern can occur, and both can occur in the same town. There is no single boundary
figure to publish, and publishing one would imply a precision that does not exist.

That is not an evasion; it is the actual finding. The two patterns are not separated by
distance. They are separated by what is at the node. A site with a station, a full car park and
a rental counter is a Commuter node whether it is at twenty kilometres or a hundred. A site
with a motorway junction, a builders' merchant and an industrial designation is an Urban Fringe
node at the same distances. The distance bands describe where each pattern is *likely* to be
found; the qualifying and disqualifying evidence decides what a given node actually is. Where
work of this kind resolves the ambiguity by drawing a line on a map, it is usually a convenient
line rather than an observed one.

Two further unsettled points belong here rather than in a separate section. The country counts
differ between the two classifications and between the map and the underlying study: seventeen
countries are displayed on the map, and the study geography behind the Urban Fringe figures
covers eighteen. The difference is real, not a typographical drift, and each figure above is
labelled with the set it belongs to. And both datasets inherit the coverage unevenness of the
underlying open map: a country whose trade counters and park-and-ride sites are thinly mapped
will appear to have fewer nodes than it has.

## What this changes for the reader

The first change is a question. Comparing two sites in the ring around a city, a reader now has
something specific to ask instead of a general impression: *which pattern does this site
actually serve?* The answers diverge immediately. If it is a Commuter node, the questions are
about the timetable, the car park's capacity and ownership, and whether the service that
creates the demand is secure. If it is an Urban Fringe node, the questions are about the
planning designation, the junction, and whether residential development is creeping toward the
truck route.

The second change is what counts as evidence of maturity. A Commuter node with transit and no
car rental and no hotel is a node where the behaviour may exist but the commerce has not
followed — two-thirds of the current Commuter dataset is in exactly that state. An Urban
Fringe node with hardware retail and nothing else is the same story in a different pattern.
Neither is bad news; both are a specific, checkable statement about how far along a place is,
and that is a more useful thing to hold than an impression.

The third is a caution against the composite. It would be straightforward to merge these two
classifications into one "metropolitan ring" score, and the result would be worse than either.
The signals are not interchangeable: a rental counter says nothing about whether trucks can
reach a site, and a motorway junction says nothing about whether anyone will leave a car there
all day. Adding them together would produce a number that is high for two incompatible reasons
and would tell a reader neither of them.

The trade-offs are real. Both classifications find what is already there and therefore find a
place after it has formed, not before. Both depend on an open map whose completeness varies by
country. Both report counts that are results of a clustering parameterisation rather than
counts of things in the world. And the honest overlap in Section Six means a reader cannot
infer the pattern from a distance figure alone — they have to look at what is at the node,
which is more work than reading a number.

## An open invitation

Several of the questions this work raises belong to fields we do not work in, and we would
rather ask them than answer them badly.

To urban geographers and regional scientists: the direct question is whether two is the right
number. We have described two non-retail patterns in the ring, and it is entirely possible that
one of them is concealing a third. The Urban Fringe category currently holds both the
trade-supply cluster serving contractors and the pure distribution and last-mile operation
serving goods movement, and those may be different enough in their land economics, their
labour demand and their locational logic to warrant separating. Nearly half the current
dataset also sits in the dual-use grey area described in Section Five, which is either an
acceptable messiness or a sign that the negative test is drawn in the wrong place. We do not
know which, and the underlying question — how many distinct agglomeration mechanisms are
actually operating in a given band — is one the agglomeration literature is better equipped to
answer than we are [duranton-puga-2004-agglomeration-microfoundations].

To transport geographers: the car-rental marker is doing a great deal of work in the Commuter
classification, and we adopted it because it is a business that only makes sense where the
underlying behaviour is real. We have not validated it against observed passenger flows. If
that marker is systematically biased — toward airports over rail, toward business travel over
commuting, toward one country's rental market structure over another's — we would like to know
before it is relied on further. A validation against real boarding or parking-occupancy data,
in even one corridor, would be worth more than any amount of further refinement of the
classification itself.

To planners working on the fringe: the disqualifying condition "dense residential immediately
adjacent" is stated as a static test, and the real phenomenon is dynamic. Residential
development advances toward industrial land over years, and the point at which a trade park
becomes untenable is a planning and political process, not a distance. How that encroachment
should be represented in a classification that is rebuilt on a data cadence is an open design
question, and the people who have watched it happen in a particular region will know things
this method cannot see.

And to anyone working on settlement hierarchy: both patterns here are defined relative to a
"metropolitan centre" drawn from a reference set, and that reference set is a choice. Which
places count as centres, and whether a town's relationship should be measured to the nearest
one or to the one it actually functions with, is the oldest open question in this subject and
we have adopted a working answer rather than solved it [christaller-1933-central-places].

## Conclusion

"Outside the city centre" is two places, not one. A Commuter node is organised around a
journey and identified by parking, transit and the commerce that serves travellers. An Urban
Fringe node is organised around land and access and identified by trades, logistics and the
absence of a grocery anchor. Both are measured here from open map data, both are live
classifications rather than proposals, and both report their level honestly — in each case the
largest group is the one where the infrastructure exists and the commerce has not yet arrived.
The two overlap in distance from the city and separate on what is actually at the node, which
is why we publish the ranges rather than a boundary. The useful discipline is not the
classification itself. It is the habit of asking what a place is *for* before asking what it is
worth.

## References

Calthorpe, P. 1993. *The Next American Metropolis: Ecology, Community, and the American
Dream.* Princeton Architectural Press.

Cervero, R., and Kockelman, K. 1997. Travel demand and the 3Ds: density, diversity, and
design. *Transportation Research Part D* 2(3): 199–219.

Christaller, W. 1933. *Die zentralen Orte in Süddeutschland.* Gustav Fischer.

Cidell, J. 2010. Concentration and decentralization: the new geography of freight distribution
in US metropolitan areas. *Journal of Transport Geography* 18(3): 363–371.

Duranton, G., and Puga, D. 2004. Micro-foundations of urban agglomeration economies.
*Handbook of Regional and Urban Economics*, vol. 4. Elsevier.

Ester, M., Kriegel, H.-P., Sander, J., and Xu, X. 1996. A density-based algorithm for
discovering clusters in large spatial databases with noise. *Proceedings of KDD-96*, 226–231.

Haklay, M. 2010. How good is volunteered geographical information? *Environment and Planning
B: Planning and Design* 37(4): 682–703.

Hotelling, H. 1929. Stability in competition. *Economic Journal* 39(153): 41–57.

Kasarda, J. D., and Lindsay, G. 2011. *Aerotropolis: The Way We'll Live Next.* Farrar, Straus
and Giroux.

Kwan, M.-P. 2016. Algorithmic geographies: big data, algorithmic uncertainty, and the
production of geographic knowledge. *Annals of the American Association of Geographers* 106(2):
274–282.

OpenStreetMap contributors. *Open Database Licence (ODbL) 1.0.*
[https://opendatacommons.org/licenses/odbl/](https://opendatacommons.org/licenses/odbl/)

Von Thünen, J. H. 1826. *Der isolierte Staat in Beziehung auf Landwirtschaft und
Nationalökonomie.* Perthes.

## Contributors

Prepared by Woodfine Management Corp.

## How this paper was produced

This paper is grounded in the preparing staff's own development and operating work, and in their standing engagement with the designers, software engineers, architects, engineers, and legal and accounting advisers the business works with. It was drafted and edited with AI assistance under editorial direction, and the analysis and conclusions are the author's own.

## Disclosures

Woodfine Capital Projects Inc. ("Woodfine") is the author of record and owns the framework and
the resulting dataset described in this paper; Woodfine Management Corp. maintains the data and
runs the analysis. Woodfine develops and promotes commercial property and uses these
classifications in deciding where to build, so this paper argues for an approach in which we
have a direct commercial interest. This work was funded internally; no external research
funding was received. Nothing in this paper constitutes an offer to sell, or a solicitation of
an offer to buy, any interest in a Woodfine direct-hold solution; any offering is made only by
the applicable Private Placement Memorandum, which prospective investors should review with
their own professional advisors. Inclusion of any location in the datasets described reflects
the screening criteria discussed and does not indicate acquisition, option, or development
activity, committed or planned, in any market. Some statements above describe planned or
intended future work; language such as "planned," "intended," "targeted," "may," and "expected"
marks this forward-looking content, which is subject to change and does not constitute a
commitment regarding future performance.

## Data and reproducibility

The business and transport locations behind both classifications come from OpenStreetMap under
the Open Database Licence, which anyone may download and use commercially, on terms requiring
that a derived database be shared on the same basis. Chains are matched by a canonical brand
identifier rather than by name text, so that the same company resolves consistently across
borders and languages. All counts in this paper — 6,953 Commuter clusters and 6,368 Urban
Fringe clusters, their level splits, the 23,117 park-and-ride records, the 10,338 hardware
locations across 45 chains, the 73.4 per cent co-location validation against a 55 per cent
acceptance threshold set in advance, and the country shares in Section Five — are drawn from
the platform's current production build and describe one dated processing run. They are not a
live feed and they are not stable: the dataset is rebuilt on a processing cadence, coverage
grows as new chain data is ingested, and a count produced under different clustering settings
would be a different count on identical underlying data. The proximity thresholds quoted
throughout are the classifications' own published qualifying conditions. Distances are
straight-line measurements, not drive times, except the labour-catchment condition in Section
Five, which is stated as a thirty-minute drive. No independent party has audited these
datasets, reproduced these figures, or reviewed these claims.

MCorp™ and Woodfine Capital Projects™ are trademarks of Woodfine Capital Projects Inc.
