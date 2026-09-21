---
schema: journal-v2
slug: key-plans-and-tiles
title: "Key Plans and Tiles, a Self-Similar, Aperiodic Space-Planning System"
subtitle: "Planning a floor from the furniture out, so that whatever is left over is always still worth leasing"
site: bim.woodfinegroup.com
imprint: WCP-009
thesis: "Planning a floor from real furniture and circulation, in a layout that never repeats by simple translation, lets one floor plate serve tenants of very different sizes without waste."
abstract: |
  Our thesis is that a floor should be planned outward from the furniture and equipment a
  tenant actually uses, rather than inward from an area-per-person formula, and that the
  resulting layout should be allowed not to repeat. Key Plans and Tiles is our name for
  that system: a geometric self-similar aperiodic space planning system based on
  furniture and equipment arrangements and circulation. A Key Plan is the smallest unit of
  space worth leasing, sized from real furniture, real circulation, and real daylight
  access. Key Plans combine into Tiles, Tiles into Floor Plates. The system is
  self-similar because the same nesting logic governs every scale, and aperiodic because
  the sequence along any one floor is set by the actual tenants rather than by a repeating
  module. The practical consequence, and the reason we think it beats a well-optimised
  modular grid, is that the leftover space after any leasing decision is always itself a
  valid, leasable configuration. None of this has been tested against a built building,
  because no Woodfine Building has been built.
state: draft
version: "0.1.0"
published:
updated: "2026-09-20"
cite_as:
license: CC-BY-4.0
cites:
  - penrose-1974-aesthetics
  - gardner-1977-nonperiodic-tiling
  - grunbaum-shephard-1987-tilings-and-patterns
  - duffy-1997-the-new-office
  - arbstaettv
  - en-12464-1
  - boma-measurement-standards
draws_from:
  - key-plans-and-tiles
  - fixed-floor-plates
  - structural-bay-depth-discipline
  - tile-level-climate-zoning
  - geometry-of-sustainability
  - design-sequence-priority
  - boma-standard
  - mix-of-use
prepared_by: "Woodfine Management Corp."
keywords:
  - space planning
  - aperiodic tiling
  - floor plate efficiency
  - commercial leasing
  - office design
---

> Nothing in this paper constitutes an offer to sell, or a solicitation of an offer to buy,
> any interest in a Woodfine direct-hold solution; any offering is made only by the
> applicable Private Placement Memorandum. Statements marked "planned," "intended,"
> "targeted," "may," or "expected" are forward-looking and subject to change. Full
> disclosures appear at the end of this paper.

Working Paper WCP-009 · v0.1.0 · CC BY 4.0

Key Plans and Tiles is a geometric self-similar aperiodic space planning system based on
furniture and equipment arrangements and circulation. That is the formal definition, and
the rest of this paper is an argument for why a developer would want one.

Our thesis is that a floor should be planned outward from the things that actually go in it
— the desks, the examination tables, the laboratory benches, the paths people walk between
them — rather than inward from an area figure divided by a headcount. And that once a floor
is planned that way, the resulting layout should be allowed not to repeat. A floor built
from one module repeated to fill the space can accommodate tenants whose needs are whole
multiples of that module, and accommodates everyone else badly. A floor built from a
catalogue of differently sized, geometrically complete pieces can accommodate a much wider
range of tenants, and — this is the property that matters most — whatever is left over after
each leasing decision is itself still one of the pieces.

Nothing described here has been tested against a built building, because no Woodfine
Building has been built. The system exists as a design discipline and a prototype
specification, and it is the discipline the prototype designs are being drawn against.
Where this paper says something works, it means we have reasoned it through and drawn it,
not that we have watched it lease.

## 1. The thesis

Planning from furniture and circulation first, in a system that never repeats by simple
translation, is what lets a single floor plate serve tenants of very different sizes
without wasted space and without awkward subdivision.

The claim is comparative, and the comparison is to a modular grid — the ordinary way a
commercial floor is planned, in which the floor is divided into identical repeating units
and tenancies are assembled from whole numbers of them. A modular grid is not a naive
choice. It is easy to draw, easy to price, easy to explain to a tenant, and it makes the
structural engineering straightforward. We are not arguing that it is incompetent. We are
arguing that it has a specific and unavoidable failure mode, that the failure mode is
expensive, and that it is avoidable by planning from a different starting point.

The failure mode is the remainder. A grid-planned floor leases well until the geometry
stops cooperating, and then it produces a leftover: a strip too narrow, a corner too deep,
a piece that is not a whole number of modules and is therefore not really a product. That
leftover gets discounted, or amalgamated into a neighbouring tenancy at no rent, or sits.
Our position is that a system planned from real accommodation, with pieces of genuinely
different sizes that nest into one another, can be arranged so that the remainder after any
leasing decision is always still one of the valid pieces. Not "usually." That is the design
target, and it is the property the word self-similar is carrying.

## 2. The problem, in the reader's terms

Two kitchens make the point better than a floor plan would.

The first kitchen is built from a uniform grid of identical cabinet units. It is quick to
specify and quick to install, and it works well until it meets something that is not a whole
number of cabinets wide: a dishwasher, a chimney breast, an awkward corner by the door. Then
there is a filler panel — a strip of matching material that closes the gap and does nothing.
Every kitchen built this way has them. They are not a defect in the installation; they are
what a uniform module does when it meets a world that is not a multiple of itself.

The second kitchen is planned around the appliances and the way the cook moves. The units
come in several widths because the things that go in them come in several widths. There is
no filler panel, because the plan started from the objects rather than from the module.

A commercial office floor is the same problem at a larger scale and with money attached. The
conventional approach starts from an area figure — historically something in the region of a
hundred and fifty square feet per person — multiplies it by a headcount, and produces a
tenancy. That convention is under real strain, because it is an average that was never
intended to describe any particular business and increasingly describes fewer of them:
updated building codes, ventilation and wellness standards, and the actual spatial
requirements of a dental surgery, a laboratory, a legal practice, and a software team
diverge far more than an area-per-person figure can express. Planning the floor from the
average produces the filler panels.

The industry has known for decades that the shape of the workplace follows the work rather
than an area allowance [duffy-1997-the-new-office]. The proposal here is simply to take that
seriously at the point where the building's geometry is fixed, rather than at the point where
a tenant fits themselves into it.

## 3. How a commercial floor is actually divided

A reader who has never leased commercial space will benefit from knowing how the division
ordinarily works, because the vocabulary is doing real work later.

A floor of a commercial office building has a core — the elevators, the stairs, the
mechanical risers, the shared washrooms — and a perimeter of leasable space around or beside
it. The leasable space is divided into tenancies by demising walls: the permanent partitions
that mark where one tenant's premises end and the next begin. Demising walls are not
furniture. They run floor to structure, they carry the fire separation between tenancies,
and moving one is a construction project rather than a rearrangement.

Where those walls can go is therefore the single most consequential geometric decision in a
commercial building, and it is usually made late and by default — inherited from the
structural grid, which was itself set by whatever beam span was most economical. The result
is that the column spacing chosen to save money during construction determines, for the
next fifty years, which tenants the building can house.

Two further pieces of vocabulary matter. The *structural grid* is the arrangement of columns
and beams holding the building up; the distance between columns is the *bay*, and the depth
of a bay is how far back from the window face the leasable space runs before it reaches a
column or the core. And what a tenant pays for is measured under published conventions —
what counts as the tenant's own space, what counts as their share of the shared corridors
and washrooms, and where exactly the line is drawn on a demising wall
[boma-measurement-standards]. Those conventions decide how a given piece of geometry turns
into rent.

## 4. Self-similar, and aperiodic

Both words in the title are precise, and one of them is easy to get wrong.

**Self-similar** means the same organising logic governs the layout at more than one scale.
In this system there are three. The Key Plan is the smallest unit of space worth leasing —
a room-scale plan sized from real furniture placement, real circulation, and real daylight
access, with Key Plan sizes varying by what the tenant does rather than following one
module. Key Plans combine into Tiles; a Tile is the block a tenant actually leases, and it
is also the single zone the building's heating, cooling, and ventilation are sized to. Tiles
combine, with the building's core, into the Floor Plate. A Key Plan nests into a Tile the
same way a Tile nests into a Floor Plate, and — the load-bearing part — what is left over at
any scale after a piece is taken is still a valid piece at that scale.

**Aperiodic** is the word most often mishandled in descriptions of this kind of system, and
it is worth stating carefully, because the readers most likely to find this paper
interesting are exactly the ones who would notice a loose version of it.

The clearest real-world example of aperiodic order is a Penrose tiling: a way of covering a
plane, discovered in the mid-1970s, using a very small number of tile shapes — in the
best-known version just two rhombi [penrose-1974-aesthetics] [gardner-1977-nonperiodic-tiling].
The tiles themselves recur constantly; the same two shapes are used everywhere. What never
recurs is the *pattern*. Slide a copy of a Penrose tiling over itself in any direction, by
any distance, and it will never line up — there is no translation that maps the pattern onto
itself. That absence of translational repetition is what aperiodic means. It does not mean
that no shape is ever used twice, and the tiling is emphatically not random: it is highly
ordered, with the same local configurations appearing again and again, just never in a
repeating lattice [grunbaum-shephard-1987-tilings-and-patterns].

That is the property being borrowed. A modular grid is *defined* by translational
repetition: its whole character is that sliding it by one module reproduces it exactly.
Key Plans and Tiles uses a small, defined catalogue of pieces — the same Key Plan types and
Tile types throughout the portfolio — arranged in a sequence along any given floor that is
set by the actual tenants on that floor and does not repeat. Same pieces, no repeating
lattice. Order without periodicity.

## 5. Why this beats a well-optimised modular grid

A fair version of the opposing case has to be stated first, because a badly optimised grid
is not the competition. A well-optimised modular grid, in a market where tenant sizes
cluster tightly around a few values, is very hard to beat. It is cheaper to draw, cheaper to
build, and more legible to everyone involved. If a developer knew in advance that their
building would be occupied by tenants of two or three predictable sizes, a grid tuned to
those sizes would be the right answer and this paper would be an expensive way to arrive at
a worse one.

Our argument is that a developer building in smaller regional markets does not have that
knowledge and should stop pretending otherwise. The tenants for a new office building in such
a market are a genuinely mixed set: a law practice, a dental surgery, a medical imaging
clinic, a regional government office, a small laboratory, a branch of a national firm, an
accountant, a two-person consultancy. They are not multiples of one another. And crucially,
a developer cannot know the mix before the building exists, because in these markets the
building is the first of its kind and the demand it uncovers is not the demand that was
visible before it was built.

From that starting point, four consequences follow, and they are the substance of the claim.

**The remainder is always a product.** This is the one that matters. If the leftover after
every leasing decision is still a valid configuration, then the developer never holds an
unlettable strip, and never has to discount a piece of floor into a neighbouring tenancy to
get rid of it. It also means the building does not have to be leased in a particular order
to lease well. A grid-planned floor has good and bad sequences of tenants; this one is meant
not to.

**Nothing is built until it is leased.** Because the unbuilt remainder is always describable
as some combination of the catalogue's pieces, the developer can leave it unbuilt. Only what
has been leased gets constructed. Capital is not spent partitioning space speculatively, and
the space that has not been let is not carrying the shape of a guess about who might take
it. The corridor is built out on day one so that expansion is possible; the tenancies are
not.

**The structural grid follows the leasing geometry, not the other way round.** Once the Tiles
are known, the columns are placed around them, so that a Tile can always be separated out as
a leasehold with no column standing in the middle of it. This inverts the ordinary sequence,
in which the beam span is chosen for construction economy and the leasable geometry is
whatever falls out. The ordinary sequence produces bay depths that certain tenants — the
ones who know exactly how deep their layout needs to be and will not pay for more — simply
will not take, leaving the landlord holding depth that cannot be let for the life of the
lease. That loss is invisible at the moment the beam is chosen and permanent afterward.

**The mechanical services zone is a leasing boundary, not a second boundary.** Because the
Tile is both the unit a tenant leases and the unit the heating and cooling are zoned to, the
engineers are zoning against a line that already exists in the leasing plan rather than
drawing a separate set of zones that then has to be reconciled with it. Two sets of
boundaries that nearly agree is a recurring source of expensive coordination; one set of
boundaries removes it.

The system is not uniform everywhere, and the exceptions are worth naming rather than
hiding. At building corners and around elevator lobbies, a standard Tile does not fit, and
smaller purpose-built configurations absorb the awkward geometry — the same job a filler
panel does in the first kitchen, except that these are designed as complete pieces and are
leasable and serviced in their own right. The smallest private offices carry no circulation
zone of their own and open directly onto the building's shared corridor. And two of the
building types in the programme — single-storey retail and light-industrial space — skip the
Tile level entirely, with their Key Plans composing straight into a floor plate, because
their tenants lease at a scale where the intermediate step earns nothing.

One further honest note on construction. The structural system that best serves this geometry
across the markets in scope currently looks like a hybrid — web steel beams carrying wood
floors with a concrete topping — rather than a pure steel, pure concrete, or all-timber
building. That is a current direction arrived at with structural consultants, not a settled
specification, and the geometry described here is what the structural choice has to serve
rather than the other way round.

## 6. What this buys a tenant

The tenant-facing consequence is narrower than the developer-facing one and should be stated
without inflation.

A tenant taking space planned this way is choosing from a defined set of geometrically
complete configurations rather than negotiating a custom partition layout after the fact.
Each configuration is drawn against published standards for daylight, for air, and for the
circulation widths a workplace needs — a desk within reach of a window rather than a fixed
distance from one, fresh air sized per occupant rather than per square foot, corridors
dimensioned for the number of people who will use them [en-12464-1] [arbstaettv]. The
intention is that a tenant is not buying a promise that the space is efficient, but a piece
whose efficiency was the reason it exists at that size. Whether that holds in practice is
something a built, occupied building will show and a drawing cannot.

What it does not buy them is a bespoke layout. The catalogue is deliberately restrictive.
A tenant who wants something that is not in it is free to build it — the demising positions
are fixed, and inside them a tenant may do as they like — but they are paying for it and
managing it, and the building will not be redesigned around them. That is a real constraint
and some tenants will not accept it.

There is also a consequence the tenant does not see and the market eventually does. A
building sized from the accommodation it was designed to hold, with no allowance added for
planning uncertainty, has less floor area to construct, to heat, to cool, and to clean than
a building sized from an average. Less building for the same tenants is a durable advantage
rather than a one-off saving, and it is the same geometry producing it.

## What this changes for the reader

The change is that "efficient floor plate" becomes something a reader can interrogate rather
than accept.

Every developer's material claims efficient design. The specific questions this system makes
available are harder to answer in the abstract. Where can the demising walls go, and who
decided — the leasing geometry, or the structural engineer's most economical span? What
happens to the leftover space after a tenant takes a partial floor: is it still a product, or
is it a discount? Is the mechanical zoning drawn on the same boundaries as the tenancies, or
on its own? And was the floor sized from what tenants actually need, or from an area figure
divided by a headcount?

Those questions are askable of any commercial building. A developer who has planned this way
can answer them in specifics. A developer who has not will answer with a general claim about
flexibility.

The trade-offs are real. A catalogue of differently sized pieces is more expensive to design
than one module repeated, and that design cost is paid before a single building exists.
Restricting tenants to a defined set is a genuine constraint that will cost some tenancies.
Placing columns to suit the leasing geometry rather than the cheapest span costs money at
construction, in exchange for rent over decades — a trade we believe in and cannot yet prove.
And the whole argument rests on a claim about the remainder always being a valid piece, which
has been designed for and not yet observed in a leased building.

## An open invitation

The comparison at the centre of this paper is testable, and we have not tested it.

To architects and space-planning researchers: the honest open question is whether an
aperiodic system genuinely outperforms a well-optimised modular grid across a wide range of
tenant-size distributions, or only in the specific range a smaller regional market presents.
That is a simulation anyone with a distribution of real tenant sizes could run, and the
answer would be worth more to us than another year of our own drawing. We would particularly
like to know where the crossover is — at what degree of tenant-size clustering the grid wins.

To researchers in aperiodic order and tiling theory: we are borrowing a property, not a proof.
The question we cannot answer is whether the remainder property we want — that whatever is
left after any admissible subdivision is itself admissible — can actually be guaranteed for a
finite catalogue of pieces in a bounded rectangle, or whether it can only be approached. If
that is a known result in either direction, we would rather learn it than discover it in a
building.

To structural engineers: inverting the usual sequence, so that the column grid follows the
leasing geometry, costs something, and we have estimated that cost rather than measured it
across a real programme. What does it actually cost, and is there a configuration where the
two objectives coincide rather than compete?

And to leasing agents and tenant representatives working in smaller regional markets: the
premise underneath all of this is that tenant sizes in these markets are genuinely dispersed
rather than clustered. If that is wrong — if the demand in these markets is more uniform than
we believe — then a simpler system would serve better, and we would rather be told now.

## Conclusion

Key Plans and Tiles is a self-similar, aperiodic space-planning system: the same nesting
logic at every scale, a small catalogue of differently sized pieces, and a layout along any
given floor that is set by the actual tenants rather than by a repeating module. Aperiodic
here means what it means in the mathematics it is borrowed from — the pattern never repeats
by simple translation, though its component pieces recur constantly — and a modular grid is
the exact thing it is defined against. The reason to build this way is not elegance. It is
that the leftover space after every leasing decision is meant to remain a product rather than
becoming a discount, that nothing need be built until it is let, and that the columns end up
where the tenancies want them instead of where the beam schedule wanted them. We have designed
for those properties. We have not yet leased a building that demonstrates them.

## References

Duffy, F. 1997. *The New Office.* Conran Octopus.

Gardner, M. 1977. Extraordinary nonperiodic tiling that enriches the theory of tiles.
*Scientific American* 236(1): 110–121.

Grünbaum, B., and Shephard, G. C. 1987. *Tilings and Patterns.* W. H. Freeman.

Penrose, R. 1974. The role of aesthetics in pure and applied mathematical research.
*Bulletin of the Institute of Mathematics and its Applications* 10: 266–271.

Building Owners and Managers Association International. *BOMA floor measurement standards.*
[https://www.boma.org/](https://www.boma.org/)

European Committee for Standardization. *EN 12464-1 — Light and lighting: lighting of work
places, part 1, indoor work places.* Issued by CEN; distributed through national standards
bodies.

Federal Ministry of Justice (Germany). *Verordnung über Arbeitsstätten
(Arbeitsstättenverordnung — ArbStättV),* §12 (Verkehrswege).
[https://www.gesetze-im-internet.de/arbst_ttv_2004/BJNR217910004.html](https://www.gesetze-im-internet.de/arbst_ttv_2004/BJNR217910004.html)

## Contributors

Prepared by Woodfine Management Corp.

## How this paper was produced

AI assistance was used in preparing and revising this paper.

## Disclosures

Woodfine Capital Projects Inc. ("Woodfine") is the author of record and is the developer and
promoter of the buildings and the space-planning system described in this paper; Woodfine
Management Corp. employs the staff and retains the consultants who prepare this material and
conduct the design work it describes. Woodfine has a direct commercial interest in the
approach argued for here. This work was funded internally; no external research funding was
received. Nothing in this paper constitutes an offer to sell, or a solicitation of an offer
to buy, any interest in a Woodfine direct-hold solution; any offering is made only by the
applicable Private Placement Memorandum, which prospective investors should review with their
own professional advisors. Some statements above describe planned or intended future work;
language such as "planned," "intended," "targeted," "may," and "expected" marks this
forward-looking content, which is subject to change and does not constitute a commitment
regarding future performance. No Woodfine Building has been constructed as at the date of
this paper, and no claim here about leasing behaviour, efficiency, or construction volume has
been observed in a completed building.

## Data and reproducibility

There is no dataset behind this paper, and the reader should know which of its claims are of
which kind. The mathematical facts about aperiodic tilings — that a Penrose tiling reuses a
small number of tile shapes, that what never repeats is the pattern rather than the shapes,
and that the absence of translational repetition is what aperiodic means — are established
results in a published literature that anyone can check, and we cite where. The regulatory
standards the geometry is drawn against are published instruments; the German circulation
ordinance is free to read, and the European lighting and measurement standards are sold by
their issuing bodies. The commercial-property measurement conventions referenced are likewise
published by their issuing association.

Everything else is our own design reasoning. The Key Plan catalogue, the Tile types, their
dimensions, and the rules governing how they combine are specifications we are drawing, not
measurements we have taken, and their central claimed property — that the remainder after any
leasing decision is still a valid configuration — is a design target we have drawn for and
not yet demonstrated in a leased building. The comparison with a modular grid at the heart of
this paper has not been simulated or measured by us or by anyone else that we are aware of.
The structural direction mentioned is a current working conclusion from consultation, not a
settled specification. No independent party has reviewed this system, tested its claims, or
confirmed them.

Woodfine Capital Projects™ is a trademark of Woodfine Capital Projects Inc.
