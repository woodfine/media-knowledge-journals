---
schema: journal-v2
slug: regional-markets-europe-rankings
title: "The 400 Published Regional Markets in Europe"
subtitle: "The full list across fifteen countries, with the metropolitan reference point and cluster composition for every entry"
site: gis.woodfinegroup.com
imprint: WCP-006
thesis: "This is the complete European published set — 400 markets drawn from a 650-market qualifying pool across fifteen countries — published in full, by country, with no rank and no score, because none is published."
abstract: |
  This is the data companion to the Regional Markets methodology paper: the full published
  European set, 400 named markets drawn from a qualifying pool of 650 across fifteen
  countries. For each market it gives the metropolitan centre the market is measured against,
  the straight-line distance to it, and how many co-location clusters of each composition
  tier the market carries. It does not re-argue the qualification method, which is the
  methodology paper's subject. Two things this table is not: it is not a ranking, because no
  rank or score is published for any market and the tables are simply sorted by reference
  distance so that they can be read; and it is not investment advice about any listed location. Two coverage facts belong up front and are
  different in kind. Germany, France and the Netherlands are excluded from the current
  European methodology by a deliberate scope decision, not a data gap. Separately, catchment
  population is genuinely absent for 141 of the 400 entries and consumer-spend figures for
  178 — real gaps in the underlying census and spend sources, disclosed rather than filled
  with a zero.
state: draft
version: "0.1.0"
published:
updated: "2026-09-16"
cite_as:
license: CC-BY-4.0
cites:
  - osm-odbl
  - overture-maps
  - ester-1996-dbscan
  - haklay-2010-osm-quality
draws_from:
  - atlas-top-400-europe
  - atlas-italy
  - atlas-spain
  - atlas-united-kingdom
  - atlas-poland
  - atlas-sweden
  - atlas-czechia
  - atlas-finland
  - atlas-hungary
  - atlas-slovakia
  - atlas-romania
  - atlas-bulgaria
  - atlas-denmark
  - atlas-croatia
  - atlas-norway
  - atlas-greece
  - about-regional-markets-system
  - co-location-methodology
prepared_by: "Woodfine Management Corp."
keywords:
  - regional markets
  - Europe
  - published dataset
  - anchor composition
  - site selection
---

# The 400 Published Regional Markets in Europe

*The full list across fifteen countries, with the metropolitan reference point and cluster composition for every entry*

> Nothing in this paper constitutes an offer to sell, or a solicitation of an offer to buy,
> any interest in a Woodfine direct-hold solution; any offering is made only by the
> applicable Private Placement Memorandum. Statements marked "planned," "intended,"
> "targeted," "may," or "expected" are forward-looking and subject to change. Full
> disclosures appear at the end of this paper.

Working Paper WCP-006 · v0.1.0 · CC BY 4.0

This paper publishes the complete European Regional Markets set: four hundred named markets
that clear the anchor-composition gates, drawn from a qualifying pool of 650 across fifteen
countries. It is a data companion, not an argument. The reasoning behind the qualification
method — why anchor composition rather than population, and why the published set is
deliberately smaller than the qualifying pool — belongs to the methodology paper and is not
restated here beyond what a reader needs to read the tables.

Two statements about what this is not, before anything else.

**It is not a ranking.** No rank and no score is published for any market in this set. The
tables below are sorted by reference distance within each country purely so they can be read,
and no market-to-market comparison is published or implied. A composite measure exists
internally to support the selection; it is not published and has no bearing on how any market is described here.

**It is not advice about any listed location.** A market's presence in this set means that
independent large-format retailers have converged there in a qualifying combination. It is not
a forecast about that market, not a recommendation, and not an indication that anything has
been acquired, optioned, or developed there or anywhere near it.

The two continental sets are produced and selected as two separate series, not as one combined
list. A European market's presence here is a statement about its standing against the European
pool, and no comparison with a North American entry is intended or supported.

## 1. How a market enters this set

A Regional Market is a named municipality whose name differs from that of its metropolitan
reference point, and whose retail co-location clusters, taken together, satisfy an
anchor-composition test.

A market qualifies under one of three gates. A **Regional Market** carries a hypermarket anchor
plus at least two of hardware, price club, lifestyle, electronics or sport, combined across all
of the market's member clusters. A **District Anchor** carries a hypermarket and a hardware
anchor with no other optional category, across at least two distinct clusters. A **Standalone
Regional Centre** meets that same condition in a market isolated from any other qualifying
market beyond the outer geographic band.

Of the four hundred European entries, 399 qualify as Regional Markets and exactly one as a
District Anchor. No European entry qualifies as a Standalone Regional Centre — Europe's
settlement geography does not produce the genuinely isolated regional centre that the
standalone gate exists to catch, and which accounts for eighteen of the North American
entries.

A geographic coherence constraint applies: all of a settlement's member clusters must lie
within a 200-kilometre bounding box. Settlements failing it are name-collision aggregations and
are excluded rather than treated as one very large market.

Selection from the qualifying pool takes the four hundred markets with the strongest anchor
composition per continent, with no per-country budget. A small per-country minimum floor
prevents a country with genuine qualifying markets from being excluded outright and otherwise
does not affect which markets are included. The per-country counts are therefore an observed
result of one continental cutoff, not a quota set in advance.

Catchment population and consumer-spend figures accompany each market in the underlying data as
descriptive context. They take no part in selection. Population is negatively correlated with
the composition measure in every country tested, so selecting on population would systematically
replace genuine regional markets with dense metropolitan-fringe suburbs.

**Germany, France and the Netherlands are excluded from the current European methodology**
under a scope decision locked on 30 June 2026. This is deliberate, not a data gap, and it is
the reason an earlier eleven-country version of this set that included them has been
superseded.

## 2. How to read the table

**Market** is the municipality's own name.

**Metropolitan reference** is the nearest major metropolitan centre in the framework's
continental reference set. It is a descriptive anchor, not a relationship: naming a centre
beside a market is not a claim that the market functions as a commuter suburb of it. For several
countries the nearest reference point lies outside the country's own borders, which is why some
national median distances are large.

**km** is the straight-line distance from the market to that centre. It is not a drive time and
not a commuting estimate, and it is recorded rather than gated — distance takes no part in
whether a market qualifies. A distance term was present in an earlier iteration of the selection
method and was removed, because it caused standalone secondary cities to outrank genuine suburbs
of major metropolitan areas.

**T1**, **T2** and **T3** are counts of the market's co-location clusters at each composition
tier. In Europe, a **Tier 1** cluster contains a hypermarket anchor alongside a hardware anchor
and at least one further anchor category. A **Tier 2** cluster contains a hypermarket and a
hardware anchor. A **Tier 3** cluster contains a single recognised anchor. A market may carry
clusters at more than one tier; the figures are counts of clusters, not of stores.

European Tier 1 compositions differ from North American ones by anchor identity rather than by
structure. In Central European markets the combination is typically anchored by a Kaufland or
Globus hypermarket, a Hornbach or Bauhaus hardware anchor, and a MediaMarkt or Saturn
electronics anchor. In the United Kingdom a Tesco Extra or Sainsbury's superstore fills the
hypermarket position, with Wickes or B&Q as the hardware anchor.

## 3. Country summary

| Country | Published markets | Qualifying pool | T1 | T2 | T3 | Median reference distance |
|---|---|---|---|---|---|---|
| Italy | 62 | 108 | 57 | 2 | 37 | 63 km |
| Spain | 55 | 79 | 53 | 2 | 13 | 77 km |
| United Kingdom | 55 | 161 | 58 | 9 | 24 | 37 km |
| Poland | 55 | 75 | 60 | 3 | 5 | 70 km |
| Sweden | 32 | 39 | 32 | 6 | 4 | 136 km |
| Czechia | 27 | 45 | 21 | 1 | 14 | 64 km |
| Finland | 19 | 21 | 18 | 3 | 4 | 141 km |
| Hungary | 19 | 19 | 19 | 0 | 4 | 95 km |
| Slovakia | 16 | 24 | 13 | 0 | 6 | 84 km |
| Romania | 13 | 15 | 11 | 2 | 2 | 100 km |
| Bulgaria | 11 | 11 | 11 | 0 | 0 | 79 km |
| Denmark | 11 | 26 | 11 | 4 | 0 | 57 km |
| Croatia | 9 | 11 | 12 | 2 | 2 | 189 km |
| Norway | 9 | 9 | 8 | 1 | 3 | 107 km |
| Greece | 7 | 7 | 4 | 1 | 3 | 138 km |
| **Total** | **400** | **650** | **388** | **36** | **121** | — |

Italy leads on published markets at 62, but the United Kingdom has by far the deepest
qualifying pool at 161 — the widest gap between qualifying and published anywhere in the set.
Hungary, Bulgaria, Norway and Greece publish their entire qualifying pool, having no markets
held back by the cap at all.

## 4. Composition and geography

The four hundred markets carry 545 co-location clusters between them — 388 Tier 1, 36 Tier 2
and 121 Tier 3 — an average of 1.36 clusters per market. Tier 1 presence is close to universal:
358 of the four hundred carry at least one Tier 1 cluster, and 28 qualify on Tier 3 clusters
alone.

European markets carry fewer clusters each than North American ones — 1.36 against 1.77 — and
that difference should not be read as a difference in market strength. European municipalities
are considerably smaller geographic units than United States incorporated places, so a European
settlement typically contains fewer clusters even where the underlying retail density per square
kilometre is comparable. The unit of measurement differs; the retail geography need not.

The set spans 108 distinct metropolitan reference points. Stockholm is the reference for 16
entries, Budapest for 13, and Košice and Milan for 10 each. Tampere carries nine, and Brno,
Gliwice and Madrid eight each.

Recorded reference distances run from 12 to 467 kilometres, with a median of 74. A little over
half the set — 232 of 400 — sits within 80 kilometres of its reference point, and 46 sit beyond
150. The long tail is concentrated in countries whose nearest reference point lies outside their
own borders: Croatia's median reference distance is 189 kilometres, Finland's 141 and Sweden's
136.

## 5. Catchment data coverage

Catchment population is recorded for 259 of the four hundred European markets and is absent for
the remaining 141. Sweden, Finland, Romania, Bulgaria, Croatia and Norway carry no catchment
population for any market at all. Consumer-spend coverage is thinner still: absent for 178
markets, with partial gaps in Italy and Spain as well.

These are disclosed gaps in the underlying census and spend source data, not omissions in this
list, and they are stated as gaps rather than filled with a zero. A market without a catchment
figure has no catchment figure; it does not have a catchment of nothing. The North American set
has no gaps of this kind, so a reader comparing coverage between the two continents is comparing
source availability rather than market quality.

## 6. The markets

Listed by country, and within each country in ascending order of reference distance. That
sort is descriptive, not ordinal: no rank or score is published for any entry, and a market's
position in a table says nothing about it beyond how far it sits from the centre named beside
it.

### Italy — 62 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Rivalta di Torino | Turin | 13.7 | 1 | 0 | 1 |
| Carugate | Milan | 14.7 | 1 | 0 | 0 |
| Prato | Florence | 17.9 | 1 | 0 | 2 |
| Cerro Maggiore | Milan | 24.2 | 1 | 0 | 0 |
| Caserta | Naples | 24.4 | 1 | 0 | 0 |
| Empoli | Florence | 25.8 | 1 | 0 | 0 |
| Chioggia, Venezia | Venice | 27.6 | 1 | 0 | 0 |
| Molfetta | Bari | 28.4 | 1 | 0 | 0 |
| Cernusco Lombardone | Milan | 30.0 | 1 | 0 | 0 |
| Padova | Venice | 31.9 | 1 | 0 | 0 |
| Mantova | Verona | 33.8 | 1 | 0 | 1 |
| Milazzo | Messina | 35.4 | 1 | 0 | 0 |
| Villesse | Trieste | 36.1 | 1 | 0 | 0 |
| Modena | Bologna | 37.8 | 3 | 0 | 0 |
| Gioia Tauro | Messina | 39.7 | 1 | 0 | 0 |
| Montecatini-Terme | Florence | 40.5 | 1 | 0 | 0 |
| Curno | Milan | 41.2 | 1 | 0 | 0 |
| Ferrara | Bologna | 42.1 | 0 | 1 | 1 |
| Novara | Milan | 43.7 | 1 | 0 | 2 |
| Asti | Turin | 44.6 | 1 | 1 | 0 |
| Faenza | Bologna | 48.3 | 1 | 0 | 1 |
| San Vendemiano | Venice | 51.5 | 1 | 0 | 0 |
| Benevento | Naples | 52.5 | 1 | 0 | 1 |
| Voghera | Milan | 53.6 | 0 | 0 | 2 |
| Castelletto sopra Ticino | Milan | 53.7 | 1 | 0 | 0 |
| Arezzo | Florence | 59.7 | 1 | 0 | 1 |
| Biella | Turin | 61.4 | 1 | 0 | 0 |
| Brescia | Verona | 61.8 | 2 | 0 | 1 |
| Alessandria | Genoa | 62.2 | 0 | 0 | 2 |
| Reggio nell'Emilia | Bologna | 62.4 | 0 | 0 | 2 |
| Piacenza | Milan | 62.9 | 1 | 0 | 1 |
| Vercelli | Milan | 62.9 | 1 | 0 | 0 |
| Forlì | Bologna | 65.2 | 3 | 0 | 0 |
| San Benedetto del Tronto | Ancona | 66.0 | 1 | 0 | 0 |
| Tavagnacco | Trieste | 67.0 | 1 | 0 | 1 |
| Viterbo | Rome | 67.4 | 1 | 0 | 0 |
| Pisa | Florence | 68.8 | 0 | 0 | 2 |
| Pesaro | Ancona | 73.7 | 1 | 0 | 1 |
| Cremona | Milan | 74.1 | 1 | 0 | 0 |
| Terni | Rome | 74.3 | 1 | 0 | 0 |
| Cuneo | Turin | 77.1 | 0 | 0 | 2 |
| Livorno | Florence | 78.3 | 1 | 0 | 0 |
| Saint-Christophe | Turin | 78.4 | 1 | 0 | 0 |
| Taranto | Bari | 78.4 | 0 | 0 | 2 |
| Perugia | Ancona | 79.8 | 0 | 0 | 3 |
| Belluno | Venice | 81.6 | 0 | 0 | 1 |
| Parma | Bologna | 87.4 | 2 | 0 | 1 |
| Bolzano/Bozen | Innsbruck (Austria) | 87.5 | 1 | 0 | 1 |
| L'Aquila | Rome | 88.2 | 1 | 0 | 1 |
| Campobasso | Naples | 88.5 | 1 | 0 | 0 |
| Foggia | Potenza | 92.2 | 1 | 0 | 0 |
| Savignano sul Rubicone | Bologna | 94.1 | 1 | 0 | 1 |
| Brindisi | Bari | 103.2 | 0 | 0 | 1 |
| Grosseto | Florence | 111.3 | 0 | 0 | 1 |
| Catanzaro | Messina | 118.2 | 1 | 0 | 0 |
| San Giovanni Teatino | Ancona | 122.3 | 1 | 0 | 0 |
| Corigliano-Rossano | Potenza | 128.5 | 1 | 0 | 1 |
| Surbo | Bari | 135.4 | 1 | 0 | 0 |
| Termoli | Naples | 140.1 | 1 | 0 | 0 |
| Cosenza | Messina | 143.4 | 1 | 0 | 0 |
| Sassari | Toulon (France) | 342.6 | 1 | 0 | 0 |
| Cagliari | Palermo | 389.3 | 1 | 0 | 0 |

### Spain — 55 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Sant Boi de Llobregat | Barcelona | 12.1 | 1 | 0 | 0 |
| Alcorcón | Madrid | 15.1 | 1 | 0 | 0 |
| San Sebastián de los Reyes | Madrid | 16.2 | 1 | 0 | 0 |
| Rivas-Vaciamadrid | Madrid | 16.4 | 1 | 0 | 0 |
| Pinto | Madrid | 17.0 | 1 | 0 | 0 |
| Torrejón de Ardoz | Madrid | 20.2 | 0 | 0 | 2 |
| Elche | Alicante | 21.7 | 1 | 0 | 0 |
| Narón | A Coruña | 22.3 | 1 | 0 | 0 |
| Jerez de la Frontera | Cádiz | 22.4 | 1 | 0 | 1 |
| Gijón | Oviedo | 23.3 | 1 | 0 | 1 |
| Durango | Bilbao | 26.4 | 1 | 0 | 0 |
| Fuengirola | Málaga | 27.4 | 1 | 0 | 0 |
| Alcalá de Henares | Madrid | 31.0 | 1 | 0 | 0 |
| Villajoyosa | Alicante | 33.8 | 1 | 0 | 0 |
| Vilanova i la Geltrú | Barcelona | 40.9 | 1 | 0 | 0 |
| Cocentaina | Alicante | 41.8 | 1 | 0 | 0 |
| Palencia | Valladolid | 42.4 | 1 | 0 | 0 |
| Motril | Granada | 48.9 | 1 | 0 | 0 |
| Orihuela | Alicante | 50.7 | 1 | 0 | 0 |
| Santiago de Compostela | A Coruña | 53.7 | 1 | 0 | 1 |
| Xàtiva | Valencia | 54.3 | 1 | 0 | 0 |
| Vic | Barcelona | 61.9 | 1 | 0 | 0 |
| Castelló de la Plana | Valencia | 62.7 | 1 | 0 | 1 |
| Huesca | Zaragoza | 66.0 | 1 | 0 | 0 |
| Talavera de la Reina | Toledo | 67.8 | 1 | 0 | 0 |
| Jaén | Granada | 69.5 | 1 | 0 | 0 |
| Murcia | Alicante | 70.4 | 1 | 1 | 1 |
| Santander | Bilbao | 77.4 | 1 | 0 | 0 |
| Lugo | A Coruña | 78.6 | 1 | 0 | 0 |
| Girona | Barcelona | 83.5 | 1 | 0 | 0 |
| Tarragona | Barcelona | 84.6 | 1 | 0 | 0 |
| Los Barrios | Cádiz | 85.3 | 1 | 0 | 0 |
| Ávila | Madrid | 86.4 | 1 | 0 | 0 |
| Castell-Platja d'Aro | Barcelona | 87.0 | 1 | 0 | 0 |
| León | Oviedo | 88.2 | 1 | 0 | 1 |
| Cartagena | Alicante | 92.1 | 1 | 0 | 0 |
| Logroño | Bilbao | 97.8 | 1 | 0 | 1 |
| Ciudad Real | Toledo | 98.2 | 1 | 0 | 0 |
| Roquetas de Mar | Granada | 98.2 | 2 | 0 | 0 |
| Lepe | Seville | 108.1 | 1 | 0 | 0 |
| Salamanca | Valladolid | 109.5 | 1 | 0 | 0 |
| Burgos | Valladolid | 115.2 | 1 | 0 | 2 |
| Aranguren | Bilbao | 117.8 | 1 | 0 | 0 |
| Figueres | Barcelona | 118.7 | 1 | 0 | 0 |
| Lleida | Zaragoza | 126.2 | 1 | 1 | 0 |
| Eivissa | Palma | 127.1 | 1 | 0 | 0 |
| Vinaròs | Valencia | 130.9 | 1 | 0 | 0 |
| Lorca | Alicante | 131.3 | 1 | 0 | 0 |
| Cuenca | Madrid | 137.9 | 1 | 0 | 0 |
| Albacete | Valencia | 138.9 | 0 | 0 | 1 |
| Villanueva de la Serena | Córdoba | 149.9 | 1 | 0 | 0 |
| Tortosa | Zaragoza | 150.9 | 1 | 0 | 0 |
| Badajoz | Lisbon (Portugal) | 186.6 | 1 | 0 | 0 |
| Cáceres | Coimbra (Portugal) | 191.3 | 1 | 0 | 0 |
| Melilla | Málaga | 209.0 | 0 | 0 | 1 |

### United Kingdom — 55 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Merton | London | 12.5 | 2 | 0 | 0 |
| Walsall | Birmingham | 12.6 | 1 | 0 | 0 |
| Greenwich | London | 12.7 | 1 | 1 | 0 |
| Lisburn | Belfast | 13.6 | 1 | 0 | 0 |
| Wakefield | Leeds | 14.9 | 2 | 0 | 0 |
| Sutton | London | 15.4 | 1 | 0 | 1 |
| Stevenage | Luton | 15.6 | 1 | 0 | 0 |
| Warrington | Wigan | 16.0 | 1 | 0 | 1 |
| Hillingdon | London | 18.9 | 2 | 0 | 1 |
| Tamworth | Birmingham | 20.2 | 1 | 0 | 0 |
| Derby | Nottingham | 22.0 | 1 | 0 | 3 |
| West Lothian | Edinburgh | 22.1 | 1 | 0 | 0 |
| Harrogate | Leeds | 22.2 | 0 | 1 | 1 |
| Rushmoor | Reading | 23.3 | 1 | 0 | 0 |
| Watford | Luton | 24.3 | 1 | 0 | 0 |
| Carmarthenshire | Swansea | 25.2 | 2 | 0 | 0 |
| Cherwell | Oxford | 25.4 | 1 | 1 | 0 |
| High Peak | Manchester | 25.4 | 0 | 2 | 0 |
| Liverpool | Wigan | 25.4 | 2 | 0 | 3 |
| Milton Keynes | Luton | 26.7 | 2 | 0 | 1 |
| Thurrock | London | 29.1 | 1 | 0 | 0 |
| Perthshire and Kinross | Dundee | 30.6 | 1 | 0 | 0 |
| Inverclyde | Glasgow | 30.9 | 0 | 1 | 1 |
| Crawley | Brighton | 33.6 | 1 | 0 | 0 |
| Lancaster | Preston | 33.7 | 1 | 0 | 0 |
| Cheshire West and Chester | Wigan | 35.8 | 2 | 0 | 0 |
| Guildford | Reading | 36.4 | 1 | 0 | 0 |
| York | Leeds | 37.4 | 1 | 0 | 1 |
| Swindon | Oxford | 41.4 | 1 | 0 | 1 |
| Weymouth and Portland | Bournemouth | 42.3 | 1 | 0 | 0 |
| Scottish Borders | Edinburgh | 44.3 | 1 | 0 | 0 |
| Telford and Wrekin | Birmingham | 45.2 | 1 | 0 | 0 |
| Peterborough | Cambridge | 49.5 | 1 | 0 | 1 |
| Lincoln | Nottingham | 50.8 | 1 | 0 | 1 |
| Gloucester | Bristol | 51.6 | 1 | 0 | 0 |
| Newry and Mourne | Belfast | 53.1 | 1 | 0 | 0 |
| North Lincolnshire | Sheffield | 58.8 | 0 | 1 | 2 |
| Cheltenham | Oxford | 59.7 | 1 | 1 | 1 |
| Wrexham | Wigan | 60.2 | 1 | 0 | 0 |
| North Devon | Swansea | 61.4 | 1 | 0 | 0 |
| Herefordshire | Birmingham | 69.1 | 1 | 1 | 0 |
| Pembrokeshire | Swansea | 73.7 | 1 | 0 | 0 |
| Boston | Nottingham | 74.6 | 1 | 0 | 0 |
| Coleraine | Belfast | 75.1 | 1 | 0 | 0 |
| Kingston upon Hull | Leeds | 78.7 | 2 | 0 | 0 |
| Carlisle | Newcastle | 84.6 | 0 | 0 | 2 |
| Exeter | Cardiff | 87.4 | 1 | 0 | 1 |
| Scarborough | Leeds | 90.4 | 1 | 0 | 0 |
| Moray | Aberdeen | 91.4 | 1 | 0 | 0 |
| Norwich | Cambridge | 92.4 | 1 | 0 | 1 |
| Dumfries and Galloway | Glasgow | 96.6 | 1 | 0 | 0 |
| Allerdale | Preston | 112.4 | 1 | 0 | 0 |
| Waveney | Cambridge | 113.3 | 1 | 0 | 0 |
| Highland | Aberdeen | 132.0 | 1 | 0 | 0 |
| Plymouth | Swansea | 136.5 | 1 | 0 | 1 |

### Poland — 55 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Pabianice | Łódź | 12.8 | 1 | 0 | 0 |
| Raszyn | Warsaw | 13.4 | 1 | 0 | 0 |
| Mikołów | Katowice | 13.7 | 1 | 0 | 0 |
| Piaseczno | Warsaw | 15.4 | 1 | 0 | 0 |
| Tarnowskie Góry | Gliwice | 20.8 | 1 | 0 | 0 |
| Rybnik | Gliwice | 23.5 | 1 | 0 | 0 |
| Żory | Gliwice | 29.4 | 1 | 0 | 0 |
| Rumia | Gdańsk | 30.3 | 1 | 0 | 0 |
| Skarżysko-Kamienna | Kielce | 31.8 | 1 | 0 | 0 |
| Stargard | Szczecin | 32.7 | 1 | 0 | 0 |
| Ostrołęka | Łomża | 39.5 | 1 | 0 | 0 |
| Inowrocław | Bydgoszcz | 39.8 | 1 | 0 | 0 |
| Toruń | Bydgoszcz | 42.5 | 2 | 0 | 1 |
| Starogard Gdański | Gdańsk | 44.1 | 1 | 0 | 0 |
| Puławy | Lublin | 45.9 | 1 | 0 | 0 |
| Nysa | Opole | 47.1 | 1 | 0 | 0 |
| Bielsko-Biała | Katowice | 47.5 | 2 | 0 | 0 |
| Gniezno | Poznań | 48.8 | 0 | 0 | 1 |
| Elbląg | Gdańsk | 53.5 | 1 | 0 | 0 |
| Ostrowiec Świętokrzyski | Kielce | 53.8 | 1 | 0 | 0 |
| Sieradz | Łódź | 53.9 | 1 | 0 | 0 |
| Świnoujście | Szczecin | 57.8 | 1 | 0 | 0 |
| Wałbrzych | Wrocław | 62.2 | 1 | 0 | 0 |
| Chełm, lubelskie | Lublin | 63.9 | 1 | 0 | 0 |
| Nowy Targ | Kraków | 67.1 | 1 | 0 | 0 |
| Ełk | Łomża | 68.1 | 1 | 0 | 0 |
| Radom | Kielce | 68.7 | 2 | 1 | 0 |
| Chojnice | Bydgoszcz | 70.5 | 1 | 0 | 0 |
| Mława | Olsztyn | 74.0 | 1 | 0 | 0 |
| Nowy Sącz | Kraków | 74.0 | 2 | 0 | 0 |
| Tarnów | Kraków | 75.9 | 1 | 0 | 0 |
| Zamość | Lublin | 76.7 | 1 | 0 | 0 |
| Ciechanów | Warsaw | 76.9 | 1 | 0 | 0 |
| Kłodzko | Wrocław | 78.9 | 1 | 0 | 0 |
| Augustów | Białystok | 79.6 | 1 | 0 | 0 |
| Ostrów Wielkopolski | Wrocław | 81.7 | 1 | 0 | 0 |
| Tarnobrzeg | Kielce | 82.2 | 1 | 0 | 0 |
| Piła | Poznań | 83.8 | 1 | 0 | 0 |
| Mielec | Kielce | 86.6 | 1 | 0 | 0 |
| Włocławek | Bydgoszcz | 87.5 | 1 | 0 | 0 |
| Gorzów Wielkopolski | Szczecin | 88.3 | 2 | 0 | 0 |
| Płock | Łódź | 89.4 | 2 | 0 | 0 |
| Głogów | Wrocław | 89.8 | 1 | 0 | 0 |
| Zgorzelec | Dresden (Germany) | 90.8 | 1 | 0 | 0 |
| Jelenia Góra | Wrocław | 92.7 | 1 | 0 | 0 |
| Biała Podlaska | Lublin | 96.4 | 0 | 1 | 1 |
| Słupsk | Gdańsk | 106.7 | 2 | 0 | 0 |
| Kołobrzeg, Zachodniopomorskie | Szczecin | 107.0 | 1 | 0 | 0 |
| Zielona Góra | Poznań | 109.8 | 1 | 1 | 0 |
| Suwałki | Białystok | 111.2 | 1 | 0 | 0 |
| Krosno | Košice (Slovakia) | 116.3 | 1 | 0 | 1 |
| Żary | Dresden (Germany) | 116.6 | 1 | 0 | 0 |
| Koszalin | Bornholm (Denmark) | 128.3 | 1 | 0 | 0 |
| Rzeszów | Kielce | 134.3 | 1 | 0 | 1 |
| Przemyśl | Lublin | 162.8 | 1 | 0 | 0 |

### Sweden — 32 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Täby | Stockholm | 15.1 | 1 | 0 | 0 |
| Järfälla | Stockholm | 15.5 | 1 | 0 | 0 |
| Haninge | Stockholm | 16.3 | 1 | 0 | 0 |
| Södertälje | Stockholm | 29.8 | 0 | 1 | 1 |
| Malmö | Copenhagen (Denmark) | 29.9 | 1 | 0 | 0 |
| Helsingborg | Copenhagen (Denmark) | 47.9 | 1 | 0 | 0 |
| Borås | Gothenburg | 57.5 | 1 | 0 | 0 |
| Norrtälje | Stockholm | 58.2 | 1 | 0 | 0 |
| Uppsala | Stockholm | 61.7 | 1 | 0 | 0 |
| Enköping | Stockholm | 65.7 | 1 | 0 | 0 |
| Trollhättan | Gothenburg | 69.9 | 1 | 0 | 0 |
| Nyköping | Stockholm | 87.2 | 1 | 0 | 0 |
| Västerås | Stockholm | 91.9 | 1 | 1 | 0 |
| Halmstad | Copenhagen (Denmark) | 111.9 | 1 | 0 | 1 |
| Jönköping | Gothenburg | 132.0 | 1 | 0 | 0 |
| Norrköping | Stockholm | 135.1 | 1 | 0 | 1 |
| Skövde | Gothenburg | 135.9 | 1 | 0 | 0 |
| Gävle | Stockholm | 156.3 | 1 | 2 | 0 |
| Karlstad | Oslo (Norway) | 165.3 | 2 | 0 | 0 |
| Luleå | Oulu (Finland) | 172.1 | 1 | 0 | 0 |
| Ludvika | Stockholm | 186.3 | 1 | 0 | 0 |
| Gotland | Stockholm | 190.5 | 1 | 0 | 0 |
| Växjö | Gothenburg | 192.3 | 0 | 1 | 1 |
| Motala | Stockholm | 193.8 | 1 | 0 | 0 |
| Borlänge | Stockholm | 194.9 | 1 | 0 | 0 |
| Skellefteå | Oulu (Finland) | 213.0 | 2 | 0 | 0 |
| Östersund | Trondheim (Norway) | 215.4 | 1 | 0 | 0 |
| Bollnäs | Stockholm | 243.1 | 1 | 1 | 0 |
| Mora | Oslo (Norway) | 243.4 | 1 | 0 | 0 |
| Umeå | Oulu (Finland) | 279.2 | 1 | 0 | 0 |
| Örnsköldsvik | Tampere (Finland) | 326.9 | 1 | 0 | 0 |
| Sundsvall | Turku (Finland) | 342.8 | 1 | 0 | 0 |

### Czechia — 27 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Čestlice | Prague | 12.3 | 1 | 0 | 0 |
| Blansko | Brno | 19.5 | 1 | 0 | 0 |
| Mělník | Prague | 31.4 | 1 | 0 | 0 |
| Králův Dvůr | Prague | 31.5 | 1 | 0 | 0 |
| Teplice | Dresden (Germany) | 44.6 | 1 | 0 | 0 |
| Příbram | Plzeň | 45.2 | 0 | 0 | 2 |
| Ústí nad Labem | Dresden (Germany) | 47.5 | 1 | 0 | 0 |
| Prostějov | Brno | 49.0 | 1 | 0 | 0 |
| Mladá Boleslav | Prague | 51.6 | 0 | 1 | 1 |
| Třebíč | Brno | 51.9 | 0 | 0 | 1 |
| Znojmo | Brno | 55.2 | 0 | 0 | 1 |
| Havířov | Gliwice (Poland) | 59.5 | 1 | 0 | 0 |
| Ostrava | Gliwice (Poland) | 62.0 | 1 | 0 | 2 |
| Olomouc | Brno | 63.9 | 1 | 0 | 3 |
| Karlovy Vary | Plzeň | 67.0 | 1 | 0 | 0 |
| Opava | Gliwice (Poland) | 67.0 | 1 | 0 | 0 |
| Přerov | Brno | 67.8 | 1 | 0 | 0 |
| Otrokovice | Brno | 69.3 | 1 | 0 | 0 |
| Frýdek-Místek | Gliwice (Poland) | 72.8 | 1 | 0 | 0 |
| Písek | Plzeň | 74.1 | 1 | 0 | 0 |
| České Budějovice | Linz (Austria) | 76.5 | 0 | 0 | 2 |
| Jihlava | Brno | 77.7 | 1 | 0 | 0 |
| Tábor | Prague | 78.4 | 1 | 0 | 0 |
| Cheb | Plzeň | 80.8 | 1 | 0 | 0 |
| Jablonec nad Nisou | Prague | 88.7 | 1 | 0 | 0 |
| Hradec Králové | Prague | 99.9 | 1 | 0 | 1 |
| Rožnov pod Radhoštěm | Gliwice (Poland) | 101.0 | 0 | 0 | 1 |

### Finland — 19 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Espoo | Helsinki | 13.8 | 2 | 0 | 0 |
| Salo | Turku | 46.9 | 1 | 0 | 0 |
| Riihimäki | Helsinki | 62.7 | 1 | 0 | 0 |
| Hämeenlinna | Tampere | 65.3 | 1 | 0 | 0 |
| Lahti | Helsinki | 96.6 | 1 | 1 | 1 |
| Pori | Tampere | 103.6 | 0 | 0 | 2 |
| Kotka | Helsinki | 114.2 | 1 | 0 | 0 |
| Ylivieska | Oulu | 114.2 | 1 | 0 | 0 |
| Jyväskylä | Tampere | 135.0 | 1 | 1 | 0 |
| Kajaani | Oulu | 140.6 | 1 | 0 | 0 |
| Seinäjoki | Tampere | 152.3 | 1 | 0 | 0 |
| Rovaniemi | Oulu | 164.9 | 1 | 0 | 0 |
| Kokkola | Oulu | 172.3 | 1 | 0 | 0 |
| Iisalmi | Oulu | 181.8 | 0 | 1 | 1 |
| Mikkeli | Tampere | 187.5 | 1 | 0 | 0 |
| Lappeenranta | Helsinki | 202.9 | 1 | 0 | 0 |
| Vaasa | Tampere | 209.5 | 1 | 0 | 0 |
| Kuopio | Tampere | 252.3 | 1 | 0 | 0 |
| Joensuu | Tampere | 336.8 | 1 | 0 | 0 |

### Hungary — 19 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Kistarcsa | Budapest | 16.1 | 1 | 0 | 0 |
| Tatabánya | Budapest | 48.9 | 1 | 0 | 0 |
| Dunaújváros | Budapest | 59.0 | 1 | 0 | 0 |
| Székesfehérvár | Budapest | 59.0 | 1 | 0 | 1 |
| Sopron | Vienna (Austria) | 61.0 | 1 | 0 | 0 |
| Győr | Bratislava (Slovakia) | 66.7 | 2 | 0 | 0 |
| Kecskemét | Budapest | 81.8 | 1 | 0 | 0 |
| Nyíregyháza | Košice (Slovakia) | 88.6 | 1 | 0 | 0 |
| Szombathely | Graz (Austria) | 93.8 | 1 | 0 | 0 |
| Veszprém | Budapest | 94.7 | 1 | 0 | 0 |
| Szolnok | Budapest | 95.0 | 1 | 0 | 0 |
| Szeged | Timișoara (Romania) | 101.2 | 2 | 0 | 0 |
| Békéscsaba | Timișoara (Romania) | 103.5 | 1 | 0 | 0 |
| Eger | Košice (Slovakia) | 108.8 | 1 | 0 | 0 |
| Zalaegerszeg | Graz (Austria) | 110.9 | 0 | 0 | 1 |
| Debrecen | Košice (Slovakia) | 131.2 | 0 | 0 | 1 |
| Szekszárd | Budapest | 131.5 | 1 | 0 | 0 |
| Kaposvár | Budapest | 158.6 | 1 | 0 | 0 |
| Pécs | Budapest | 172.3 | 1 | 0 | 1 |

### Slovakia — 16 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Prešov | Košice | 32.2 | 1 | 0 | 0 |
| Malacky | Bratislava | 32.6 | 0 | 0 | 1 |
| Dunajská Streda | Bratislava | 42.3 | 1 | 0 | 0 |
| Michalovce | Košice | 48.1 | 1 | 0 | 0 |
| Bardejov | Košice | 67.2 | 1 | 0 | 0 |
| Nitra | Bratislava | 74.4 | 1 | 0 | 1 |
| Stará Ľubovňa | Košice | 79.6 | 1 | 0 | 0 |
| Poprad | Košice | 81.8 | 1 | 0 | 0 |
| Levice | Budapest (Hungary) | 86.7 | 0 | 0 | 1 |
| Rimavská Sobota | Košice | 98.3 | 1 | 0 | 0 |
| Trenčín | Bratislava | 106.4 | 1 | 0 | 1 |
| Liptovský Mikuláš | Kraków (Poland) | 112.4 | 1 | 0 | 0 |
| Žilina | Katowice (Poland) | 118.3 | 1 | 0 | 0 |
| Zvolen | Budapest (Hungary) | 120.6 | 1 | 0 | 0 |
| Prievidza | Bratislava | 131.5 | 1 | 0 | 0 |
| Banská Bystrica | Budapest (Hungary) | 136.3 | 0 | 0 | 2 |

### Romania — 13 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Arad | Timișoara | 50.0 | 1 | 0 | 0 |
| Blejoi | Bucharest | 60.8 | 1 | 0 | 0 |
| Târgovişte | Bucharest | 75.5 | 1 | 0 | 0 |
| Vima Mică | Cluj-Napoca | 75.9 | 1 | 0 | 0 |
| Târgu Mureş | Cluj-Napoca | 76.4 | 0 | 1 | 1 |
| Alba Iulia | Cluj-Napoca | 76.6 | 1 | 0 | 0 |
| Buzău | Bucharest | 99.7 | 1 | 0 | 0 |
| Şelimbăr | Brașov | 111.4 | 1 | 0 | 0 |
| Focşani | Brașov | 125.8 | 1 | 0 | 0 |
| Satu Mare | Cluj-Napoca | 126.9 | 1 | 0 | 0 |
| Oradea | Cluj-Napoca | 133.9 | 1 | 0 | 0 |
| Târgu Jiu | Timișoara | 179.6 | 1 | 0 | 0 |
| Craiova | Bucharest | 183.2 | 0 | 1 | 1 |

### Bulgaria — 11 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Pernik | Sofia | 25.1 | 1 | 0 | 0 |
| Pazardzhik | Plovdiv | 33.3 | 1 | 0 | 0 |
| Dobrich | Varna | 39.5 | 1 | 0 | 0 |
| Vratsa | Sofia | 58.3 | 1 | 0 | 0 |
| Ruse | Bucharest (Romania) | 66.2 | 1 | 0 | 0 |
| Shumen | Varna | 79.2 | 1 | 0 | 0 |
| Stara Zagora | Plovdiv | 81.1 | 1 | 0 | 0 |
| Burgas | Varna | 84.3 | 1 | 0 | 0 |
| Veliko Tarnovo | Plovdiv | 126.5 | 1 | 0 | 0 |
| Pleven | Sofia | 132.6 | 1 | 0 | 0 |
| Yambol | Varna | 139.4 | 1 | 0 | 0 |

### Denmark — 11 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Høje-Taastrup | Copenhagen | 18.3 | 1 | 0 | 0 |
| Nyborg | Odense | 27.1 | 1 | 0 | 0 |
| Randers | Aarhus | 35.1 | 1 | 2 | 0 |
| Svendborg | Odense | 39.6 | 1 | 0 | 0 |
| Silkeborg | Aarhus | 41.1 | 1 | 0 | 0 |
| Frederikshavn | Aalborg | 56.7 | 1 | 0 | 0 |
| Slagelse | Odense | 60.5 | 1 | 0 | 0 |
| Sønderborg | Odense | 64.8 | 1 | 0 | 0 |
| Næstved | Copenhagen | 68.9 | 1 | 0 | 0 |
| Herning | Aarhus | 75.4 | 1 | 0 | 0 |
| Esbjerg | Odense | 115.6 | 1 | 2 | 0 |

### Croatia — 9 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Pula | Trieste (Italy) | 86.3 | 1 | 0 | 0 |
| Varaždin | Graz (Austria) | 111.2 | 1 | 0 | 0 |
| Zagreb | Graz (Austria) | 147.4 | 4 | 1 | 0 |
| Zadar | Ancona (Italy) | 179.1 | 1 | 0 | 0 |
| Sisak | Graz (Austria) | 189.2 | 1 | 0 | 0 |
| Osijek | Timișoara (Romania) | 199.0 | 1 | 0 | 1 |
| Šibenik | Ancona (Italy) | 213.8 | 1 | 0 | 0 |
| Slavonski Brod | Timișoara (Romania) | 255.8 | 1 | 1 | 0 |
| Split | Ancona (Italy) | 256.0 | 1 | 0 | 1 |

### Norway — 9 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Ullensaker | Oslo | 34.6 | 1 | 0 | 0 |
| Drammen | Oslo | 39.7 | 1 | 0 | 2 |
| Moss | Oslo | 55.1 | 1 | 0 | 0 |
| Steinkjer | Trondheim | 84.1 | 1 | 0 | 0 |
| Ringsaker | Oslo | 106.8 | 0 | 1 | 1 |
| Elverum | Oslo | 116.8 | 1 | 0 | 0 |
| Arendal | Aalborg (Denmark) | 173.0 | 1 | 0 | 0 |
| Rana | Trondheim | 365.6 | 1 | 0 | 0 |
| Bodø | Trondheim | 466.6 | 1 | 0 | 0 |

### Greece — 7 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Gerakas | Athens | 12.3 | 1 | 0 | 0 |
| Elefsina | Athens | 17.9 | 1 | 0 | 0 |
| Chania | Heraklion | 103.3 | 0 | 0 | 1 |
| Kalamata | Patras | 138.4 | 0 | 0 | 1 |
| Volos | Thessaloniki | 141.3 | 1 | 0 | 0 |
| Alexandroupolis | Plovdiv (Bulgaria) | 171.9 | 0 | 1 | 1 |
| Kanali | Patras | 219.8 | 1 | 0 | 0 |

## References

Ester, M., Kriegel, H.-P., Sander, J., and Xu, X. 1996. A density-based algorithm for
discovering clusters in large spatial databases with noise. *Proceedings of KDD-96*, 226–231.

Haklay, M. 2010. How good is volunteered geographical information? *Environment and Planning B:
Planning and Design* 37(4): 682–703.

OpenStreetMap contributors. *Open Database Licence (ODbL) 1.0.*
[https://opendatacommons.org/licenses/odbl/](https://opendatacommons.org/licenses/odbl/)

Overture Maps Foundation. *Open map data — places, buildings, transportation, addresses.*
[https://overturemaps.org/](https://overturemaps.org/)

## Contributors

Prepared by Woodfine Management Corp.

## How this paper was produced

This paper is grounded in the operating and development work the preparing staff do themselves, and in what they have learned from the people they work with routinely: the graphic designers, web developers, and software developers and engineers who build the platform alongside them, and the architects and structural, building-services, and civil engineers they develop buildings with. No outside professional reviewed or approved this paper, and nothing in it is professional advice. It was drafted and edited with AI assistance under editorial direction, and the analysis and conclusions are Woodfine's own.

## Disclosures

Woodfine Capital Projects Inc. ("Woodfine") is the author of record and owns the framework and
the resulting dataset published here; Woodfine Management Corp. maintains the data and runs the
analysis. Woodfine develops and promotes commercial property in markets of the kind listed, so
this paper publishes a dataset in which we have a direct commercial interest. This work was
funded internally; no external research funding was received. Nothing in this paper constitutes
an offer to sell, or a solicitation of an offer to buy, any interest in a Woodfine direct-hold
solution; any offering is made only by the applicable Private Placement Memorandum, which
prospective investors should review with their own professional advisors. **Inclusion of any
market in this list reflects the screening criteria described in Section 1 and does not indicate
acquisition, option, or development activity, committed or planned, in that market or any
other.** No rank, score, or market-to-market comparison is published, and nothing here is a
forecast of any market's performance. The named retail chains appear as the subject of a
site-selection method; their inclusion is not a statement about their businesses. Some
statements above describe planned or intended future work; language such as "planned,"
"intended," "targeted," "may," and "expected" marks this forward-looking content, which is
subject to change and does not constitute a commitment regarding future performance.

## Data and reproducibility

Every row in Section 6 is reproduced from the published country tables, not re-derived for this
paper, so the figures here and the figures on the published country pages are the same figures.
The co-location data behind them is drawn from OpenStreetMap under the Open Database Licence —
freely downloadable, usable commercially, on terms requiring that a derived database be shared
on the same basis — filtered by canonical chain identifiers so that the same company resolves
consistently across borders, and supplemented by civic-anchor records from an openly licensed
global places dataset. Cluster boundaries are computed in two passes over the anchor locations.
A reader with those sources can reconstruct the composition assessment for any market in this
list. Municipal boundaries are from the European
statistical office's published administrative-unit dataset. The figures describe the current
dataset build; a September 2026 rebuild superseded an earlier eleven-country selection that had
included Germany, France and the Netherlands, retired under the 30 June 2026 methodology lock,
so any copy of this list carrying those countries is a stale one. The set is a curated editorial
selection derived from the live market layer and does not replace or alter that layer, which
remains unranked and uncurated at its full qualifying count of 650. Counts move between
builds as chain coverage grows and as clusters re-form, so this is a dated snapshot rather than
a permanent statement. Market display names are reproduced as the underlying settlement records
carry them, in the local spelling and including any regional suffix; no market's identity or
geography has been altered. Catchment population and consumer-spend figures are absent for 141
and 178 entries respectively and are reported as absent rather than as zero. No independent party has audited this dataset, reproduced these
figures, or reviewed these claims.

Woodfine Capital Projects™ is a trademark of Woodfine Capital Projects Inc.
