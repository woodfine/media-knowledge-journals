---
schema: journal-v2
slug: aec-data-layers
title: "Open-Licence Building-Data Coverage for Site Analysis, Across Sixteen Countries"
subtitle: "Which regulatory-grade geospatial inputs are actually open, and where the real gaps are"
site: gis.woodfinegroup.com
imprint: WCP-2026-03
thesis: "Regulatory-grade geospatial data for building design is openly available for most of what a site evaluator needs, in most of the countries studied — but three specific, structural gaps remain, and no prior comparison had actually mapped where they are."
abstract: |
  Anyone evaluating a commercial building site needs a specific set of regulatory inputs —
  building-code climate zone, flood hazard designation, seismic ground acceleration, solar
  potential, and several others — and each one is normally sourced country by country, agency
  by agency, with no single comparison of which of these are actually open and usable across
  jurisdictions. We built that comparison directly: an eight-category taxonomy of the
  regulatory geospatial inputs a large building project actually needs, assessed across sixteen
  countries in North America and Europe on a simple three-level scale — genuinely
  regulatory-grade and open, a workable proxy, or not available at all. The headline finding is
  that most of what matters is available: the United States has fully open, regulatory-grade
  data for all four of the highest-priority categories, and eight European countries can
  produce regulatory-grade building-climate-zone data by joining each country's own energy
  code to its municipal boundaries, even though no single European-wide climate-zone map
  exists. Three real, structural gaps remain: Canada has no national flood-hazard layer at all;
  Mexico's most precise environmental data carries a licence that blocks commercial use;
  and United States wind and snow-load design maps are copyrighted and cannot be freely
  redistributed. The main limitation: the coverage assessment itself is documentary — built
  from reading each source's actual licence and regulatory status — rather than a completed
  run of the data pipeline against every study country, which remains a real, stated next step.
state: draft
version: "1.0.0"
published:
updated: "2026-09-15"
doi:
license: CC-BY-4.0
cites:
  - taylor-2008-climate-zones
  - alphen-lodder-2006-flood-planning
  - haklay-2010-vgi-quality
  - brodsky-2018-h3
  - dinerstein-2017-ecoregions
  - eu-floods-directive-2007-60
  - eu-epbd-2010-31
  - wri-aqueduct-floods-2023
draws_from: []
contributors:
  - name: Peter M. Woodfine
    roles: [Founding Contributor]
  - name: Jennifer M. Woodfine
    roles: [Founding Contributor]
  - name: Mathew Woodfine
    roles: [Founding Contributor]
keywords:
  - AEC site analysis
  - building code climate zones
  - open geospatial data
  - flood hazard
  - continental-scale coverage
---

## 1. The question

Designing a large commercial building requires a specific, well-defined set of regulatory
inputs before design work can even begin: a building-code climate zone for HVAC and envelope
design, a flood-hazard designation that can trigger mandatory insurance and elevation
requirements, a seismic ground-acceleration value that drives structural system selection, and
a solar-potential figure for energy code compliance and photovoltaic sizing. Each of these
inputs is public information, funded by a government agency, in most of the countries where
large commercial development happens. What has never existed, as far as we can find, is a
single, systematic comparison of which of these inputs are actually open — meaning freely
usable, including commercially, without a proprietary licence blocking redistribution — across
a meaningful set of countries at once.

The absence of that comparison has a real practical consequence. A site-evaluation platform
serving multiple countries either defaults to United States data, because that is where the
comparison has been done informally many times over, or substitutes a coarse global proxy
(a generic climate classification, a generic flood-risk index) without being explicit about
what precision or regulatory standing was traded away to get continental coverage. Someone
evaluating a site in Madrid deserves to know, plainly, whether the data behind that
evaluation is the same regulatory-grade input a Spanish engineer would actually use, or a
global approximation standing in for it.

The question this paper answers is direct: across eight categories of regulatory geospatial
data and sixteen countries in North America and Europe, what is actually open, what is a
workable but lower-precision proxy, and where is there genuinely nothing usable at all? And
having answered that, can the open and proxy layers actually be joined, in practice, to a
map of real building sites, using a method that does not require sixteen separate,
one-off integration efforts?

## 2. What we found

**Most of what a site evaluator needs is genuinely open, in most of the countries studied.**
Of the eight data categories assessed, five achieve regulatory-grade open status in at least
six of the sixteen countries. Two categories — seismic hazard and solar potential — are
covered, at least at a workable regulatory or near-regulatory standard, in literally every one
of the sixteen countries, because both are served by continent-wide open programs (the United
States Geological Survey's hazard model domestically, the European Seismic Hazard Model and
the EU's own solar-potential service across Europe) that do not depend on any single country
publishing its own layer.

**The United States has complete, regulatory-grade coverage across all four of the
highest-priority categories** — climate zone, flood hazard, seismic hazard, and solar
potential — each one sourced from the exact federal agency or program that is actually cited
in US building code and permitting practice, not a proxy standing in for it.

**Europe's situation is more interesting than "less complete," because it required a real
methodological workaround rather than accepting a downgrade.** No single, European-wide
building-climate-zone map exists, because unlike the United States, each European country
defines its own national energy code independently. Rather than falling back to a coarse
global climate classification for the whole continent, the approach we took joins each
country's own national energy-code climate zones directly to that country's own municipal
boundary data. This produces a genuinely regulatory-grade result — the actual zone a national
engineer would use — for eight of the European countries studied, and it does so without
requiring a single harmonized European standard to exist first. The remaining European
countries in the study either use a single nationwide zone (making a zone map unnecessary) or
require a data-registration step we have not yet completed.

**Three real, structural gaps remain, and each has a genuinely different cause.** Canada
currently has no national, regulatory flood-hazard layer at all — the program meant to produce
one is still underway, and the best available substitute today is a modelled prediction, not a
regulatory product, a distinction worth stating plainly to anyone using it. Mexico's most
precise environmental and climate classification data exists but carries a licence that
specifically excludes commercial use, which is a real barrier for anyone building a commercial
product on top of it, not merely an inconvenience — a lower-precision, commercially-usable
global substitute exists, but it is a genuine downgrade in precision for Mexican sites
specifically. United States wind-speed and snow-load design values, unlike the other Tier 1
categories, are copyrighted by the standards body that publishes them, meaning they cannot be
freely redistributed as a map layer at all — the workable approach is a live, point-in-time
lookup against the standards body's own compliant API, rather than a downloadable dataset,
which is a structurally different (and slower, externally-dependent) integration pattern than
every other layer in this study.

## 3. How we assessed it

The assessment method is documentary, not a live pipeline run, and we want to be direct about
that distinction rather than let the word "assessment" imply more than it means here. For each
of the eight data categories, in each of the sixteen countries, we identified the actual
source agency or program, read its stated licence terms, and classified the result on a simple
three-level scale: genuinely regulatory-grade and open (explicitly the source cited in an
actual building code, flood-insurance program, or compliance standard, usable commercially
without restriction); a workable proxy (a coarser, global, or otherwise lower-precision
substitute, still usable, but not the exact regulatory-grade input a local professional would
cite); or not available at all under any open licence. This produces a 128-cell scorecard —
eight categories across sixteen countries — that is, as far as we have found, the first
systematic version of this specific comparison to exist.

Separately from the licence and precision assessment, we specified an integration method for
actually joining these layers to a map of real building sites at scale, rather than treating
each country as its own one-off project. The method uses a single, consistent spatial grid
(H3 hexagonal cells at a resolution of roughly 1.2 square kilometres per cell) as the common
key every layer is joined against, regardless of whether the underlying data arrives as a
polygon map, a continuous raster surface, or a single number attached to a point. This gives
every country the same integration pattern, differing only in which raw source feeds it, which
is what makes a sixteen-country (and, in principle, larger) comparison practical to maintain
rather than requiring a bespoke pipeline per country.

We want to state plainly what this paper does not yet include: a completed run of that
integration pipeline against real site data for all sixteen countries, producing an actual
count of how many real sites fall into each coverage category per country. The licence and
regulatory-standing assessment in §2 is complete and does not depend on that run. The
per-country site counts do, and are not yet available — we say so directly rather than
presenting a documentary assessment as if it were a completed empirical count.

## 4. What it changes

For anyone evaluating development sites across more than one country, the practical change is
knowing, country by country and category by category, whether the data behind a site
evaluation is the actual regulatory input a local professional would use, or a lower-precision
substitute standing in for it — and knowing this before relying on the evaluation for a real
decision, not after. A flood-hazard designation sourced from the actual national regulatory
program carries real, checkable regulatory weight; one sourced from a global proxy layer does
not, and treating the two as equivalent risks a real, costly surprise later in a project's
permitting process.

The European climate-zone finding changes something more specific: it shows that the absence
of a single continental standard does not require falling back to a coarse global
approximation. Joining each country's own real national standard to its own municipal
boundaries produces a genuinely regulatory-grade result without waiting for European-wide
harmonization that may never happen. This is a reusable pattern, not a one-off fix — any
category where individual countries maintain their own regulatory standard, without a
continental equivalent, is a candidate for the same join-based approach rather than a global
proxy.

The three structural gaps change what an evaluator should expect and disclose for sites in the
affected countries specifically: a Canadian flood assessment today is a modelled prediction,
not a regulatory determination, and should be presented as such; a Mexican eco-region or
precision-climate assessment using the open substitute is a real but lower-precision stand-in
for data that exists but cannot be redistributed commercially; and any wind or snow load figure
for a US site needs to come from a live, compliant lookup rather than a static map, because no
static, freely-redistributable map of that data can legally exist.

## 5. Where this could be wrong

**The coverage assessment is documentary, not empirically validated against real site data
yet.** As stated directly in §3, the per-country counts of how many real sites actually fall
into each coverage category await a completed pipeline run. The licence and regulatory-status
findings do not depend on that run and are not affected by this limitation, but anyone wanting
an empirical count of affected sites, rather than a category-level assessment, should treat
that as a planned next step, not a current result.

**The European climate-zone method is a derived result, not a native regulatory publication,
and inherits a real maintenance obligation.** Because the method depends on joining each
country's own lookup table to municipal boundary data, any error in that lookup table, or any
update to a country's national energy code, requires the join to be updated before it reflects
the current regulatory reality. This is a structural, ongoing cost of the method, not a
one-time limitation.

**Coverage assessments for smaller or less-studied countries carry more uncertainty than the
larger ones.** The sixteen study countries include several with a single, simpler national
standard and correspondingly less to assess; the depth of documentary research behind each
country's row in the scorecard is not perfectly uniform, and a country assessed as fully
covered on a simpler standard is a different kind of finding than the United States' coverage
of four independently complex regulatory systems.

**Redistribution licence terms can change.** Several of the "open" classifications in this
assessment depend on a specific agency's current licence terms remaining as documented; a
licence change at the source would require the corresponding cell in the scorecard to be
re-assessed, not assumed to remain valid indefinitely.

## 6. Conclusion

The question was whether regulatory-grade geospatial data for commercial building design is
actually open, across a meaningful set of countries, in a form that can be compared and
integrated consistently rather than assessed one country at a time. It largely is: five of
eight data categories are regulatory-grade and open in at least six of sixteen countries
studied, two categories are covered continent-wide in every country studied, and the United
States and eight European countries achieve full or near-full regulatory-grade coverage across
the highest-priority categories — Europe's result achieved specifically by joining each
country's own real standard to its own boundaries, rather than by a continental map that does
not exist. Three real, structural gaps remain, each with a different cause and a different
practical workaround. What is not yet done is turning this documentary assessment into a
completed, per-country empirical count against real site data — a real, stated next step, not
a result already in hand.

---

## 7. Claims and what would count against them

**H1 (coverage).** At least six of the eight data categories can be sourced from open,
commercially-usable licences in at least eight of the sixteen study countries.

**H2 (US regulatory-grade).** All four Tier 1 categories — climate zone, flood hazard,
seismic hazard, solar potential — are available for the United States from the actual source
each is cited from in real code-compliance and permitting practice.

| Test | What it checks | Status |
|---|---|---|
| Coverage count | H1: at least 6 of 8 categories reach open status in at least 8 of 16 countries | Passed under the documentary assessment in §2; not yet re-verified against a completed pipeline run |
| US regulatory-grade confirmation | H2: each US Tier 1 source is the one actually cited in permitting practice, not a proxy | Passed under direct source verification |
| Licence-compatibility check | No layer with a non-commercial or share-alike licence enters the production pipeline undocumented | Designed; to be re-run whenever a new layer is added |
| Reproducibility check | Rebuilding the pipeline from the documented source URLs produces the same output | Designed; not yet executed end to end |
| European join-accuracy check | Spot-checking a sample of municipal centroids against each country's own official climate-zone publication | Designed; not yet executed |

H1 is falsified if fewer than six categories reach open status in at least eight countries.
H2 is falsified if any of the four cited US sources is found not to be the one actually used
in real permitting practice.

### Appendix A — The eight data categories

Building-code climate zone, flood hazard zone, seismic ground acceleration, solar potential,
eco-region/landscape reference zones, wind and snow design load, wildfire hazard, and soil
classification — ranked by how directly each is cited in a binding building code, flood
program, or environmental compliance standard, from most to least code-prescriptive.

### Appendix B — Structural gaps, in brief

Canada: no national regulatory flood-hazard layer yet exists; a modelled prediction is the
current substitute. Mexico: precision eco-region and climate data exist but carry a
non-commercial licence; a lower-precision, commercially-usable global substitute is used
instead. United States: wind and snow design-load maps are copyrighted by their publishing
standards body and cannot be freely redistributed; a live, compliant point-lookup API is the
workable alternative to a static map.

## References

Alphen, J. van, and W. Lodder. 2006. Flood risk mapping in the Netherlands and abroad.
*International Symposium on Flood Defence.*

Brodsky, E. 2018. H3: Uber's hexagonal hierarchical spatial index. *Uber Engineering.*

Dinerstein, E., et al. 2017. An ecoregion-based approach to protecting half the terrestrial
realm. *BioScience* 67(6): 534–545.

Haklay, M. 2010. How good is volunteered geographical information? *Environment and Planning
B: Planning and Design* 37(4): 682–703.

Taylor, Z. T., et al. 2008. ANSI/ASHRAE/IESNA Standard 90.1-2007 climate zones. *Pacific
Northwest National Laboratory.*

---

## Contributors

Peter M. Woodfine, Jennifer M. Woodfine, and Mathew Woodfine are credited as founding
contributors to Woodfine Capital Projects Inc.'s geographic-intelligence research programme.

## How this paper was produced

This paper was prepared with AI assistance under human editorial direction; all analytical
claims and conclusions are the responsibility of the named institutional author.

## Disclosures

The integration pipeline this paper describes is built and operated by an affiliate of the
paper's author, Woodfine Capital Projects Inc. All source data referenced is public; licence
terms and source agencies are documented in Appendix B and are independently verifiable. This
paper contains forward-looking statements about a planned completed pipeline run; such
statements reflect current intentions and are subject to change without notice.

## Data and reproducibility

Every data source referenced in this paper is public and independently obtainable from its
named source agency. The three-level coverage classification and the H3-based integration
method are described in full in §3 and are reproducible by any researcher with access to the
same public sources.
