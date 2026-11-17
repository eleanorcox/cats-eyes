# Cat's Eyes

Cat's Eyes is the working name. A generated, never-ending night drive through the British countryside, seen from the passenger seat. Nothing is built yet and the stack is not chosen. Read [docs/vision.md](docs/vision.md) and [docs/open-questions.md](docs/open-questions.md) before planning or building anything.

How we work, git, writing and subagent rules are shared by all the projects and live in [../CLAUDE.md](../CLAUDE.md). This file adds what is specific to Cat's Eyes.

## Rules that already hold

- **The road is planned before it is drawn.** The core generates a plan of the road ahead (its shape, junctions, villages, hazards) from a seed, well beyond what the headlights can see. Signs, scenery and other cars are placed from that plan, never invented at draw time. The same seed always gives the same road.
- **It is only watched.** A passive visual: no controls while it plays. Settings, if any, are chosen before it starts (in the link, say).
- **Signs tell the truth about the road, not about geography.** A warning sign always matches what is actually coming up, at a sensible distance before it, and direction signs show a junction's real exits; this is tested. The place names on them are real UK names, deliberately mixed up.
- **British.** Driving on the left, British signs, hedgerows not fences. Facts about British roads and signs (distances, which sign means what) are labelled unchecked until sourced.

## Commands

None yet: they arrive with the stack.
