---
schema: journal-v2
slug: independent-record-per-building
title: "Why Each Building Keeps Its Own Independent Record"
subtitle: "One independently hosted, open-source record server per building, organized toward a published records-management standard"
site: bim.woodfinegroup.com
imprint: WCP-007
thesis: "A building's design record should live on its own independently hosted server running open software, not inside one vendor's shared system serving a whole portfolio."
abstract: |
  Our thesis is that a building's design record should be held the way the building
  itself is held — one record, one building, under the owner's control — rather than as
  one portfolio-wide database reachable only through a single vendor's hosted portal.
  The design intent is a separate record server for each building, running open-source
  software, which the architects, engineers, and specialist consultants working on that
  building connect their own tools to. The record is to be organized and governed
  against ISO 19650, the published international standard for managing building
  information. That standard governs how a record is structured, named, versioned, and
  handed over — it is a records-management discipline, not a file format, and we are
  careful not to claim more for it than that. Two limits are worth stating plainly. No
  Woodfine Building has been built yet, so no building's record is in service today.
  And a record server that any consultant's software can connect to without integration
  work is an aim, not a solved problem.
state: draft
version: "0.1.0"
published:
updated: "2026-09-20"
cite_as:
license: CC-BY-4.0
cites:
  - iso-19650
  - bsi-iso-19650-certification
  - buildingsmart-openbim
draws_from:
  - bim-design-philosophy
  - property-manager-bim-gap
  - open-bim-regulatory-acceptance
  - customer-hostability
  - fixed-floor-plates
  - key-plans-and-tiles
  - bim-market-context
prepared_by: "Woodfine Management Corp."
keywords:
  - building records
  - ISO 19650
  - open standards
  - vendor independence
  - property ownership
---

# Why Each Building Keeps Its Own Independent Record

*One independently hosted, open-source record server per building, organized toward a published records-management standard*

> Nothing in this paper constitutes an offer to sell, or a solicitation of an offer to buy,
> any interest in a Woodfine direct-hold solution; any offering is made only by the
> applicable Private Placement Memorandum. Statements marked "planned," "intended,"
> "targeted," "may," or "expected" are forward-looking and subject to change. Full
> disclosures appear at the end of this paper.

Working Paper WCP-007 · v0.1.0 · CC BY 4.0

Our thesis is that a building's design record should be held the way the building itself is
held: one record, one building, on a server the owner controls. The usual arrangement is
the opposite. A developer's whole portfolio sits inside one software platform, hosted on
the software company's own computers, reachable only through that company's own website,
on an annual subscription. The drawings, the structural calculations, the mechanical
layouts, the specifications, the permit set, the as-built corrections — all of it lives
in one place that belongs to somebody else, and the owner's access to it lasts exactly as
long as the commercial relationship does.

We intend to build the other arrangement. Each Woodfine Building is to have its own
record server — its own small, separate computer, running open-source software, holding
that one building's design record and nothing else. The architects, engineers, and
specialist consultants working on that building connect their own tools to that building's
own server. The record is to be organized and governed against ISO 19650, the published
international standard for managing information about buildings, which sets out how a
record should be structured, named, versioned, approved, and handed over. That standard is
a discipline for running a record, not a file format, and this paper is careful throughout
not to claim more for it than it delivers.

Two things are worth saying at the outset, because they bear on how much of this is
already true. No Woodfine Building has been built. The record arrangement described here
is a commitment being built into the delivery method, not a system with buildings in it.
And the harder half of the ambition — a record server that any consultant's software can
connect to without integration work of its own — is an aim we hold and have not solved.
This paper sets out why we think the arrangement is worth the effort, and where a
specialist could tell us we have it wrong.

## 1. The thesis

Hosting a building's design record independently, on open software, one building at a
time, means the record's availability never depends on one portfolio-wide commercial
relationship continuing.

That is a narrower claim than it may first appear, and the narrowness is deliberate. We
are not claiming that a record held this way is better drawn, more complete, or more
accurate than one held in a hosted platform. We are claiming something structural about
who has to keep existing for the record to remain reachable. In the ordinary arrangement,
the answer is: the software company, the subscription, and the portfolio-wide account. In
the arrangement we intend, the answer is: the owner of that one building.

The reason to care is that the two things have very different lifespans. A commercial
office building is designed, financed, and underwritten on the assumption that it will
stand for fifty years or more. Software companies, software products, and the file formats
they write in do not last fifty years, and are not expected to. Neither do commercial
relationships. A building's record is asked to outlive, by decades, every arrangement that
was in place when it was created. Almost nothing about how the industry ordinarily stores
that record is designed for that.

## 2. The problem, in the reader's terms

Think about how a building's drawings used to be kept, and in many places still are.

The architecture firm that designed the building holds the drawing set. It sits in a flat
file cabinet in their office — the wide, shallow drawers that large-format drawings are
stored flat in. If the owner needs a copy, they telephone the firm, and the firm sends
one. This works. It has worked for a century. It works for exactly as long as three
conditions hold: the firm is still in business, the firm still has the drawings, and the
firm still returns the owner's calls.

Every one of those conditions fails eventually. Firms merge, retire, and close. Archives
get thinned when a lease on office space gets expensive. A relationship that was warm
under one managing partner is cool under the next. And when the conditions fail, what the
owner has lost is not a convenience. A building without its drawings is a building that
cannot be efficiently renovated, cannot be sold without a discount for the uncertainty,
and cannot answer a regulator's or an insurer's question about what is actually inside its
walls without somebody opening them.

The modern version of this arrangement is not an improvement on it. It is the same
arrangement with a larger cabinet and a monthly invoice. The design record for a whole
portfolio lives inside one software platform, on that company's computers, behind that
company's login. The building's owner can see the record whenever they like, which feels
like an advance on telephoning an architect. But the underlying dependency has not moved;
it has been consolidated. Where the old arrangement risked one firm's cabinet, the new one
puts every building in the portfolio behind a single commercial relationship, and a single
company's continued willingness and ability to host them.

There is a second, quieter failure that the industry documents on itself. The detailed
digital model of a building is commissioned by the developer, produced by the architects
and engineers, used through construction, and handed to the property manager at
completion. A large share of the people who receive it never use it. They do not have the
software licence, they have not been trained on the software, and the file they were
handed does not open in anything they do have. The model was paid for, delivered, and
contractually complete, and it sits unopened. That is not a failure of the people at the
receiving end. It is a failure of an arrangement in which the record is only reachable
through one expensive, specialised door.

## 3. What a building's design record actually is

It is worth being concrete about the contents, because "the building's record" is a phrase
that can sound either trivial or grand depending on what the reader imagines is in it.

A commercial building's design record is, at minimum: the architectural drawings that show
what is where; the structural drawings and calculations that show what holds it up; the
mechanical, electrical, and plumbing drawings that show how air, power, water, and waste
move through it; the specifications, which are the written document saying exactly which
products, grades, and standards every element must meet; the permit set that the local
authority approved; and the as-built corrections, which record the many places where what
was constructed differs from what was drawn. Add to that, over the building's life, the
equipment registers, the maintenance and inspection history, the lease plans showing who
occupies what, and the record of every alteration a tenant has made.

Since roughly the turn of the century, the industry has increasingly held this material
not as a set of separate drawings but as a single three-dimensional model in which every
wall, duct, beam, and door is an object carrying its own attached information — its
dimensions, its material, its fire rating, its manufacturer, its warranty. The practice is
called building information modelling, usually shortened to BIM. The word "model" is a
little misleading to a newcomer: the useful part is not the three-dimensional picture, it
is the structured information attached to every piece of it. A well-built model can answer
"how many fire dampers are in this building, where are they, and when was each last
inspected?" in a way that a stack of drawings cannot.

This is genuinely better than drawings, and it is why public buyers now insist on it. The
United States federal government, the European Union, the United Kingdom, and a growing
list of other jurisdictions require it for public procurement, and require it in open,
vendor-neutral form rather than in any one company's proprietary format. But being better
than drawings does not make it safe. A richer record held in a more consolidated place is
a larger thing to lose.

## 4. What "independent" means here

The design intent is a separate record server for each building: its own small computer —
in practice a lightweight virtual machine, which is a self-contained computer that exists
as software on shared hardware and can be copied, moved, or archived whole — holding that
one building's information and nothing else. Alongside the building's own model sits a
materials database, recording what the building is actually made of, which matters both
for maintenance and for the eventual recovery of materials when something is refitted or
taken down. The same machine is intended to receive the readings from the building's own
sensors as it operates, so that the record of what the building is and the record of how
it is behaving are not two systems that have to be reconciled by hand.

Three properties follow from that arrangement, and they are the whole of the claim.

**The software is open-source.** That phrase carries a specific meaning worth stating
plainly for a reader who has only met it in passing. Open-source software is published
with its underlying instructions readable by anyone, under a licence that permits anyone
to run it, examine it, change it, and pass it on. The practical consequence is not that it
is free of charge — that is often true and is not the point. It is that no single company
can withdraw it. If the people who wrote it stop maintaining it, the published instructions
remain, and anyone competent can keep it running. An owner's ability to open their own
building's record does not sit behind anyone's business decision.

**The hosting is per building.** One building, one record, one server. This is the part
that most distinguishes the arrangement from the ordinary one, and it is worth being
blunt about what it costs: running many small record servers is more work than running one
large one, and it forgoes real conveniences that a single portfolio-wide system provides.
We accept that cost deliberately. A building is bought, financed, insured, and sold one at
a time. A record that can only be separated from its portfolio by a migration project is
a record that is not really attached to the building at all.

**The consultants connect their own tools.** The people who actually author and revise a
building's record are not its owner. They are the control architect who holds the overall
design, the local architect who prepares the permit drawings for that jurisdiction, and
the structural, mechanical, landscape, and parking specialists working alongside them.
Each has their own software, chosen for their own reasons, and none of them will change it
for one client. The intent is that each of them reaches that building's own server with
the tools they already use, rather than every party being obliged onto one platform
because the record happens to live there.

This third property is where we are least far along, and the honest statement is short.
An open record server that any consultant's software can connect to without integration
work of its own is an aim, not an achievement — and it is one we expect to be harder in
practice than it sounds in a sentence. Today the commitment we can actually stand behind
is narrower: the server is open-source and independently hosted per building, so a new
consultant's tools can be connected to it without depending on one company's hosted
platform continuing to exist. That is not the same as saying any tool will read it out of
the box, and we do not want the stronger claim to be read into the weaker one.

## 5. The standard the record is organized toward

A server is a place to put things. It says nothing about whether what is in it is
intelligible. A record can be perfectly available and still be useless, if nobody can tell
which of four files is the current one, or what "approved" meant when somebody wrote it in
2029.

ISO 19650 is the published international standard that addresses exactly that. It is worth
describing plainly, because its name suggests something more technical than it is. The
standard sets out how information about a building should be organized and managed across
the whole life of a project: how a container of information is named so that its
discipline, stage, and revision are readable from the name itself; what status it carries
as it moves from work in progress, to shared with the rest of the team, to formally
published; who is responsible for approving that movement; what the client must specify
they need before the work starts; and what, exactly, must be handed over at completion and
in what condition.

It is a records-management discipline. It is not a file format, and it does not make one
company's software read another's. Those are separate problems with separate standards
addressing them, and conflating the two is a common enough error that we want to be
explicit about not making it. What ISO 19650 gives an owner is the ability to say, of a
record they hold, that it was produced and handed over under a published international
discipline rather than under whatever conventions a particular project team happened to
adopt.

Our intention is to obtain formal certification against the standard through an
independent certification body. That is a target, not a held credential, and it will
remain a target until a body has actually assessed the work and issued it.

There is a real open question underneath this, which the section on invitations returns
to. ISO 19650's published guidance, and most of the practice built on it, assumes a
project team working in a shared, centrally hosted information environment — what the
standard calls a common data environment. Our arrangement deliberately is not that. It is
many small environments, one per building. Whether the standard's requirements are
satisfied cleanly by a per-building, independently hosted arrangement, or whether that
reading strains the standard in ways a practitioner would immediately see, is something we
would rather be told than assume.

## 6. What this protects against

The failure this design exists to prevent is specific, and stating it concretely is more
useful than a general appeal to independence.

A developer holds a portfolio of buildings whose records all live in one hosted platform.
The platform's owner is acquired, or discontinues the product, or changes its pricing in a
way that makes the subscription untenable, or has an outage, or fails. What happens next
is not that the records vanish — there is almost always an export path, and it is almost
always worse than the original. Export formats lose what the receiving format does not
understand. The attached information that made the model worth having — the ratings, the
warranties, the maintenance history, the tenant links — is the part most likely to be
dropped, because it is the part most specific to the platform that held it. The owner ends
up with geometry and loses the thing the geometry was carrying.

Per-building independence does not make that scenario impossible. It makes it survivable
one building at a time. If something goes wrong with one building's record server, it is
one building's problem. There is no arrangement in which every building in the portfolio
becomes unreachable together, because there is no single thing they all depend on.

The same property matters at the other end of a building's life with an owner. When a
building is sold, the intent is that its record goes with it — the whole machine, handed
over as a unit, the way a set of keys is handed over. The buyer does not need to be
onboarded to a platform, have permissions reconstructed, or negotiate a subscription for
access to the history of the thing they just bought. The record is part of what was
bought.

## What this changes for the owner

The change is that a question which is usually vague becomes a question with a checkable
answer.

An owner or a prospective buyer assessing a building's design record can today ask only
soft versions of the right question: is the documentation good, is it complete, is it
current. Those are hard to verify and easy to answer optimistically. The question this
arrangement makes available is harder to be vague about. Does this building's record
depend on one company's hosted system remaining available, or is it independently hosted
and under the owner's control? Can it be handed over whole at sale, or must it be exported?
Is the software that reads it published openly, or does opening it require a licence that
somebody must keep paying for?

Those are answerable on any building, including buildings that have nothing to do with us.
A reader who takes only one thing from this paper could reasonably take that: the
questions are worth asking of any commercial property whose documentation matters to its
value.

The trade-offs belong in the same breath. Running one record server per building is more
administrative work than running one system for a portfolio, and that work does not go
away. Some genuinely useful things are easier in a single consolidated system — comparing
across a portfolio, applying one change everywhere, reporting on everything at once. The
open-source commitment means that when something breaks, there is no vendor whose
obligation it is to fix it; the responsibility sits with the owner and whoever they engage.
And the part of this we consider most valuable to a working design team — that every
consultant can connect their own tools — is the part not yet delivered.

## An open invitation

Several of the questions raised here belong to people who practise in fields we are
building against rather than in.

To records-management and information-management specialists working under ISO 19650: the
standard and the guidance around it are written with a centrally hosted common data
environment in view. We are proposing many small ones, one per asset. We would genuinely
like to know whether the standard's information-container, status, and approval
requirements are satisfied cleanly by that shape, whether it creates obligations at
handover that a centralised environment discharges automatically, and whether there is
prior practice — in sectors with stricter separation requirements than ours — that has
already worked this through.

To architects and engineers who actually have to work across client platforms: the claim
we are least confident in is that a specialist consultant can be given access to a
per-building record server and simply work. We would rather hear, before we build it,
where that breaks — which parts of a normal workflow assume a shared platform, what
coordination between disciplines actually depends on, and what the realistic integration
cost is for a firm asked to connect to one more environment.

To facilities and property managers: the handover gap described earlier is your problem
before it is ours, and you have seen more handovers than we have. What would a building's
record have to look like, on the day you receive it, for you to actually use it in the
first year — not in principle, but given the software, budget, and time you really have?

And to anyone who has lived through a platform migration for a real portfolio: we are
arguing from a structural analysis and not from that experience. If there is a category of
loss that only shows up when a migration actually happens, we would rather learn it from
you than discover it ourselves.

## Conclusion

A building's design record should be held the way the building is held — one record, one
building, under the owner's control, on software nobody can withdraw. That is the position,
and it is deliberately a modest one. It does not claim that any tool will read any record,
that the arrangement is cheaper to administer, or that a published standard solves a
technical problem it was never written to solve. It claims that availability should be
measured building by building rather than promised portfolio-wide, and that an owner
should be able to check which of the two they have. A building outlives its software, its
consultants, and usually its owners. Its record should be arranged accordingly.

## References

International Organization for Standardization. *ISO 19650 — Organization and digitization
of information about buildings and civil engineering works, including building information
modelling (BIM): information management using building information modelling.*
[https://www.iso.org/standard/68078.html](https://www.iso.org/standard/68078.html)

BSI Group. *BIM — Building Information Modelling — ISO 19650 certification.*
[https://www.bsigroup.com/en-CA/bim---building-information-modelling---iso-19650/](https://www.bsigroup.com/en-CA/bim---building-information-modelling---iso-19650/)

buildingSMART International. *openBIM — open, neutral standards for the built asset
industry.* [https://www.buildingsmart.org/](https://www.buildingsmart.org/)

## Contributors

Prepared by Woodfine Management Corp.

## How this paper was produced

This paper is grounded in the operating and development work the preparing staff do themselves, and in what they have learned from the people they work with routinely: the graphic designers, web developers, and software developers and engineers who build the platform alongside them, and the architects and structural, building-services, and civil engineers they develop buildings with. No outside professional reviewed or approved this paper, and nothing in it is professional advice. It was drafted and edited with AI assistance under editorial direction, and the analysis and conclusions are Woodfine's own.

## Disclosures

Woodfine Capital Projects Inc. ("Woodfine") is the author of record and is the developer
and promoter of the buildings and the delivery method described in this paper; Woodfine
Management Corp. employs the staff and retains the consultants who prepare and maintain
this material. Woodfine has a direct commercial interest in the approach argued for here.
This work was funded internally; no external research funding was received. Nothing in
this paper constitutes an offer to sell, or a solicitation of an offer to buy, any
interest in a Woodfine direct-hold solution; any offering is made only by the applicable
Private Placement Memorandum, which prospective investors should review with their own
professional advisors. Some statements above describe planned or intended future work;
language such as "planned," "intended," "targeted," "may," and "expected" marks this
forward-looking content, which is subject to change and does not constitute a commitment
regarding future performance. No Woodfine Building has been constructed as at the date of
this paper, and nothing here should be read as a statement that any building, record
server, or certification described is in service.

## Data and reproducibility

There is no dataset behind this paper. What it describes is a design commitment and the
reasoning for it, and every element of that commitment is checkable in one of two ways.
The international standard the record is to be organized against is published and can be
purchased and read by anyone; the certification body that assesses conformance to it
publishes its own scheme openly. The property we claim for open-source software — that
anyone may run, read, alter, and redistribute it, and that no single company can withdraw
it — is a property of the licence such software is published under, not a promise we make
about our own conduct, and a reader can verify it for any particular piece of software by
reading that licence. The figures a reader might expect and will not find here — how many
buildings, how large a record, how much it costs to run — do not exist yet, because no
building has been built. We would rather say so than estimate them. No independent party
has reviewed this arrangement, assessed it against the standard named, or confirmed the
claims made for it.

Woodfine Capital Projects™ is a trademark of Woodfine Capital Projects Inc.
