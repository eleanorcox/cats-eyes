# Ideas

Every idea so far, each with the smallest version worth building. Sizes are rough guesses for that smallest version: **S** is a few days, **M** is a week or two, **L** is a month or more.

## Summary

| Idea | Size | Depends on |
| --- | --- | --- |
| The road plan | M | nothing; this comes first |
| Driving along it | S | road plan |
| Headlights in the dark | S | driving along it |
| Cat's eyes and white lines | S | headlights |
| Roadside: hedges, trees, walls | M | road plan |
| Road signs that match the road | M | road plan |
| Kinds of road | M | road plan |
| Villages and place names | M | kinds of road, signs |
| Other cars | M | road plan |
| People in the other cars | M | other cars |
| Inside the car | M | driving along it |
| Weather and sky | M | headlights |
| Sound | S, then M | driving along it |
| Projected as an installation | S | most of the above |

## The road plan

The heart of it. A **generator** that, from a seed, produces the road as a list of pieces: straight, bend left or right (how sharp), rise, dip, junction, village. It runs well ahead of the car, say a kilometre or two, so everything else can look ahead in it. Behind the car, old pieces are thrown away.

- **Smallest version:** a seeded list of straights and bends, turned into a smooth centre line (a **spline**: a curve drawn smoothly through a set of points), with no gaps or kinks where one piece joins the next.
- **Why it comes first:** signs, scenery and other cars are all placed from it. Kept free of drawing code, it can be tested thoroughly: same seed, same road; no kinks; bends never tighter than a car could take.

## Driving along it

The camera moves along the centre line at a steady speed, on the left of the road, looking ahead with a slight lean into bends.

- **Smallest version:** a flat grey ribbon on black ground and a camera gliding along it forever.

## Headlights in the dark

Two **spotlights** (lights that shine in a cone, like a torch) from the front of the car, a dark sky, and **fog** so the distance fades out. Dipped and full beam.

- **Smallest version:** dipped headlights lighting the ribbon. Probably the moment it first feels like the idea.
- **Unknown:** shadows from many lights are expensive to draw; how far the scene can go before it stutters needs measuring.

## Cat's eyes and white lines

Centre-line dashes, edge lines, and studs that glow only when the headlights hit them.

- **Smallest version:** dashes and studs along the centre line, bright when lit. The name of the project, so worth having early.

## Roadside: hedges, trees, walls

Hedgerows close to the road, trees, stone walls, field gates, telegraph poles. Placed from the plan and the seed, drawn by **instancing** (drawing many copies of one shape in one go, which is how thousands of trees stay fast).

- **Smallest version:** a continuous hedge on both sides and scattered trees.

## Road signs that match the road

Warning signs placed a set distance before what they warn of: bend, double bend, junction, crossroads, steep hill, deer, a village's name, speed limits.

- **Smallest version:** a bend sign before every sharp bend, tested so that every sharp bend has one and no sign stands before a straight.
- **Unknown:** the real rules for how far before a hazard a sign goes (the UK's Traffic Signs Manual has them; unchecked). The sign designs themselves are Crown copyright, possibly usable under the Open Government Licence (unchecked).

## Kinds of road

Single-track lanes with grass down the middle and passing places; B-roads with a centre line; the occasional A-road. The road changes between them at junctions.

## Villages and place names

The road passes through villages: a name sign, a 30 limit, houses close to the road, a pub, a church, streetlights, then the countryside again.

- **Fun part:** generated British place names, built from real pieces (Little, Upper, -bury, -by, -thorpe, -on-the-Wold, -under-Edge).

## Other cars

Occasionally a car comes the other way: first a glow, then headlights, then gone. Rarer still, one ahead with red tail lights.

- **Smallest version:** oncoming headlights that appear over a rise and pass on the right.
- Your full beam dips as it passes, as a polite driver would.

## People in the other cars

Someone visible at the wheel as a car passes, lit by its dashboard. Simple and suggestive rather than detailed. A passenger, a dog, a stack of boxes.

## Inside the car

A dashboard with dials glowing, the edges of the windscreen, a rear-view mirror that shows the dark road behind, perhaps the driver's hands.

## Weather and sky

Rain on the windscreen with wipers; mist in the dips; a moon that silhouettes trees; stars on a clear night; a dawn eventually?

## Sound

The engine's hum, tyres on wet or dry road, rain, a radio that drifts between stations.

## Projected as an installation

A car seat facing a wall-sized projection, as if the wall were the windscreen. Brings it into the projection work alongside the aquarium.
