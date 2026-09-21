---
schema: journal-v2
slug: site-context-overlays
title: "Site Context Overlays"
subtitle: "Holding each jurisdiction's local rules as swappable data laid over one unchanged design"
site: bim.woodfinegroup.com
imprint: WCP-010
thesis: "Local compliance should be a separate layer of data laid over a jurisdiction-agnostic design, never authored back into it, so a new market is a data question rather than a redesign."
abstract: |
  Our thesis is that compliance with a particular jurisdiction's rules should be computed
  as a separate, swappable layer of data laid over a design that is itself
  jurisdiction-agnostic — and never written back into the design. Opening in a new market
  should mean adding a record, not redrawing a building. The mechanism is a per-jurisdiction
  overlay held beside the design rather than inside it: the numeric and property
  requirements expressed in a published machine-readable constraint format, the
  requirements that have a spatial shape expressed as geometry, and both anchored to
  element identities that mean the same thing in every market. The design's core geometry
  and its leasing plans do not change when a jurisdiction is added; the overlay changes.
  This is the systems half of a two-part argument — a companion paper covers what the
  shared safety baseline actually contains. Almost none of this is running: the first
  overlay set is planned as a single illustrative jurisdiction, and the step that would
  put constraints in front of a designer while they work is intended, not built.
state: draft
version: "0.1.0"
published:
updated: "2026-09-20"
cite_as:
license: CC-BY-4.0
cites:
  - ids-1-0
  - bsdd-v1
  - ifc-4-3
  - iso-19650
  - bca-singapore-corenet
draws_from:
  - common-building-code
  - key-plans-and-tiles
  - fixed-floor-plates
  - development-regions
  - geographic-co-location-methodology
  - city-code-as-composable-geometry
  - asset-anchored-bim-vault
  - bim-design-philosophy
  - open-bim-regulatory-acceptance
prepared_by: "Woodfine Management Corp."
keywords:
  - regulatory compliance
  - multi-jurisdiction development
  - building information
  - open standards
  - expansion cost
---

> Nothing in this paper constitutes an offer to sell, or a solicitation of an offer to buy,
> any interest in a Woodfine direct-hold solution; any offering is made only by the
> applicable Private Placement Memorandum. Statements marked "planned," "intended,"
> "targeted," "may," or "expected" are forward-looking and subject to change. Full
> disclosures appear at the end of this paper.

Working Paper WCP-010 · v0.1.0 · CC BY 4.0

A design office entering a new country faces one question before any other: does opening
here mean redrawing the building, or does it mean adding a record to a table? Our thesis is
that it should be the second, and that whether a developer can actually answer it that way
is decided years earlier, by how the compliance information was arranged in the first place.

Our position is that a jurisdiction's local rules should be held as a separate, swappable
layer of data laid over a design that is itself jurisdiction-agnostic — and never authored
back into the design. The design carries no country in it. Beside it sits a per-jurisdiction
overlay: the numeric and property requirements written in a published, machine-readable
format; the requirements that have a spatial shape written as geometry; and both anchored to
element identities that mean the same thing everywhere. Registering a new jurisdiction adds
an overlay. It does not touch the building.

This is the systems half of a two-part argument, and the halves should not be confused. A
companion paper on this site argues the content question — what the shared safety baseline
actually is, and why building once above the strictest safety requirement anywhere absorbs
nearly all of what a code contains. This paper takes that baseline as given and asks the
mechanical question that follows: given a narrow local remainder, how is it actually tracked
and computed without anyone touching the design files? Almost none of the answer is running
yet, and the section on what is actually built says so plainly.

## 1. The thesis

Keeping the design jurisdiction-agnostic, and holding every local rule as data in a
separate per-jurisdiction overlay, means registering a new market is a matter of adding one
record rather than editing a design.

The distinction that carries the whole argument is between information that is *in* a thing
and information that is *about* a thing. A dimension written onto a drawing is in the design:
change it and you have changed the building. A rule stating that this jurisdiction requires a
particular clearance is about the design: it can be checked against the design, and it can be
swapped for a different jurisdiction's rule, without the design moving.

Almost every developer working across borders ends up with the first arrangement, not because
anyone chose it but because nobody prevented it. A local requirement is discovered during
permitting, the drawing is amended to satisfy it, and from that moment the requirement has
become part of that building's design. It is no longer legible as a local rule. Three markets
later, nobody can say which features of which drawing set exist because the building needs
them and which exist because one authority once asked. The design has absorbed its own
compliance history, and the ability to say "this building, in that market" has been lost.

Our position is that this absorption is the actual failure, and that everything expensive
about multi-market expansion follows from it. Keep the two separate and the expansion cost
behaves differently.

## 2. The problem, in the reader's terms

Consider a company operating in a dozen tax jurisdictions.

Nobody runs twelve accounting systems. A competently run company runs one — one chart of
accounts, one ledger, one set of controls — and holds the jurisdictional differences as
data within it: a tax table listing the rates, thresholds, filing dates, and treatments that
apply in each place. When a rate changes, somebody edits a row. When the company enters a
thirteenth country, somebody adds a row, and the ledger itself is untouched.

Two properties make this work, and both are worth naming because they transfer directly.
First, the table is *legible*: anyone can read it and see exactly what is different about
Poland, in one place, without inferring it from the behaviour of the system. Second, it is
*swappable*: the accounting system does not care which row is in force, so a new one can be
added without regression testing the whole ledger.

Now picture the same company running the other arrangement — twelve separate accounting
systems, each incorporating its own jurisdiction's rules into the way it posts entries. Each
one is correct. None of them is comparable to the others. A change in group policy has to be
applied twelve times. And no one can produce, on request, a statement of what is actually
different about Poland, because the difference is distributed through the software rather
than written down.

That second arrangement is how building compliance is ordinarily handled, and it is what we
are trying not to do.

## 3. How compliance is normally checked

The standard architecture for checking a building against a code has been stable for twenty
years and is worth describing accurately, because our proposal is a departure from it and the
departure should be judged against a fair account of it.

A designer draws the building in whatever authoring software they use. When the design is
substantially complete it is exported and submitted to a rule-checking service. The service
applies a ruleset — sometimes a proprietary rule language, sometimes a published constraint
file, sometimes a script — and produces a report listing violations. A person reads the
report, returns to the authoring software, corrects the design, and resubmits. The cycle
repeats until the report is clean.

This works, and it is genuinely valuable. It also has a structural property that no amount of
improvement removes: the check happens after the design is made. The rule-checker sits
outside the design environment and communicates with it after the fact, which means the cost
of a violation is proportional to how long it went unnoticed. The more thorough the checking,
the longer each cycle. Design teams budget weeks for this on complex projects, and the weeks
are not a tooling defect anyone has failed to fix. They are inherent to checking afterward
rather than constraining beforehand.

Public authorities have pushed this arrangement about as far as it goes. Singapore's national
building-submission system accepts models for permit application and runs automated
code-compliance checking against national requirements, which is, as far as we have been able
to establish, the most advanced version of this in public production anywhere
[bca-singapore-corenet]. It remains a checker: models are authored freely, submitted, and
returned with findings.

The arrangement we want sits differently. If the requirement travels *with the element* — so
that placing a non-compliant configuration is not a thing the design environment lets a
designer do easily — then the cost of a violation is not weeks of rework. The violation does
not enter the model. We are careful to say this is an architecture we are building toward
rather than one we have; the last section is explicit about how far along it is.

## 4. How the overlay actually works

Three pieces, held beside the design rather than inside it. What follows is the intended
arrangement, described in the present tense because that is how an architecture is most
clearly explained; the section after it says how much of it exists today, which is not much.

**A stable name for every kind of element.** Before anything else can work, a wall has to mean
the same thing in Poland as in Mexico. There is a published international dictionary for
exactly this — a shared reference in which each type of building element has a permanent
identifier and an agreed definition, independent of any software or any country
[bsdd-v1]. Every element in the design carries its identifier from that dictionary. That
identifier is what a jurisdiction's overlay refers to. It is the equivalent of the account
code in the accounting analogy: the thing both the ledger and the tax table can point at
without ambiguity.

**The numeric and property requirements, in a published constraint format.** Most of a local
requirement is expressible as a number or a property: a minimum rating, a maximum
heat-transfer value, a required clearance, a mandatory characteristic. There is a published
open standard for writing exactly this kind of requirement in a form software can act on — a
specification format in which one states what a valid model must contain, element type by
element type [ids-1-0]. A jurisdiction's overlay includes one of these files. It is a
document a person can read and a machine can apply, which is the property the accounting
analogy's tax table has and a rule buried in a drawing does not.

**The requirements that have a shape, as geometry.** Some requirements cannot be written as a
number. "This separating wall must be continuous from floor slab to ceiling slab with no
unprotected penetrations" is a statement about space and adjacency, not about a value. For
those, the overlay carries geometry: a solid shape, in an open, internationally standardised
building-data format, defining the volume that must be kept clear or must be filled by
conforming construction [ifc-4-3]. It attaches to the element and resolves where the element
is placed.
A designer sees the required spatial condition while designing rather than after submitting.

All three sit in a per-jurisdiction folder alongside the building's record — one folder per
market, each holding that market's dictionary references, its constraint file, and its
geometry fragments. The folder is the row in the tax table. Adding a market adds a folder.

Two consequences follow, and they are the point of the arrangement.

**The design does not change.** The building's core geometry and its leasing plans are
untouched when a jurisdiction is added. This is not a convention we are undertaking to
observe; it is a consequence of the rules living somewhere the design files do not reach. The
overlay changes, the plan does not.

**The differences become legible.** Because each market's requirements sit in one readable
place, it is possible to answer "what is actually different about Italy?" by reading a file,
rather than by comparing two drawing sets. It also lets the variants be organised sensibly. We expect the
clusters of genuinely divergent requirements not to follow national borders neatly, so where
a physical variant of the building is warranted, it is intended to be organised around where
the codes actually fail to overlap rather than around which country a site sits in.

The programme these overlays serve is nine planned development jurisdictions — Canada, the
United States, Mexico, Spain, the United Kingdom, Italy, Poland, the Nordics, and New Europe.
That is a count of places we plan to build, and a reader working through the wider set of
these papers will meet a different, smaller count elsewhere referring to something else
entirely: the jurisdictions in which investment vehicles are established. The two numbers
count different things and should not be reconciled.

## 5. What is actually built

Very little, and this section exists so the previous one is not read as a description of a
running system.

The element dictionary and the constraint-file standard are real, published, and maintained
by an international standards body; they are not ours and they are not speculative. The
building-data format the geometry fragments use is an international standard as well. What we
are proposing is a particular way of assembling those published pieces, and the assembly is
at an early stage.

The first overlay set is planned as a single illustrative jurisdiction — one zoning code and
one climate zone's performance parameters — chosen to prove the shape rather than to cover a
market. It is a demonstration, not a compliance product, and nothing should be read into the
choice of jurisdiction. Generating conformant constraint files automatically from the overlay
data, so that existing rule-checkers can consume them, is intended and not built. And the
step that would deliver the actual benefit argued for above — constraints reaching a designer's
authoring software at the moment an element is placed, rather than at submission — is intended
and further off than the other two.

Until that last step exists, the honest description of what this arrangement buys is narrower
than the architecture suggests. Today it buys legibility and separation: the local rules are
written down, in one place, in a machine-readable form, and they are not in the drawings.
That is worth having on its own and it is not the same as compliance-by-construction. We
would rather a reader hold us to the narrower claim.

It is also worth stating what does not change under any version of this. A local architect
still redraws the approved design for the local permit, stamps it, and takes it through the
authority's process. That is required professional work in every jurisdiction. Nothing here
removes it, and nothing here should be read as proposing to.

## What this changes for the reader

The change is in what an investor should expect the second, fifth, and ninth market to cost
relative to the first.

If compliance is authored into the design, every market carries a design cost, and the ninth
resembles the first. If compliance is a separate data layer, the design is paid for once and
each further market carries a registration cost and a permit cost — real, but of a different
order. The difference compounds across a programme, and it is invisible from outside unless
somebody asks the right question.

The right question is not "do you operate in multiple jurisdictions," which everyone answers
yes to. It is: can you show me, as a document, what is different about this market — and did
the building change when you entered it? A developer with a genuine overlay can hand over the
document. A developer whose compliance is in the drawings will describe a process, because
there is nothing to hand over.

The trade-offs belong in the same paragraph. The arrangement assumes local requirements are
mostly *additive* — that a jurisdiction asks for more rather than for something structurally
incompatible. Where that assumption fails, the overlay cannot express the difference and a
variant of the building is needed, which is exactly the redesign the arrangement exists to
avoid. Maintaining overlays is ongoing work that does not appear in a construction budget:
codes change, and a stale overlay is worse than none because it looks authoritative. And the
benefit argued for here is largest at the step that is furthest from being built.

## An open invitation

The open questions here belong to people who build software for the built environment and to
people who administer building regulation, and both would tell us things we cannot work out
from the inside.

To software and data-architecture specialists working in construction technology: the
load-bearing assumption is that local requirements are additive deltas over a shared
baseline. We do not know whether this overlay pattern generalises cleanly to jurisdictions
with genuinely incompatible base requirements — not stricter, but differently shaped — and we
have not tested it against one. If there is a known market where the assumption breaks, that
is the single most useful thing anyone could tell us.

To the maintainers and practitioners of the open constraint and dictionary standards we are
building on: we are using published standards in a way their guidance does not obviously
anticipate — as the storage format for a developer's own per-market rule set, rather than as
a checking specification for a single project. We would like to know whether that use is
sound, whether it strains the standards in ways a practitioner would immediately see, and
whether anyone has already done it.

To regulators and code officials publishing requirements: the arrangement described here
works far better if a jurisdiction's requirements are published in a machine-readable form by
the jurisdiction itself, rather than transcribed into one by a developer. Transcription is a
liability — ours, and eventually the authority's, when somebody relies on a transcription that
has drifted. We would rather consume an authoritative published form than maintain our own,
and we would participate in work aimed at producing one.

And to anyone maintaining a regulatory data set across many jurisdictions in any industry:
the maintenance problem — how often overlays are reviewed, on what trigger, by whom, and how
staleness is detected before somebody relies on it — is not specific to buildings, and other
fields have solved it better than a developer entering its first markets will.

## Conclusion

One design, many jurisdictions, each expressed as data rather than as a redraw. That is the
separation this paper argues for: the building carries no country in it, and everything a
particular country requires sits beside it, readable by a person and actionable by software,
swappable without the design moving. The benefit is not primarily speed, although speed
follows. It is that the difference between one market and another stays legible instead of
dissolving into a drawing set. Today that separation buys us a written, machine-readable
record of local requirements and the discipline of keeping them out of the design. The
stronger version — where a non-compliant configuration is simply not something a designer can
place — is the direction, and it is not yet built.

## References

buildingSMART International. *buildingSMART Data Dictionary (bSDD) — classification and
property definitions.*
[https://www.buildingsmart.org/users/services/buildingsmart-data-dictionary/](https://www.buildingsmart.org/users/services/buildingsmart-data-dictionary/)

buildingSMART International. *Information Delivery Specification (IDS) 1.0.*
[https://www.buildingsmart.org/standards/bsi-standards/information-delivery-specification/](https://www.buildingsmart.org/standards/bsi-standards/information-delivery-specification/)

buildingSMART International. *Industry Foundation Classes (IFC) 4.3 — ISO 16739-1:2024.*
[https://ifc43-docs.buildingsmart.org/](https://ifc43-docs.buildingsmart.org/)

Building and Construction Authority, Singapore. *CORENET — regulatory submission for the
built environment.* [https://www.bca.gov.sg/](https://www.bca.gov.sg/)

International Organization for Standardization. *ISO 19650 — Organization and digitization of
information about buildings and civil engineering works, including building information
modelling (BIM).*
[https://www.iso.org/standard/68078.html](https://www.iso.org/standard/68078.html)

## Contributors

Prepared by Woodfine Management Corp.

## How this paper was produced

AI assistance was used in preparing and revising this paper.

## Disclosures

Woodfine Capital Projects Inc. ("Woodfine") is the author of record and is the developer and
promoter of the buildings and the delivery method described in this paper; Woodfine
Management Corp. employs the staff and retains the consultants who prepare this material and
perform the work it describes. Woodfine has a direct commercial interest in the approach
argued for here. This work was funded internally; no external research funding was received.
Nothing in this paper constitutes an offer to sell, or a solicitation of an offer to buy, any
interest in a Woodfine direct-hold solution; any offering is made only by the applicable
Private Placement Memorandum, which prospective investors should review with their own
professional advisors. Nothing here is a legal opinion on the building code or permitting
requirements of any jurisdiction, and nothing here should be relied on in place of advice
from a qualified local architect, engineer, or code consultant. Some statements above
describe planned or intended future work; language such as "planned," "intended,"
"targeted," "may," and "expected" marks this forward-looking content, which is subject to
change and does not constitute a commitment regarding future performance. Reference to nine
planned development jurisdictions describes intended programme scope and is not a statement
that any site has been acquired, optioned, or permitted in any of them.

## Data and reproducibility

The three open standards this arrangement is assembled from — the element dictionary, the
constraint-specification format, and the building-data format the geometry fragments use —
are published by an international standards body and are freely readable by anyone. A reader
who wants to check whether we have characterised them accurately can, and we would encourage
it, since the accuracy of that characterisation is what most of this paper rests on. The
international records-management standard referenced is sold rather than given away, which is
ordinary practice.

What does not exist yet, and therefore cannot be inspected, is our own overlay data. There is
no published per-jurisdiction rule set to examine, because the first one is planned as a
single illustrative jurisdiction and is not yet complete. There are no figures here on how
long registering a jurisdiction takes, what an overlay costs to maintain, or how much of a
market's requirements a given overlay actually captures, because no such measurement has been
made and we would rather say so than estimate. The sequence described — design, then shared
baseline, then local overlay applied at permit stage by a local architect — is the delivery
method being built, not an observed process with completed buildings behind it. No independent
party has reviewed this arrangement, tested it against any jurisdiction's requirements, or
confirmed the claims made for it.

Woodfine Capital Projects™ is a trademark of Woodfine Capital Projects Inc.
