---
schema: journal-v2
slug: regional-markets-north-america-rankings
title: "The 400 Published Regional Markets in North America"
subtitle: "The full list, with the metropolitan reference point and cluster composition for every entry"
site: gis.woodfinegroup.com
imprint: WCP-005
thesis: "This is the complete North American published set — 400 markets drawn from a 1,121-market qualifying pool — published in full, by country, with no rank and no score, because none is published."
abstract: |
  This is the data companion to the Regional Markets methodology paper: the full published
  North American set, 400 named markets drawn from a qualifying pool of 1,121 across three
  countries. For each market it gives the metropolitan centre the market is measured against,
  the straight-line distance to it, and how many co-location clusters of each composition
  tier the market carries. It does not re-argue the qualification method, which is the
  methodology paper's subject. Two things this table is not: it is not a ranking, because no
  rank or score is published for any market and the tables are simply sorted by reference
  distance so that they can be read; and it is not investment advice about any listed location. The recorded distance is descriptive
  context and takes no part in qualification — it is a straight-line measurement, not a
  drive time, and it is not a claim that a market functions as a commuter suburb of the
  centre named beside it.
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
  - atlas-top-400-north-america
  - atlas-united-states
  - atlas-canada
  - atlas-mexico
  - about-regional-markets-system
  - co-location-methodology
prepared_by: "Woodfine Management Corp."
keywords:
  - regional markets
  - North America
  - published dataset
  - anchor composition
  - site selection
---

> Nothing in this paper constitutes an offer to sell, or a solicitation of an offer to buy,
> any interest in a Woodfine direct-hold solution; any offering is made only by the
> applicable Private Placement Memorandum. Statements marked "planned," "intended,"
> "targeted," "may," or "expected" are forward-looking and subject to change. Full
> disclosures appear at the end of this paper.

Working Paper WCP-005 · v0.1.0 · CC BY 4.0

This paper publishes the complete North American Regional Markets set: four hundred named
markets that clear the anchor-composition gates, drawn from a qualifying pool of 1,121 across
three countries. It is a data companion, not an argument. The reasoning behind the
qualification method — why anchor composition rather than population, and why the published
set is deliberately smaller than the qualifying pool — belongs to the methodology paper and is
not restated here beyond what a reader needs to read the tables.

Two statements about what this is not, before anything else.

**It is not a ranking.** No rank and no score is published for any market in this set. The
tables below are sorted by reference distance within each country purely so they can be read,
and no market-to-market comparison is published or implied. A composite measure exists
internally to support the selection; it is not published and has no bearing on how any market is described here.

**It is not advice about any listed location.** A market's presence in this set means that
independent large-format retailers have converged there in a qualifying combination. It is not
a forecast about that market, not a recommendation, and not an indication that anything has
been acquired, optioned, or developed there or anywhere near it.

## 1. How a market enters this set

A Regional Market is a named settlement — a legally incorporated place or equivalent
administrative unit, whose name differs from that of its metropolitan reference point — whose
retail co-location clusters, taken together, satisfy an anchor-composition test.

A market qualifies under one of three gates. A **Regional Market** carries a hypermarket anchor
plus at least two of hardware, price club, lifestyle, electronics or sport, combined across all
of the market's member clusters. A **District Anchor** carries a hypermarket and a hardware
anchor with no other optional category, across at least two distinct clusters. A **Standalone
Regional Centre** meets that same condition in a market isolated from any other qualifying
market beyond the outer geographic band.

Of the four hundred North American entries, 382 qualify as Regional Markets and 18 as
Standalone Regional Centres — nine in Mexico, five in Canada, four in the United States. No
North American entry qualifies as a District Anchor. The standalone class is where this set
reaches genuinely isolated regional centres rather than settlements sitting in a metropolitan
orbit.

A geographic coherence constraint applies: all of a settlement's member clusters must lie
within a 200-kilometre bounding box. Settlements failing it are name-collision aggregations —
several unrelated places sharing a name — and are excluded rather than treated as one very
large market.

Selection from the qualifying pool takes the four hundred markets with the strongest anchor
composition per continent, with no per-country budget. A small per-country minimum floor
prevents a country with genuine qualifying markets from being excluded outright and otherwise
does not affect which markets are included. The per-country counts are therefore an observed
result of one continental cutoff, not a quota set in advance.

Catchment population and consumer-spend figures accompany each market in the underlying data as
descriptive context. They take no part in selection. Population is negatively correlated with
the composition measure in every country tested, so selecting on population would
systematically replace genuine regional markets with dense metropolitan-fringe suburbs.

## 2. How to read the table

**Market** is the settlement's own name.

**Metropolitan reference** is the nearest major metropolitan centre in the framework's
continental reference set. It is a descriptive anchor, not a relationship: naming a centre
beside a market is not a claim that the market functions as a commuter suburb of it.

**km** is the straight-line distance from the market to that centre. It is not a drive time and
not a commuting estimate, and it is recorded rather than gated — distance takes no part in
whether a market qualifies. A distance term was present in an earlier iteration of the
selection method and was removed, because it caused standalone secondary cities to outrank
genuine suburbs of major metropolitan areas.

**T1**, **T2** and **T3** are counts of the market's co-location clusters at each composition
tier. In North America, a **Tier 1** cluster contains a hypermarket — Walmart Supercenter,
Target, Meijer or H-E-B among them — a home-improvement warehouse such as Home Depot or Lowe's,
and a warehouse club such as Costco, Sam's Club or BJ's. A **Tier 2** cluster contains a
hypermarket and a hardware anchor without a warehouse club. A **Tier 3** cluster contains a
single recognised anchor category. A market may carry clusters at more than one tier; the
figures are counts of clusters, not of stores.

## 3. Country summary

| Country | Published markets | Qualifying pool | T1 | T2 | T3 | Median reference distance |
|---|---|---|---|---|---|---|
| United States | 298 | 916 | 348 | 59 | 79 | 75 km |
| Canada | 56 | 112 | 77 | 13 | 17 | 90 km |
| Mexico | 46 | 93 | 54 | 3 | 58 | 152 km |
| **Total** | **400** | **1,121** | **479** | **75** | **154** | — |

The United States publishes 298 of 916 qualifying markets — under a third of its pool, and the
deepest reserve in either continental set. Canada and Mexico publish roughly half of theirs.

## 4. Composition and geography

The four hundred markets carry 708 co-location clusters between them — 479 Tier 1, 75 Tier 2
and 154 Tier 3 — an average of 1.77 clusters per market. Tier 1 presence is close to universal:
397 of the four hundred markets carry at least one Tier 1 cluster, and only two markets qualify
on Tier 3 clusters alone.

Mexico is the exception, in composition rather than in qualification. Its 46 markets carry 54
Tier 1 clusters but 58 Tier 3 clusters — the only country in either continental set where Tier
3 clusters outnumber Tier 1.

The set spans 110 distinct metropolitan reference points. Vancouver is the reference for 13
entries and Toronto for 12 — the two largest, both Canadian, in a set that is three-quarters
United States markets. Baltimore carries 10, and Boston, Minneapolis, Montreal, Mexico City and
Nashville between eight and nine each.

Recorded reference distances run from 12 to 694 kilometres, with a median of 81. Just under
half the set — 198 of 400 — sits within 80 kilometres of its reference point, and 109 sit beyond
150. Mexico accounts for much of the long tail, with a median reference distance of 152
kilometres against 75 for the United States and 90 for Canada.

## 5. Catchment data coverage

Catchment population and consumer-spend figures are recorded for all four hundred North
American markets, with no country-level gaps — in contrast to the European set, where more than
a third of entries carry no catchment population at all.

Two methods produce those figures, and each record discloses which applied. For 192 markets the
figure is a deduplicated union of catchment cells across all of the market's member clusters.
For the remaining 208 it falls back to the strongest member cluster's own figure, because a
full union could not be computed. The two are not interchangeable, and a reader comparing
catchment figures between markets should check which method produced each.

## 6. The markets

Listed by country, and within each country in ascending order of reference distance. That
sort is descriptive, not ordinal: no rank or score is published for any entry, and a market's
position in a table says nothing about it beyond how far it sits from the centre named beside
it.

### United States — 298 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Brentwood, MO | St. Louis | 12.0 | 1 | 0 | 0 |
| Manchester, CT | Hartford | 12.3 | 1 | 0 | 0 |
| Blasdell, NY | Buffalo | 12.4 | 1 | 0 | 0 |
| Attleboro, MA | Providence | 12.6 | 1 | 0 | 0 |
| Tonawanda Town, NY | Buffalo | 12.9 | 1 | 0 | 0 |
| Sunnyvale, CA | San Jose | 13.4 | 1 | 0 | 0 |
| Ankeny, IA | Des Moines | 13.7 | 1 | 0 | 0 |
| Chula Vista, CA | Tijuana (Mexico) | 13.9 | 3 | 0 | 0 |
| Rossville, MD | Baltimore | 13.9 | 2 | 0 | 0 |
| Spring Valley, NV | Las Vegas | 13.9 | 1 | 0 | 2 |
| San Bernardino, CA | Riverside | 14.3 | 1 | 1 | 0 |
| West Des Moines, IA | Des Moines | 14.6 | 1 | 0 | 0 |
| Tempe, AZ | Phoenix | 15.2 | 2 | 0 | 1 |
| Oakdale, PA | Pittsburgh | 15.3 | 1 | 0 | 0 |
| Burbank, CA | Los Angeles | 15.4 | 1 | 0 | 1 |
| Franklin, WI | Milwaukee | 15.4 | 1 | 0 | 1 |
| Pineville, NC | Charlotte | 15.5 | 1 | 0 | 0 |
| Florence, KY | Cincinnati | 15.9 | 1 | 0 | 1 |
| Hoover, AL | Birmingham | 15.9 | 2 | 0 | 1 |
| Henderson, NV | Las Vegas | 16.5 | 1 | 0 | 1 |
| Avon, IN | Indianapolis | 16.7 | 1 | 0 | 0 |
| Alafaya, FL | Orlando | 16.9 | 1 | 0 | 0 |
| Warrensville Heights, OH | Cleveland | 17.5 | 1 | 0 | 0 |
| Sandy Springs, GA | Kennesaw | 17.6 | 1 | 0 | 1 |
| Aurora, CO | Denver | 17.7 | 4 | 1 | 0 |
| Hawthorne, CA | Los Angeles | 18.4 | 1 | 1 | 0 |
| Tukwila, WA | Seattle | 18.7 | 1 | 0 | 0 |
| Moorestown-Lenola, NJ | Philadelphia | 18.8 | 2 | 0 | 1 |
| Warwick, RI | Providence | 19.1 | 3 | 1 | 0 |
| Hillsboro, OR | Portland | 19.4 | 1 | 1 | 0 |
| Hiram, GA | Kennesaw | 19.8 | 1 | 0 | 0 |
| Plymouth Meeting, PA | Philadelphia | 19.9 | 1 | 0 | 0 |
| Columbia, MD | Baltimore | 20.4 | 1 | 0 | 0 |
| Gulfport, MS | Mobile | 20.4 | 1 | 0 | 0 |
| Norfolk, VA | Virginia Beach | 20.4 | 1 | 0 | 0 |
| Short Pump, VA | Richmond | 20.8 | 1 | 0 | 1 |
| Horn Lake, MS | Memphis | 21.0 | 1 | 0 | 0 |
| Owasso, OK | Tulsa | 21.1 | 1 | 0 | 0 |
| Maple Grove, MN | Minneapolis | 21.3 | 2 | 0 | 0 |
| Overland Park, KS | Kansas City | 21.6 | 1 | 1 | 1 |
| Sandy, UT | Salt Lake City | 21.6 | 1 | 1 | 0 |
| Carmel, IN | Indianapolis | 22.0 | 2 | 0 | 0 |
| Issaquah, WA | Seattle | 22.2 | 1 | 0 | 0 |
| Universal City, TX | San Antonio | 22.2 | 1 | 0 | 0 |
| Scottsdale, AZ | Phoenix | 22.7 | 1 | 2 | 0 |
| Maywood, NJ | New York | 23.1 | 1 | 0 | 0 |
| Hunters Creek, FL | Orlando | 23.2 | 1 | 0 | 1 |
| King of Prussia, PA | Wilmington DE | 23.2 | 1 | 0 | 0 |
| Danvers, MA | Boston | 23.4 | 2 | 0 | 0 |
| Lone Tree, CO | Denver | 23.5 | 1 | 0 | 1 |
| Pearland, TX | Houston | 23.9 | 1 | 1 | 1 |
| Mount Juliet, TN | Nashville | 24.0 | 1 | 0 | 0 |
| Woodland, CA | Sacramento | 24.0 | 1 | 0 | 0 |
| Franklin, TN | Nashville | 25.1 | 2 | 1 | 0 |
| Alpharetta, GA | Kennesaw | 25.2 | 1 | 0 | 1 |
| Lynnwood, WA | Seattle | 25.4 | 1 | 0 | 0 |
| Coon Rapids, MN | Minneapolis | 25.7 | 1 | 0 | 0 |
| Gastonia, NC | Charlotte | 25.9 | 1 | 0 | 0 |
| Mansfield, TX | Fort Worth | 25.9 | 1 | 0 | 0 |
| Burlington, NC | Greensboro | 26.2 | 1 | 0 | 0 |
| Horsham, PA | Philadelphia | 26.7 | 2 | 0 | 0 |
| Concord, NC | Charlotte | 26.8 | 2 | 0 | 0 |
| Woodbury, MN | Minneapolis | 27.1 | 1 | 0 | 1 |
| Silverdale, WA | Seattle | 27.2 | 1 | 0 | 0 |
| Avon, OH | Cleveland | 27.3 | 1 | 0 | 0 |
| Tracy, CA | Stockton | 27.3 | 1 | 0 | 0 |
| Glen Carbon, IL | St. Louis | 27.4 | 1 | 0 | 0 |
| Clearwater, FL | Tampa | 27.7 | 2 | 0 | 0 |
| Long Beach, CA | Los Angeles | 27.7 | 3 | 0 | 0 |
| Leominster, MA | Worcester | 28.4 | 1 | 1 | 0 |
| Plano, TX | Dallas | 28.4 | 3 | 2 | 1 |
| Southlake, TX | Fort Worth | 28.5 | 1 | 0 | 1 |
| Framingham, MA | Boston | 28.6 | 1 | 0 | 0 |
| Livonia, MI | Detroit | 28.8 | 2 | 0 | 0 |
| Roseville, CA | Sacramento | 28.8 | 2 | 1 | 0 |
| Round Rock, TX | Austin | 29.0 | 1 | 0 | 1 |
| Seven Fields, PA | Pittsburgh | 29.0 | 1 | 0 | 0 |
| Humble, TX | Houston | 30.2 | 1 | 0 | 0 |
| Chesapeake, VA | Virginia Beach | 30.6 | 2 | 1 | 0 |
| Mesa, AZ | Phoenix | 30.9 | 2 | 1 | 4 |
| Bear, DE | Wilmington DE | 31.1 | 1 | 0 | 0 |
| Sugar Land, TX | Houston | 31.2 | 1 | 0 | 0 |
| Douglasville, GA | Kennesaw | 31.3 | 1 | 0 | 0 |
| Nampa, ID | Boise | 31.5 | 1 | 0 | 0 |
| Folsom, CA | Sacramento | 31.8 | 1 | 0 | 1 |
| Colonial Heights, VA | Richmond | 32.6 | 1 | 0 | 0 |
| Florham Park, NJ | New York | 32.7 | 1 | 0 | 0 |
| Uniondale, NY | New York | 34.1 | 1 | 0 | 0 |
| Rock Hill, SC | Charlotte | 34.3 | 1 | 0 | 0 |
| Parole, MD | Baltimore | 34.6 | 1 | 0 | 0 |
| Orland Park, IL | Chicago | 35.6 | 1 | 0 | 0 |
| Rockwall, TX | Dallas | 35.9 | 1 | 0 | 1 |
| Conyers, GA | Atlanta | 37.6 | 1 | 0 | 0 |
| Fullerton, CA | Los Angeles | 37.7 | 2 | 0 | 0 |
| Concord, CA | San Francisco | 39.3 | 1 | 0 | 0 |
| Brentwood, CA | Stockton | 39.6 | 1 | 0 | 0 |
| Smith Mills, MA | Providence | 39.9 | 1 | 0 | 0 |
| Live Oak, CA | San Jose | 40.3 | 1 | 0 | 0 |
| Conway, AR | Little Rock | 40.7 | 1 | 1 | 0 |
| Mooresville, NC | Charlotte | 40.8 | 1 | 0 | 0 |
| Danbury, CT | New Haven | 42.4 | 1 | 0 | 0 |
| Appleton, WI | Green Bay | 42.5 | 1 | 1 | 0 |
| Spartanburg, SC | Greenville SC | 43.3 | 1 | 1 | 0 |
| Vallejo, CA | San Francisco | 43.8 | 1 | 0 | 0 |
| Florida City, FL | Miami | 43.9 | 1 | 0 | 0 |
| Frisco, TX | Dallas | 44.0 | 3 | 1 | 0 |
| Sunrise, FL | Miami | 44.6 | 1 | 0 | 1 |
| Methuen Town, NH | Boston | 45.0 | 1 | 0 | 1 |
| Anderson, SC | Greenville SC | 45.2 | 1 | 1 | 0 |
| Akron, OH | Cleveland | 46.0 | 1 | 0 | 0 |
| Riverhead, NY | New Haven | 46.7 | 1 | 0 | 0 |
| Gilroy, CA | San Jose | 46.8 | 1 | 0 | 0 |
| Ames, IA | Des Moines | 47.0 | 1 | 0 | 0 |
| Riverdale, UT | Salt Lake City | 47.4 | 1 | 0 | 0 |
| Vernon Hills, IL | Chicago | 48.0 | 1 | 0 | 0 |
| Santa Clarita, CA | Los Angeles | 48.2 | 3 | 1 | 0 |
| Murrieta, CA | Riverside | 48.9 | 2 | 0 | 0 |
| Norwalk, CT | New Haven | 49.3 | 1 | 0 | 0 |
| Saratoga Springs, NY | Albany | 50.0 | 1 | 0 | 0 |
| Tustin, CA | Riverside | 50.4 | 1 | 0 | 0 |
| San Marcos, TX | Austin | 50.6 | 1 | 0 | 0 |
| Lakeland, FL | Tampa | 51.1 | 1 | 0 | 1 |
| Paxtonia, PA | Lancaster | 51.6 | 1 | 0 | 0 |
| Pleasant Prairie, WI | Milwaukee | 52.3 | 1 | 0 | 0 |
| Buford, GA | Atlanta | 52.9 | 1 | 1 | 1 |
| Mission Viejo, CA | Riverside | 54.7 | 2 | 0 | 0 |
| Nashua, NH | Boston | 55.8 | 2 | 1 | 1 |
| Ann Arbor, MI | Detroit | 56.5 | 2 | 0 | 0 |
| Joliet, IL | Chicago | 56.6 | 2 | 0 | 0 |
| Coral Springs, FL | Miami | 56.9 | 2 | 0 | 1 |
| Princeton, NJ | Philadelphia | 56.9 | 1 | 0 | 0 |
| Merced, CA | Modesto | 57.2 | 1 | 0 | 0 |
| Millville, NJ | Philadelphia | 59.5 | 1 | 0 | 0 |
| Palmdale, CA | Los Angeles | 60.7 | 1 | 0 | 1 |
| Commack, NY | New York | 61.3 | 2 | 0 | 0 |
| Visalia, CA | Fresno | 61.9 | 1 | 1 | 0 |
| New London, CT | Hartford | 62.1 | 1 | 0 | 0 |
| Conroe, TX | Houston | 63.5 | 1 | 0 | 0 |
| Mechanicsburg, PA | Lancaster | 64.3 | 1 | 0 | 1 |
| Pueblo, CO | Colorado Springs | 64.8 | 1 | 1 | 0 |
| Clarksville, TN | Nashville | 66.1 | 1 | 0 | 0 |
| Hickory, NC | Charlotte | 67.1 | 1 | 0 | 0 |
| Centerville, OH | Cincinnati | 67.6 | 1 | 0 | 1 |
| Las Cruces, NM | El Paso | 68.4 | 2 | 0 | 0 |
| Goleta, CA | Oxnard | 68.5 | 1 | 0 | 0 |
| Ballenger Creek, MD | Baltimore | 69.2 | 1 | 0 | 0 |
| McKee City, NJ | Philadelphia | 72.6 | 1 | 0 | 0 |
| Bellingham, WA | Vancouver (Canada) | 73.8 | 2 | 0 | 0 |
| Loveland, CO | Denver | 74.6 | 1 | 0 | 1 |
| Bayou Cane, LA | New Orleans | 75.8 | 1 | 0 | 0 |
| Dulles Town Center, VA | Baltimore | 75.9 | 1 | 0 | 0 |
| Manchester, NH | Boston | 76.5 | 1 | 2 | 0 |
| Tuscaloosa, AL | Birmingham | 76.7 | 1 | 0 | 1 |
| Hot Springs, AR | Little Rock | 77.8 | 1 | 0 | 0 |
| Waldorf, MD | Baltimore | 78.0 | 1 | 0 | 1 |
| Santa Rosa, CA | San Francisco | 78.4 | 1 | 1 | 0 |
| Kokomo, IN | Indianapolis | 79.1 | 1 | 0 | 0 |
| Daytona Beach, FL | Orlando | 79.4 | 1 | 0 | 1 |
| Lincoln, NE | Omaha | 80.1 | 2 | 1 | 2 |
| Manahawkin, NJ | Philadelphia | 80.7 | 1 | 0 | 0 |
| Fredericksburg, VA | Richmond | 81.0 | 1 | 1 | 0 |
| Portsmouth, NH | Boston | 81.4 | 1 | 0 | 1 |
| Sandusky, OH | Cleveland | 81.7 | 1 | 0 | 0 |
| Beavercreek, OH | Cincinnati | 84.0 | 1 | 0 | 0 |
| Fayetteville, NC | Raleigh | 84.2 | 1 | 2 | 1 |
| Poland, OH | Pittsburgh | 84.9 | 1 | 0 | 0 |
| Niles, OH | Cleveland | 85.0 | 1 | 0 | 0 |
| Santa Fe, NM | Albuquerque | 85.7 | 1 | 0 | 1 |
| Lafayette, LA | Baton Rouge | 86.2 | 1 | 0 | 2 |
| Opelika, AL | Montgomery | 87.9 | 1 | 0 | 0 |
| Scotchtown, NY | New York | 88.2 | 1 | 0 | 0 |
| Westover, WV | Pittsburgh | 88.7 | 1 | 0 | 0 |
| Fort Collins, CO | Denver | 89.4 | 1 | 1 | 1 |
| Flint, MI | Detroit | 90.5 | 1 | 0 | 1 |
| Lafayette, IN | Indianapolis | 91.4 | 2 | 0 | 0 |
| Palm Desert, CA | Riverside | 92.4 | 1 | 0 | 1 |
| Bowling Green, KY | Nashville | 92.7 | 1 | 0 | 1 |
| Potomac Mills, VA | Baltimore | 92.7 | 1 | 0 | 0 |
| Burlington, WA | Seattle | 94.0 | 1 | 0 | 0 |
| Janesville, WI | Milwaukee | 94.9 | 1 | 0 | 0 |
| Oxford, AL | Birmingham | 94.9 | 1 | 0 | 0 |
| Athens-Clarke County, GA | Atlanta | 95.1 | 1 | 1 | 0 |
| Ontario, OH | Columbus | 97.2 | 1 | 0 | 0 |
| Temple, TX | Austin | 97.3 | 2 | 0 | 0 |
| St. Cloud, MN | Minneapolis | 97.8 | 1 | 0 | 0 |
| Normal, IL | Springfield IL | 100.7 | 1 | 0 | 0 |
| Sherman, TX | Dallas | 101.6 | 1 | 0 | 0 |
| Ocala, FL | Orlando | 101.8 | 1 | 1 | 0 |
| Concord, NH | Boston | 101.9 | 1 | 0 | 0 |
| Gainesville, VA | Baltimore | 102.5 | 1 | 1 | 0 |
| Topeka, KS | Kansas City | 102.6 | 1 | 0 | 0 |
| Brighton, NY | Buffalo | 104.1 | 1 | 0 | 0 |
| Watertown, NY | Syracuse | 104.4 | 1 | 0 | 0 |
| Mankato, MN | Minneapolis | 104.7 | 1 | 0 | 0 |
| Endwell, NY | Syracuse | 106.4 | 1 | 0 | 0 |
| Arlington Heights, PA | New York | 109.0 | 1 | 0 | 0 |
| Port Charlotte, FL | Tampa | 109.1 | 1 | 0 | 0 |
| California, MD | Baltimore | 110.7 | 1 | 0 | 0 |
| Logan, UT | Salt Lake City | 110.8 | 1 | 0 | 0 |
| Augusta-Richmond County, GA | Columbia SC | 111.1 | 1 | 0 | 0 |
| Sun Prairie, WI | Milwaukee | 111.2 | 1 | 0 | 0 |
| Grand Forks, ND | Fargo | 114.4 | 1 | 0 | 0 |
| Terre Haute, IN | Indianapolis | 114.5 | 1 | 0 | 0 |
| Big Flats, NY | Syracuse | 115.7 | 1 | 0 | 0 |
| Florence, SC | Columbia SC | 116.7 | 1 | 1 | 0 |
| Macon-Bibb County, GA | Atlanta | 117.0 | 1 | 1 | 0 |
| Palm Beach Gardens, FL | Miami | 118.6 | 1 | 0 | 1 |
| Rockford, IL | Chicago | 119.5 | 1 | 0 | 0 |
| Mishawaka, IN | Chicago | 121.5 | 1 | 0 | 0 |
| Lexington-Fayette, KY | Cincinnati | 122.1 | 2 | 0 | 0 |
| South Burlington, VT | Montreal (Canada) | 123.0 | 1 | 0 | 0 |
| Champaign, IL | Springfield IL | 125.4 | 1 | 0 | 0 |
| Sioux City, IA | Sioux Falls | 126.1 | 0 | 0 | 2 |
| Prescott, AZ | Phoenix | 127.1 | 1 | 0 | 0 |
| Chico, CA | Sacramento | 129.6 | 1 | 0 | 0 |
| Salisbury, MD | Baltimore | 132.9 | 1 | 0 | 0 |
| Erie, PA | Hamilton (Canada) | 134.7 | 1 | 0 | 0 |
| West Vero Corridor, FL | Orlando | 135.4 | 1 | 0 | 0 |
| Roanoke, VA | Winston-Salem | 136.9 | 1 | 0 | 0 |
| Santa Maria, CA | Bakersfield | 137.1 | 1 | 0 | 0 |
| Chattanooga, TN | Kennesaw | 137.2 | 1 | 0 | 2 |
| Clarksville, IN | Cincinnati | 138.3 | 1 | 0 | 0 |
| Wilkes-Barre, PA | Lancaster | 138.9 | 1 | 0 | 0 |
| Johnson City, TN | Knoxville | 143.5 | 1 | 0 | 0 |
| Waterloo, IA | Des Moines | 143.9 | 1 | 0 | 0 |
| Eau Claire, WI | Minneapolis | 146.2 | 1 | 0 | 0 |
| Dothan, AL | Montgomery | 147.9 | 2 | 0 | 0 |
| Tyler, TX | Dallas | 148.1 | 1 | 0 | 2 |
| Zilwaukee, MI | Detroit | 148.6 | 1 | 0 | 0 |
| Beechwood, MI | Milwaukee | 149.7 | 1 | 0 | 0 |
| San Luis Obispo, CA | Bakersfield | 151.6 | 1 | 0 | 0 |
| South Portland, ME | Boston | 152.7 | 1 | 0 | 0 |
| Tupelo, MS | Memphis | 154.4 | 1 | 0 | 0 |
| Cape Girardeau, MO | St. Louis | 157.5 | 1 | 0 | 0 |
| Lebanon, NH | Worcester | 157.6 | 1 | 0 | 0 |
| Victoria, TX | San Antonio | 158.0 | 1 | 0 | 0 |
| Harrisonburg, VA | Richmond | 158.7 | 1 | 0 | 0 |
| Indian Hills, NV | Sacramento | 159.8 | 1 | 0 | 0 |
| Dickson City, PA | New York | 160.5 | 1 | 0 | 0 |
| Naples, FL | Miami | 164.1 | 1 | 1 | 0 |
| Florence, AL | Birmingham | 165.0 | 1 | 0 | 0 |
| Yakima, WA | Tacoma | 166.9 | 1 | 0 | 0 |
| Coralville, IA | Des Moines | 168.1 | 1 | 0 | 0 |
| Valdosta, GA | Jacksonville | 168.8 | 1 | 0 | 0 |
| Joplin, MO | Tulsa | 169.9 | 1 | 0 | 1 |
| Baxter, MN | Minneapolis | 171.2 | 2 | 0 | 0 |
| Fort Wayne, IN | Indianapolis | 171.3 | 2 | 2 | 1 |
| Bristol, TN | Knoxville | 171.8 | 1 | 0 | 1 |
| Fort Smith, AR | Tulsa | 172.1 | 2 | 0 | 0 |
| Battle Creek, MI | Detroit | 175.5 | 1 | 0 | 0 |
| Grandville, MI | Milwaukee | 176.1 | 1 | 0 | 1 |
| St. George, UT | Las Vegas | 177.1 | 1 | 1 | 0 |
| Owensboro, KY | Nashville | 177.3 | 1 | 1 | 0 |
| Reno, NV | Sacramento | 179.0 | 1 | 2 | 1 |
| Twin Falls, ID | Boise | 180.4 | 1 | 0 | 0 |
| Lufkin, TX | Houston | 183.4 | 1 | 0 | 0 |
| Traverse City, MI | Green Bay | 189.3 | 1 | 0 | 0 |
| Kentwood, MI | Milwaukee | 191.0 | 2 | 0 | 0 |
| Elizabethtown, KY | Nashville | 191.6 | 1 | 0 | 0 |
| Bend, OR | Portland | 192.7 | 1 | 0 | 1 |
| Paducah, KY | Nashville | 193.0 | 1 | 1 | 0 |
| Bluffton, SC | Columbia SC | 194.8 | 1 | 0 | 0 |
| Longview, TX | Dallas | 194.8 | 1 | 0 | 0 |
| Meridian, MS | Pensacola | 195.4 | 1 | 0 | 0 |
| Lake Charles, LA | Baton Rouge | 196.3 | 0 | 1 | 1 |
| Flagstaff, AZ | Phoenix | 199.4 | 1 | 0 | 2 |
| Myrtle Beach, SC | Columbia SC | 200.1 | 1 | 0 | 0 |
| Onalaska, WI | Minneapolis | 205.1 | 1 | 0 | 0 |
| Grand Island, NE | Omaha | 208.4 | 1 | 0 | 0 |
| Corpus Christi, TX | San Antonio | 208.9 | 1 | 1 | 1 |
| Davenport, IA | Springfield IL | 211.7 | 1 | 0 | 0 |
| Charleston, WV | Columbus | 212.9 | 1 | 0 | 0 |
| Evansville, IN | Nashville | 213.4 | 1 | 1 | 0 |
| McAllen, TX | Monterrey (Mexico) | 216.2 | 3 | 0 | 0 |
| Texarkana, AR | Little Rock | 219.3 | 1 | 0 | 0 |
| Duluth, MN | Minneapolis | 220.9 | 1 | 0 | 0 |
| Yuma, AZ | Tijuana (Mexico) | 225.0 | 1 | 0 | 1 |
| Abilene, TX | Fort Worth | 227.6 | 1 | 1 | 0 |
| Panama City, FL | Pensacola | 234.6 | 1 | 0 | 0 |
| Redding, CA | Sacramento | 234.6 | 1 | 0 | 0 |
| Augusta, ME | Boston | 241.4 | 2 | 0 | 0 |
| Tallahassee, FL | Jacksonville | 250.8 | 1 | 1 | 2 |
| Kennewick, WA | Tacoma | 274.0 | 1 | 1 | 1 |
| Bossier City, LA | Little Rock | 276.8 | 1 | 0 | 0 |
| Casper, WY | Rapid City | 280.1 | 1 | 0 | 0 |
| Shreveport, LA | Dallas | 284.6 | 1 | 2 | 1 |
| Bangor, ME | Quebec City (Canada) | 291.1 | 1 | 0 | 0 |
| San Angelo, TX | Austin | 293.5 | 1 | 0 | 0 |
| Bismarck, ND | Fargo | 303.5 | 1 | 0 | 2 |
| Kalispell, MT | Calgary (Canada) | 312.7 | 1 | 0 | 0 |
| Grand Junction, CO | Denver | 317.7 | 1 | 0 | 0 |
| Medford, OR | Portland | 350.2 | 1 | 0 | 1 |
| Odessa, TX | El Paso | 392.4 | 1 | 0 | 0 |
| Amarillo, TX | Oklahoma City | 397.9 | 1 | 3 | 1 |
| Missoula, MT | Boise | 400.7 | 1 | 0 | 1 |
| Lubbock, TX | Fort Worth | 436.3 | 1 | 0 | 0 |
| Billings, MT | Rapid City | 459.9 | 1 | 0 | 2 |
| Bozeman, MT | Boise | 468.6 | 1 | 0 | 0 |

### Canada — 56 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Burlington | Hamilton | 12.9 | 2 | 0 | 1 |
| Sherwood Park | Edmonton | 13.3 | 2 | 0 | 0 |
| Saint-Bruno-de-Montarville, QC | Montreal | 14.4 | 1 | 0 | 0 |
| St. Albert, AB | Edmonton | 14.5 | 1 | 0 | 0 |
| Laval | Montreal | 15.3 | 1 | 1 | 0 |
| Pointe-Claire | Montreal | 20.0 | 1 | 0 | 0 |
| Brantford, ON | Kitchener | 20.6 | 1 | 0 | 0 |
| Guelph, Ontario | Kitchener | 21.1 | 1 | 1 | 1 |
| Vaughan, Ontario | Toronto | 21.1 | 3 | 1 | 0 |
| Coquitlam, BC | Vancouver | 21.5 | 2 | 0 | 0 |
| Waterloo, ON | Kitchener | 22.8 | 2 | 1 | 0 |
| Markham | Toronto | 23.1 | 2 | 0 | 1 |
| Mississauga, ON | Toronto | 24.4 | 4 | 1 | 1 |
| Boisbriand, QC | Montreal | 25.2 | 1 | 0 | 0 |
| Surrey | Vancouver | 25.9 | 4 | 0 | 1 |
| Ajax, ON | Toronto | 37.2 | 1 | 0 | 0 |
| Langley District Municipality | Vancouver | 37.7 | 1 | 0 | 0 |
| Okotoks | Calgary | 38.6 | 1 | 0 | 0 |
| Vaudreuil-Dorion, Québec | Montreal | 38.8 | 1 | 0 | 0 |
| Newmarket, ON | Toronto | 46.2 | 2 | 0 | 0 |
| Oshawa, ON | Toronto | 50.9 | 2 | 0 | 0 |
| Orangeville | Toronto | 65.1 | 1 | 0 | 0 |
| Abbotsford, BC | Vancouver | 65.9 | 2 | 0 | 0 |
| Nanaimo, British Columbia | Vancouver | 67.0 | 1 | 0 | 0 |
| Barrie, ON | Toronto | 83.7 | 2 | 0 | 0 |
| Chilliwack, BC | Vancouver | 85.1 | 1 | 0 | 0 |
| Cornwall, Ontario | Ottawa | 85.6 | 1 | 0 | 0 |
| London | Kitchener | 86.6 | 3 | 0 | 4 |
| Drummondville, Québec | Montreal | 92.5 | 1 | 0 | 0 |
| Langford | Vancouver | 96.8 | 1 | 0 | 0 |
| Orillia, ON | Toronto | 107.1 | 1 | 0 | 0 |
| Peterborough, ON | Toronto | 110.7 | 1 | 0 | 1 |
| Sherbrooke, Québec | Montreal | 125.4 | 1 | 0 | 0 |
| Saint John | Moncton | 134.0 | 1 | 1 | 0 |
| Red Deer, AB | Calgary | 136.1 | 1 | 1 | 0 |
| Kingston, ON | Syracuse (United States) | 138.6 | 1 | 0 | 0 |
| Courtenay | Vancouver | 141.7 | 1 | 1 | 1 |
| Fredericton | Moncton | 145.2 | 1 | 0 | 1 |
| Belleville, ON | Syracuse (United States) | 162.2 | 1 | 0 | 0 |
| Lethbridge, AB | Calgary | 176.1 | 1 | 0 | 1 |
| Chicoutimi, Québec | Quebec City | 176.8 | 1 | 0 | 0 |
| Brandon, MB | Winnipeg | 202.2 | 1 | 0 | 1 |
| Lloydminster | Edmonton | 231.4 | 1 | 1 | 0 |
| Kamloops, BC | Vancouver | 248.9 | 1 | 0 | 0 |
| Medicine Hat, AB | Calgary | 268.4 | 1 | 0 | 0 |
| Kelowna, BC | Vancouver | 274.5 | 1 | 0 | 0 |
| North Bay | Toronto | 296.8 | 1 | 0 | 1 |
| Vernon | Vancouver | 298.1 | 1 | 0 | 0 |
| Greater Sudbury, ON | Toronto | 338.2 | 2 | 0 | 0 |
| Grande Prairie, AB | Edmonton | 389.5 | 1 | 1 | 0 |
| Thunder Bay | Green Bay (United States) | 442.3 | 1 | 1 | 0 |
| Saskatoon | Edmonton | 485.9 | 1 | 1 | 2 |
| Prince George, BC | Vancouver | 511.2 | 1 | 0 | 0 |
| Prince Albert, SK | Edmonton | 515.7 | 1 | 0 | 0 |
| Regina, SK | Winnipeg | 534.8 | 2 | 1 | 0 |
| Timmins, Ontario | Ottawa | 549.3 | 1 | 0 | 0 |

### Mexico — 46 markets

| Market | Metropolitan reference | km | T1 | T2 | T3 |
|---|---|---|---|---|---|
| Santa Catarina | Monterrey | 12.2 | 1 | 1 | 0 |
| Naucalpan de Juárez | Mexico City | 12.8 | 1 | 1 | 1 |
| Álvaro Obregón | Mexico City | 12.9 | 3 | 0 | 1 |
| Apodaca, Nuevo León | Monterrey | 13.5 | 1 | 1 | 2 |
| Tlajomulco de Zúñiga | Guadalajara | 14.4 | 1 | 0 | 2 |
| Playas de Rosarito | Tijuana | 15.0 | 1 | 0 | 0 |
| Tlalnepantla de Baz | Mexico City | 15.4 | 2 | 0 | 1 |
| Tlalpan | Mexico City | 15.5 | 1 | 0 | 1 |
| Ecatepec de Morelos | Mexico City | 19.0 | 1 | 0 | 5 |
| Texcoco, MX | Mexico City | 25.3 | 1 | 0 | 1 |
| Ixtapaluca | Mexico City | 30.3 | 1 | 0 | 0 |
| Tulancingo de Bravo | Pachuca | 39.2 | 1 | 0 | 0 |
| Celaya, Guanajuato | Querétaro | 44.6 | 2 | 0 | 0 |
| Toluca | Mexico City | 55.1 | 1 | 0 | 3 |
| Solidaridad | Cancún | 63.3 | 2 | 0 | 1 |
| Delicias | Chihuahua | 78.2 | 1 | 0 | 0 |
| Ensenada | Tijuana | 83.3 | 1 | 0 | 1 |
| Uruapan | Morelia | 94.9 | 1 | 0 | 0 |
| Zapotlán el Grande | Guadalajara | 108.2 | 1 | 0 | 1 |
| Zamora | Morelia | 119.8 | 1 | 0 | 1 |
| Córdoba | Puebla | 133.4 | 1 | 0 | 1 |
| Poza Rica de Hidalgo | Pachuca | 145.7 | 1 | 0 | 1 |
| Xalapa, Veracruz | Puebla | 146.9 | 1 | 0 | 3 |
| Fresnillo | Aguascalientes | 156.7 | 1 | 0 | 0 |
| Chilpancingo de los Bravo | Cuernavaca | 157.7 | 1 | 0 | 0 |
| Tepic | Guadalajara | 184.6 | 1 | 0 | 1 |
| Salina Cruz | Oaxaca | 186.7 | 1 | 0 | 0 |
| Cajeme | Hermosillo | 201.4 | 1 | 0 | 1 |
| Ciudad Valles | San Luis Potosí | 204.9 | 1 | 0 | 1 |
| Reynosa | Monterrey | 205.2 | 1 | 0 | 3 |
| Veracruz | Puebla | 213.0 | 1 | 0 | 6 |
| Boca del Río | Puebla | 219.8 | 2 | 0 | 0 |
| Acapulco de Juárez | Cuernavaca | 242.8 | 1 | 0 | 3 |
| Victoria | Monterrey | 244.8 | 1 | 0 | 1 |
| Tampico | Pachuca | 257.3 | 1 | 0 | 1 |
| Coatzacoalcos | Oaxaca | 265.5 | 1 | 0 | 1 |
| Centro | Campeche | 325.5 | 2 | 0 | 2 |
| Durango | Aguascalientes | 339.0 | 1 | 0 | 2 |
| Tuxtla Gutiérrez | Oaxaca | 385.8 | 2 | 0 | 0 |
| Ahome | Hermosillo | 412.2 | 1 | 0 | 0 |
| Mazatlán | Guadalajara | 428.2 | 1 | 0 | 2 |
| Comitán de Domínguez | Campeche | 434.3 | 1 | 0 | 1 |
| Culiacán, Sinaloa | Chihuahua | 448.3 | 2 | 0 | 2 |
| Tapachula | Oaxaca | 534.8 | 1 | 0 | 1 |
| La Paz | Hermosillo | 553.6 | 1 | 0 | 1 |
| Los Cabos | Hermosillo | 694.2 | 0 | 0 | 3 |

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

AI assistance was used in preparing and revising this paper.

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
list. The figures describe the current dataset build; a September 2026 rebuild superseded an
earlier and incomplete selection of 369 United States, 23 Canadian and 8 Mexican markets, so
any copy of this list carrying those counts is a stale one. The set is a curated editorial
selection derived from the live market layer and does not replace or alter that layer, which
remains unranked and uncurated at its full qualifying count of 1,121. Counts move between
builds as chain coverage grows and as clusters re-form, so this is a dated snapshot rather than
a permanent statement. Market display names are reproduced as the underlying settlement records
carry them, including inconsistent use of state and province suffixes; no market's identity or
geography has been altered. No independent party has audited this dataset, reproduced these
figures, or reviewed these claims.

Woodfine Capital Projects™ is a trademark of Woodfine Capital Projects Inc.
