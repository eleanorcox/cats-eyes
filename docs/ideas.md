# Ideas

Every idea so far, each with the smallest version worth building. Sizes are rough guesses for that smallest version: **S** is a few days, **M** is a week or two, **L** is a month or more. Eleanor's [first notes](first-notes.md) are the source of most of them.

## Summary

| Idea | Size | Depends on |
| --- | --- | --- |
| The road plan | M | nothing; this comes first |
| Being driven along it | S | road plan |
| Headlights in the dark | S | being driven |
| The car's jitter and bumps | S | being driven |
| Cat's eyes, white lines, bollards | S | headlights |
| Roadside: hedgerows, fields, trees | M | road plan |
| Roadside clutter: roadkill, plastic in the hedge | S | roadside |
| Road signs that match the road | M | road plan |
| Mixed-up UK place names | S | signs |
| Kinds of road | M | road plan |
| Roundabouts | M | kinds of road, signs |
| Roadworks | M | signs |
| Villages, and the odd weird one | M | kinds of road, signs |
| The car in front | M | road plan, headlights |
| Kinds of vehicle | M | the car in front |
| Oncoming cars | S | headlights |
| People in the cars | M | the car in front |
| Inside the car, and glancing at the driver | M | being driven |
| Fog, rain and lightning storms | M | headlights |
| Sound and music | S, then M | being driven |
| Projected as an installation | S | most of the above |

## The road plan

The heart of it. A **generator** that, from a seed, produces the road as a list of pieces: straight, bend left or right (how sharp), rise, dip, roundabout, junction, roadworks, village. It runs well ahead of the car, say a kilometre or two, so everything else can look ahead in it. Behind the car, old pieces are thrown away.

- **Smallest version:** a seeded list of straights and bends, turned into a smooth centre line (a **spline**: a curve drawn smoothly through a set of points), with no gaps or kinks where one piece joins the next.
- **Why it comes first:** signs, scenery and other cars are all placed from it. Kept free of drawing code, it can be tested thoroughly: same seed, same road; no kinks; bends never tighter than a car could take.

## Being driven along it

The camera sits in the passenger seat (on the left in a British car) and moves along the road at the speed a careful driver would take it: slower into bends, slowing for roundabouts and villages.

- **Smallest version:** a flat grey ribbon on black ground and a camera gliding along it forever.

## Headlights in the dark

Two **spotlights** (lights that shine in a cone, like a torch) from the front of the car, a dark sky, and **fog** so the distance fades out. Dipped and full beam: the driver dips for oncoming cars and when following one.

- **Smallest version:** dipped headlights lighting the ribbon. Probably the moment it first feels like the idea.
- **Unknown:** shadows from several lights are expensive to draw; how much the scene can hold before it stutters needs measuring.

## The car's jitter and bumps

Small, constant shake from the road surface, bigger jolts over potholes and cattle grids, a lean into bends and a nod when braking. The road plan can mark rough patches so the bumps come from the road, not at random.

## Cat's eyes, white lines, bollards

Centre-line dashes, edge lines, cat's eyes that glow only when the headlights hit them, white bollards with reflective bands at bends and junctions, fluorescent marker posts along the verge.

- **Smallest version:** dashes and cat's eyes along the centre line, bright when lit. The name of the project, so worth having early.

## Roadside: hedgerows, fields, trees

The side of the road changes: hedgerow, an open field behind a fence or gate, a line of trees, woodland closing in. Several kinds of tree (oak, ash, hawthorn, birch, conifers in plantations), each with its own shape. Drawn by **instancing** (drawing many copies of one shape in one go, which is how thousands of trees stay fast).

- **Smallest version:** a continuous hedge on both sides and two kinds of tree scattered behind it.

## Roadside clutter: roadkill, plastic in the hedge

The details that make it real and a little grim: a carcass on the verge (handled at a distance, a shape in the headlights rather than gore), a plastic bag snagged in a hawthorn, a lost glove on a fence post, a sign bent by a collision.

## Road signs that match the road

Warning signs placed a set distance before what they warn of: bend, double bend, junction, roundabout, steep hill, deer, roadworks, a village's name, speed limits. Direction signs before roundabouts and junctions show their real layout.

- **Smallest version:** a bend sign before every sharp bend, tested so that every sharp bend has one and no sign stands before a straight.
- **Unknown:** the real rules for how far before a hazard a sign goes (the UK's Traffic Signs Manual has them; unchecked). The sign designs are Crown copyright, possibly usable under the Open Government Licence (unchecked). The lettering on British signs is the Transport typeface; free copies exist, licence unchecked.

## Mixed-up UK place names

Real place names from all over the UK on the same signs, so the signs look right but the geography is nonsense. A list of real names could come from the Ordnance Survey's free gazetteer, OS Open Names (unchecked). Village name signs use the same list.

## Kinds of road

Single-track lanes with grass down the middle and passing places; B-roads with a centre line; the occasional A-road. The road changes between them at junctions and roundabouts.

## Roundabouts

The car goes round and takes an exit; a car in front may take a different one and be gone. Direction signs before it show its real exits.

- **Unknown:** roundabouts are the hardest piece of road to generate: the centre line has to branch, and the road plan has to choose an exit.

## Roadworks

A "Road works ahead" sign, then cones, temporary traffic lights on red, a parked digger, yellow flashing lights in the dark.

## Villages, and the odd weird one

A name sign and a 30 limit; houses close to the road, some lit windows, a pub, a church, streetlights, a bus shelter; then the countryside again. Occasionally a village that is wrong: every window lit, or none; a figure standing still; the same house repeated; a village with no name.

## The car in front

For stretches you follow another car: its red tail lights, and its headlights throwing a wedge of light across the trees and hedges ahead of it. Then it turns off at a roundabout or junction and you are alone again.

- **Smallest version:** a car ahead on the same road, lighting the trees with its own headlights, that turns off at the next junction.
- Placed from the road plan, so it knows where it is going to turn.

## Kinds of vehicle

Hatchbacks, estates, a tractor, a lorry, a van with orange stripes (the chevrons on highway maintenance vans).

## Oncoming cars

Now and then, a glow over a rise, then headlights, then gone. Rare: it is mostly empty.

## People in the cars

Someone visible at the wheel of a passing car, lit by its dashboard. A passenger, a dog, a stack of boxes. Simple and suggestive rather than detailed.

## Inside the car, and glancing at the driver

From the passenger seat: the dashboard's glow, the windscreen's edges, the rear-view mirror showing the dark road behind. Now and then the view turns by itself, as a passenger's head would: out of the side window, or to the driver, lit by the dashboard. Who the driver is (someone you know, a stranger, nobody) could do a lot for the mood.

## Fog, rain and lightning storms

Mist in the dips that the headlights turn into a white wall; rain on the windscreen with wipers; a lightning storm where each flash shows the whole landscape for an instant, then black.

## Sound and music

The engine's hum, tyres on wet or dry road, rain, the indicator ticking at a roundabout. A radio that drifts between stations. Perhaps the drive reacts to music playing in the room or on its radio: the weather, speed or the light following it. Nobody controls it; it only listens. [Gloaming](../../gloaming/docs/ideas.md) also wants to respond to sound, so what is learned in one helps the other.

## Projected as an installation

A car seat facing a wall-sized projection, as if the wall were the windscreen. Brings it into the projection work alongside the aquarium.
