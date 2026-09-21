---
schema: journal-v2
slug: open-regulatory-site-data
title: "How Much Regulatory Site Data Is Actually Open and Usable"
subtitle: "A cell-by-cell coverage scorecard across eight kinds of data and sixteen countries, gaps included"
site: gis.woodfinegroup.com
imprint: WCP-003
thesis: "The public availability of the regulatory data a building site decision depends on is uneven between countries and between kinds of data, and publishing that unevenness cell by cell serves a reader better than a single figure that hides which country and which risk is actually covered."
abstract: |
  Our thesis is that a coverage scorecard a reader can check cell by cell is worth more than
  an average that hides where the holes are. Evaluating a commercial building site needs a
  specific set of public inputs — the climate zone the energy code assigns, the flood
  designation that can trigger insurance and elevation requirements, the seismic value that
  drives the structure, the wind and snow loads, and several more. Each is normally chased
  country by country and agency by agency. We built the comparison instead: eight categories
  of regulatory geospatial data across sixteen countries in North America and Europe, each
  cell graded on a three-level scale — genuinely regulatory-grade and openly licensed, a
  workable lower-precision substitute, or nothing usable at all. Most of what matters is
  open. Seismic and solar data reach at least a workable standard in every one of the
  sixteen countries, and the United States has regulatory-grade open data for all four of
  the highest-priority categories. Three gaps are structural and each has a different cause:
  Canada has no national regulatory flood-hazard layer; Mexico's most precise environmental
  data carries a licence excluding commercial use; and United States wind and snow design
  values are copyrighted and cannot be redistributed as a map at all. The main limitation is
  stated plainly rather than implied: this assessment is documentary — it reads each source's
  licence and regulatory standing — and is not a completed pipeline run counting how many
  real sites fall into each coverage category per country.
state: draft
version: "0.1.0"
published:
updated: "2026-09-16"
cite_as:
license: CC-BY-4.0
cites:
  - taylor-2008-climate-zones
  - ashrae-90-1
  - nbc-2020
  - eu-epbd-2010-31
  - eu-floods-directive-2007-60
  - alphen-lodder-2006-flood-planning
  - baugh-2016-lisflood-fp
  - wri-aqueduct-floods-2023
  - dinerstein-2017-ecoregions
  - buchhorn-2020-copernicus-land-cover
  - brodsky-2018-h3
  - haklay-2010-osm-quality
  - osm-odbl
draws_from:
  - about-regional-markets-system
  - gis-data-overview
  - zoning-acquisition-rules
  - trade-area-data-sources
  - spend-population-provenance
  - co-location-intelligence-overview
prepared_by: "Woodfine Management Corp."
keywords:
  - open geospatial data
  - building codes
  - flood hazard
  - data licensing
  - site assessment
---

> Nothing in this paper constitutes an offer to sell, or a solicitation of an offer to buy,
> any interest in a Woodfine direct-hold solution; any offering is made only by the
> applicable Private Placement Memorandum. Statements marked "planned," "intended,"
> "targeted," "may," or "expected" are forward-looking and subject to change. Full
> disclosures appear at the end of this paper.

Working Paper WCP-003 · v0.1.0 · CC BY 4.0

Our thesis is that when the public data behind a site assessment is uneven between countries,
the right thing to publish is the unevenness itself — country by country and category by
category — rather than an average that hides it. For some of the countries this platform
covers, essentially all of the regulatory information a building decision depends on is open
and machine-readable. For others, essentially none of it is. That is an awkward fact to state
plainly, and stating it plainly is the whole point of this paper.

The practical stake for a reader is direct. Told that a site in Spain and a site in Canada
have both been "assessed," you would reasonably assume the two assessments rest on the same
kind of evidence. They do not. The Canadian one is missing a flood layer that does not exist
in any national regulatory form. The Spanish one is drawing on a national energy-code climate
zone that is genuinely the figure a Spanish engineer would use. The two assessments are not
equivalent, and nothing in a summary score would tell you so.

This paper describes a coverage scorecard built the same way for every jurisdiction: eight
categories of regulatory data, sixteen countries, and one of three verdicts in each cell. It
reports what is open, what is a workable substitute, and where there is nothing at all. It is
a documentary exercise — a catalogue of what is publicly available and on what licence — and
it is not an empirical claim about how buildings perform. One category a reader might expect
to find here is deliberately absent, and Section Five explains why.

## 1. The thesis

A single number is the wrong shape for this information.

Suppose a platform reported that it had "87 per cent coverage" of the regulatory data behind
its site assessments. That figure would be true and useless. It would not tell you whether the
missing 13 per cent is scattered evenly — a little thin everywhere, no particular problem — or
concentrated entirely in one country's flood data, which would make every flood claim about
that country worthless. It would not tell you whether the covered 87 per cent is the actual
regulatory input a local engineer would cite or a coarse global stand-in wearing the same
label. And it would give a reader no way to check any of it.

A scorecard reports the same information in a form that can be interrogated. Each cell names
a country, a category of data, a source, a licence, and a verdict. A reader who cares about
one country and one risk can go to that cell, read the source it names, and form their own
view. A reader who wants the summary can still take it, but the summary is derived from
visible parts rather than standing in for them.

The composition is the claim. Each individual assessment in this scorecard is unremarkable:
somebody reads an agency's licence page and decides whether the data can be used. What did
not exist, so far as we can find, is the systematic version — the same eight questions asked
of the same sixteen countries at once, published with the failures in it. That is the
contribution, and it is a modest one by design.

## 2. The problem, in the reader's terms

Two documents will help.

The first is a used-car inspection certificate — the single sticker or one-page report saying
the vehicle has been "certified." It gives you one verdict. You do not know what was checked,
what was checked cursorily, what could not be checked because the part was inaccessible, or
what the inspector's standard was. You are trusting a person you have not met and a process
you cannot see. If the car turns out to have a rusted subframe, the certificate offers you
nothing, because it never said anything specific enough to be wrong.

The second is the same car's full service history: a stack of dated entries, each naming a
garage, a date, a mileage and a job. It is more work to read. It is also checkable line by
line, and its gaps are visible — you can see that nothing was done for four years between two
entries, which is itself information. Nobody has to be trusted, because nothing has been
summarised.

Site-assessment data has the same two forms available. The first is a consultant's report
saying a jurisdiction has been assessed, without naming which public records the assessment
actually drew on. The second is a scorecard saying: in this country, the building-code climate
zone came from the national energy code and is the figure an engineer there would cite; the
flood designation came from a global modelled index rather than a national regulatory
programme, and is a substitute; the seismic value came from the continental hazard model. Same
subject, entirely different relationship to the reader.

The reason this matters more than it looks is that the difference between a regulatory-grade
input and a workable substitute is not a difference of accuracy. It is a difference of
standing. A flood designation issued by a national regulatory programme carries weight in a
permit application, an insurance negotiation and a lender's file. A modelled global flood
index does not, however good the model. Treating the two as interchangeable is fine right up
until the point in a project where somebody asks which one you used.

## 3. What a site decision actually needs before design begins

A reader outside this industry may not know what is meant by "regulatory site data," so this
section establishes the vocabulary before the results.

Before an architect draws anything for a large commercial building, a specific set of facts
about the place has to be established, because each one changes the building. They are not
matters of preference and they are not negotiable; a building designed against the wrong ones
will not be approved.

**The building-code climate zone** determines the heating, ventilation and air-conditioning
system and the performance of the walls and roof. It is not the weather — it is a formal
classification assigned by an energy code, and a building's required insulation, glazing and
equipment follow from it. In the United States the classification traces to a documented
methodology developed for the national energy standard [taylor-2008-climate-zones]
[ashrae-90-1]. In Europe each country defines its own under a European framework
[eu-epbd-2010-31]; in Canada the national building code sets the equivalent [nbc-2020].

**The flood hazard designation** says whether the site sits in a mapped flood zone. The
consequences are immediate and expensive: mandatory insurance, a minimum floor elevation, a
restriction on what may be placed at ground level, and in some jurisdictions a refusal. In
Europe a directive obliges member states to produce flood hazard and risk maps
[eu-floods-directive-2007-60]. National practice in producing them varies considerably even
under a common obligation [alphen-lodder-2006-flood-planning].

**The seismic ground acceleration** is a number describing how hard the ground is expected to
shake at that location over a defined period. It drives the structural system, and the
difference between two values can be the difference between a conventional frame and a
substantially more expensive one.

**The solar potential** figure feeds energy-code compliance and the sizing of any rooftop
generation.

Four further categories complete the set: **eco-region and landscape reference zones**, which
govern landscaping, drainage and environmental compliance; **wind and snow design loads**,
which size the roof and the structure; **wildfire hazard**; and **soil classification**, which
determines the foundation. Eight in total, ordered by how directly each is cited in a binding
code or compliance standard rather than by how interesting it is.

Each of these is public information in most countries where large commercial development
happens, produced and funded by a government agency. "Public" and "usable" are not the same
thing, which is the subject of the next section.

## 4. What the scorecard measures, and what each verdict means

For each of the eight categories, in each of the sixteen countries, the assessment identifies
the actual source agency or programme, reads its stated licence terms, and records one of
three verdicts. That is 128 cells.

**Regulatory-grade and open.** The source is the one actually cited in a real building code,
flood-insurance programme, or compliance standard in that country, *and* its licence permits
commercial use without restriction on redistribution. This is the strong verdict: a reader
with the licence terms in front of them can confirm both halves.

**A workable substitute.** Usable data exists, but it is coarser, global rather than national,
or otherwise not the exact input a local professional would cite. Global land-cover and
ecological classification products are the common case here — genuinely useful, genuinely
open, and genuinely not what a national regulator names [buchhorn-2020-copernicus-land-cover]
[dinerstein-2017-ecoregions]. A modelled global flood index is another
[wri-aqueduct-floods-2023] [baugh-2016-lisflood-fp]. The verdict says the cell is covered and
says what was traded away.

**Nothing usable.** No source exists under any open licence, or one exists and its licence
forbids the use.

Two words in those definitions carry most of the weight, and they are worth separating
because they are routinely conflated.

*Open* here means commercially usable and redistributable, not merely visible. A dataset
published on a government website that a member of the public may look at but may not
incorporate into a commercial product is not open in this sense, however freely it can be
viewed. That distinction is the reason one of the three structural gaps below exists at all.

*Regulatory-grade* means the source is the one with standing — the map the code names, not a
map of the same phenomenon. Two datasets can describe the same flood plain to similar accuracy
and have entirely different weight in a permit file.

Separately from the per-cell assessment, the layers have to be joined to actual locations, and
doing that sixteen separate ways would be unmaintainable. Every layer is joined against one
common spatial key: a worldwide hexagonal grid, at a resolution of roughly 1.2 square
kilometres a cell [brodsky-2018-h3]. A polygon map, a continuous raster surface and a single
value attached to a point all resolve to the same cells, so every country gets the same
integration pattern and differs only in which source feeds it. That is what makes a
sixteen-country comparison something that can be maintained rather than a set of sixteen
one-off projects.

## 5. What the scorecard found

**Most of what a site decision needs is genuinely open, in most of the countries studied.**
Of the eight categories, five reach regulatory-grade open status in at least six of the
sixteen countries. Two categories — seismic hazard and solar potential — reach at least a
workable regulatory or near-regulatory standard in every one of the sixteen, because both are
served by continent-wide open programmes rather than depending on each country publishing its
own layer: the United States federal hazard model domestically, and the European seismic
hazard model and the European Union's own solar-potential service across Europe.

**The United States has complete regulatory-grade coverage across all four of the
highest-priority categories** — climate zone, flood hazard, seismic hazard and solar potential
— each sourced from the exact federal agency or programme actually cited in code-compliance
and permitting practice, not a substitute standing in for it.

**Europe's result required a workaround rather than an acceptance of a downgrade, and that is
the more interesting half of the finding.** No single European-wide building-climate-zone map
exists, because each country defines its own national energy code independently under the
European framework. The obvious fallback would be a coarse global climate classification for
the whole continent, which would be a real loss of standing. Instead, each country's own
national energy-code climate zones are joined directly to that country's own municipal
boundary data. The result is genuinely regulatory-grade — the actual zone a national engineer
would use — for eight of the European countries in the study, and it does not require a
harmonised European standard to exist first. The remaining European countries either use a
single nationwide zone, which makes a zone map unnecessary, or require a data-registration
step not yet completed.

That pattern generalises, which is why we think it is worth publishing rather than merely
using. Any category where individual countries maintain their own regulatory standard, with no
continental equivalent, is a candidate for the same join rather than for a global proxy.

**Three gaps are structural, and each has a different cause.** They are not three instances of
one problem, and the distinction matters because the remedies are different.

*Canada has no national regulatory flood-hazard layer.* The programme intended to produce one
is still underway. The best available substitute today is a modelled prediction, not a
regulatory product — a distinction that should be stated to anyone relying on it rather than
smoothed over by the word "flood data." The cause here is simply that the thing does not exist
yet, and the remedy is to wait or to disclose.

*Mexico's most precise environmental and climate classification data carries a licence that
excludes commercial use.* The data exists and is good. It cannot be built on. A
lower-precision, commercially usable global substitute is used instead, and for Mexican sites
specifically that is a real downgrade in precision rather than an inconvenience. The cause is
legal, not technical, and no amount of engineering removes it.

*United States wind and snow design values are copyrighted by the standards body that
publishes them.* Unlike the other high-priority United States categories, these cannot be
redistributed as a map layer at all. The workable approach is a live, point-in-time lookup
against the standards body's own compliant service rather than a downloadable dataset — a
structurally different integration pattern from every other layer in the study, and a slower
and more externally dependent one. The cause is intellectual property, and the remedy is an
architectural accommodation rather than a fix.

**One category a reader might expect is not in the scorecard at all: zoning.** Nobody has
assembled an open, continental layer of municipal zoning, and we have not either. Zoning is
set municipality by municipality, in local instruments, in forms that differ in every
jurisdiction. It is therefore handled outside this scorecard entirely and verified parcel by
parcel before any land purchase: either the intended building is already a permitted use under
the existing designation, or diligence has established a credible, evidenced path to a
rezoning, tested against the municipality's own plan and its recent decisions on comparable
applications. Land is not acquired on the expectation that a rezoning will work out.

**What is delivered on the live platform is a subset of what the scorecard assesses.** The
scorecard is a statement about what is publicly available; the platform's own layer inventory
is a statement about what has been built and joined so far, and they are not the same thing.
At the reference date of the current coverage record, the delivered layers were: the United
States building-code climate zone, reaching 94.4 per cent of the qualifying United States
markets; the European regulatory energy climate zones, at a coverage that varies sharply by
country — near-complete in Germany and France, partial in Spain and the United Kingdom; a
global climate classification, at 100 per cent of all markets; and a global ecoregion layer,
at 99.5 per cent. The seismic and flood-hazard layers were in preparation, with the seismic
values sourced from the United States federal survey and the European hazard model and the
flood designations from the United States federal flood programme and the European Union's
own research service. Coverage figures of this kind go stale between processing runs; the live
platform, not a published snapshot, is the current statement of what is delivered.

**The limitation, stated rather than implied.** This assessment is documentary. For each cell
it reads the source's licence and its regulatory standing. It is not a completed run of the
integration pipeline against real site data in all sixteen countries producing an actual count
of how many real sites fall into each coverage category per country. The licence and standing
findings do not depend on that run; the per-country site counts do, and they are not available.
We say so directly rather than presenting a documentary catalogue as though it were a completed
empirical count.

## What this changes for the reader

The first change is a question you can now ask before relying on a site assessment: *for this
particular country and this particular risk, was the underlying data the actual regulatory
input, or a substitute?* That question has a specific answer in a specific cell, and the answer
does not depend on our characterisation of it — the cell names a source, and the source names
its own licence.

The second change is what you should expect for sites in the three affected countries. A
Canadian flood assessment today is a modelled prediction, not a regulatory determination, and
should be presented and read as one. A Mexican eco-region or precision-climate assessment is
using a lower-precision global stand-in for data that exists and cannot be licensed. And any
wind or snow load figure for a United States site has to come from a live compliant lookup
rather than a static map, because no freely redistributable static map of that data can legally
exist.

The third is more general, and it is the habit rather than the result. When any platform tells
you it has assessed something across many countries, the useful follow-up is not "how accurate
is it" but "which specific public record did you use, in which country, and on what licence."
A platform that can answer cell by cell is in a different position from one that can only
answer on average. We would rather be asked that question than not, which is why the scorecard
is published with its holes in it.

The trade-offs are real. A scorecard is more work to read than a score. It is a snapshot: a
licence change at any source would require the corresponding cell to be re-assessed rather
than assumed still valid. The depth of research behind each cell is not perfectly uniform — a
country with a single simple national standard has less to assess than one with four
independently complex regulatory systems, and a clean verdict in the first case is a different
kind of finding from a clean verdict in the second. And the European climate-zone join, being
derived rather than natively published, carries a permanent maintenance obligation: every time
a country updates its energy code, the join has to be updated before it reflects current
regulatory reality.

## An open invitation

Several of the questions this raises are better answered by people who work inside the
jurisdictions concerned.

To open-data and geographic-information specialists in the countries with the largest gaps —
Canada on flood, Mexico on precision environmental classification — the direct question is
whether a public source exists that this assessment has simply not found. That is an entirely
plausible outcome. A national or provincial programme, a research institution's published
dataset, a regional authority's open portal: any of these could close a cell we have marked
empty, and we would rather be corrected than right. Corrections are welcome and will change
the scorecard.

To the standards bodies and agencies whose licences create the gaps: the Mexican
non-commercial restriction and the United States wind and snow copyright are both deliberate
policy choices rather than oversights, and we are not suggesting either is illegitimate. The
question worth asking together is whether the intended effect of those choices requires
excluding the specific use in question — a site-assessment platform joining a value to a
location — or whether a narrower licence would achieve the same protection. We do not know the
answer and would not presume it.

To researchers working on European building-energy data: the national-energy-code join
described in Section Five is our own construction, not a published standard, and it is
therefore only as good as the lookup tables behind it. A spot-check of municipal centroids
against each country's own official climate-zone publication is the obvious validation and we
have not run it. Anyone holding one country's official zone map could falsify or confirm our
result for that country in an afternoon, and we would publish the outcome either way.

To people working on volunteered and open geographic data quality generally: the coverage
unevenness this paper reports for regulatory layers has a documented analogue in
volunteer-contributed map data [haklay-2010-osm-quality]. Whether the same
measurement approaches transfer from one to the other — per-country completeness estimation, in
particular — is a question we would like answered, because a scorecard that could attach a
confidence to each cell rather than a three-level verdict would be a materially better
instrument.

And to anyone maintaining a comparable catalogue: we would like to know of one. Part of the
reason this exists is that we could not find it, and a duplicated effort is a worse outcome
than a shared one.

## Conclusion

The honest position on regulatory site data is that it is mostly open, unevenly open, and that
where it is not open the reasons differ enough to matter. Five of the eight categories reach
regulatory-grade open status in at least six of the sixteen countries studied; two reach a
workable standard in all sixteen; the United States is complete across its four highest
priorities, and eight European countries reach regulatory-grade climate-zone coverage by
joining each country's own standard to its own boundaries rather than waiting for a continental
map that does not exist. Three gaps remain, caused respectively by a programme not yet
finished, a licence that forbids commercial use, and a copyright that forbids redistribution.
And this is a catalogue of what is publicly available, not a count of how many real sites it
reaches — a distinction we would rather draw ourselves than have drawn for us. Publishing the
real, uneven picture is more useful to a reader than a single number implying a rigour that is
not uniform, and it is the only version of this document that can be checked.

## References

Alphen, J. van, and Lodder, Q. 2006. Flood management and spatial planning in Europe.
*Proceedings of the ICE — Water Management* 159(1): 7–13.

Baugh, C. A., Bates, P. D., Schumann, G., and Trigg, M. A. 2016. LISFLOOD-FP hydrodynamic model
for a global river flood model. *Geoscientific Model Development* 9(11): 4347–4365.

Brodsky, I. 2018. *H3: Uber's hexagonal hierarchical spatial index.* Uber Engineering.
[https://www.uber.com/en-US/blog/h3/](https://www.uber.com/en-US/blog/h3/)

Buchhorn, M., Lesiv, M., Tsendbazar, N.-E., Herold, M., Bertels, L., and Smets, B. 2020.
Copernicus global land cover layers — collection 2. *Remote Sensing* 12(6): 1044.

Dinerstein, E., et al. 2017. An ecoregion-based approach to protecting half the terrestrial
realm. *BioScience* 67(6): 534–545.

European Union. 2007. *Directive 2007/60/EC on the assessment and management of flood risks.*
[https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32007L0060](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32007L0060)

European Union. 2010. *Directive 2010/31/EU on the energy performance of buildings; recast
2024/1275/EU.*
[https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32010L0031](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32010L0031)

Haklay, M. 2010. How good is volunteered geographical information? *Environment and Planning B:
Planning and Design* 37(4): 682–703.

National Research Council Canada. 2020. *National Building Code of Canada 2020.*
[https://nrc.canada.ca/en/certifications-evaluations-standards/codes-canada/codes-canada-publications/national-building-code-canada-2020](https://nrc.canada.ca/en/certifications-evaluations-standards/codes-canada/codes-canada-publications/national-building-code-canada-2020)

OpenStreetMap contributors. *Open Database Licence (ODbL) 1.0.*
[https://opendatacommons.org/licenses/odbl/](https://opendatacommons.org/licenses/odbl/)

Taylor, Z. T., Huang, D., Lucas, R., Chaney, A., and Gowri, M. 2008. *Using building energy
simulation and optimization to design climate zones (PNNL-17241).* Pacific Northwest National
Laboratory.
[https://www.pnnl.gov/main/publications/external/technical_reports/PNNL-17241.pdf](https://www.pnnl.gov/main/publications/external/technical_reports/PNNL-17241.pdf)

American Society of Heating, Refrigerating and Air-Conditioning Engineers. *ASHRAE Standard
90.1 — Energy Standard for Buildings Except Low-Rise Residential Buildings.*
[https://www.ashrae.org/technical-resources/bookstore/standard-90-1](https://www.ashrae.org/technical-resources/bookstore/standard-90-1)

World Resources Institute. 2023. *Aqueduct Floods 3.0: comparing future flood risk across
scenarios.* [https://www.wri.org/aqueduct](https://www.wri.org/aqueduct)

## Contributors

Prepared by Woodfine Management Corp.

## How this paper was produced

This paper is grounded in the preparing staff's own development and operating work, and in their standing engagement with the designers, software engineers, architects, engineers, and legal and accounting advisers the business works with. It was drafted and edited with AI assistance under editorial direction, and the analysis and conclusions are the author's own.

## Disclosures

Woodfine Capital Projects Inc. ("Woodfine") is the author of record and owns the framework and
the resulting dataset described in this paper; Woodfine Management Corp. maintains the data and
runs the analysis. Woodfine develops commercial property and relies on the coverage described
here in evaluating its own sites, so this paper argues for an approach in which we have a
direct commercial interest. This work was funded internally; no external research funding was
received. Nothing in this paper constitutes an offer to sell, or a solicitation of an offer to
buy, any interest in a Woodfine direct-hold solution; any offering is made only by the
applicable Private Placement Memorandum, which prospective investors should review with their
own professional advisors. This paper describes building-code, flood, seismic and zoning
concepts in general terms in order to explain a data-coverage assessment; it is not advice on
any particular site's regulatory position and is not a substitute for the professional advice
a real project requires. Some statements above describe planned or intended future work;
language such as "planned," "intended," "targeted," "may," and "expected" marks this
forward-looking content, which is subject to change and does not constitute a commitment
regarding future performance.

## Data and reproducibility

Every data source assessed in this paper is public and independently obtainable from the agency
or programme that publishes it, and the verdict in each cell rests on that publisher's own
stated licence terms, which a reader can go and read. The three-level grading scale and the
common hexagonal grid used to join layers to locations are described in full in Section Four,
so the assessment is reproducible by anyone with access to the same public sources. Two things
should be read as dated rather than permanent. Licence terms change: an "open" verdict reflects
a publisher's terms as they stood when the cell was assessed, and a change at source requires
that cell to be re-read rather than assumed still valid. And the platform's own delivered-layer
coverage figures quoted in Section Five describe one dated reference build; the live platform is
the current statement of what is delivered. The store and civic location data the layers are
joined to is drawn from OpenStreetMap under the Open Database Licence, which permits commercial
use and requires derived databases to be shared on the same terms. The per-country counts of how
many real sites fall into each coverage category are not yet available, because the pipeline run
that would produce them has not been completed — this is a catalogue of public availability, not
a count of sites. No independent party has audited this assessment, re-read these licences, or
reviewed these claims.

MCorp™ and Woodfine Capital Projects™ are trademarks of Woodfine Capital Projects Inc.
