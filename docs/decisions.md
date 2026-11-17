# Decision log

A record of the design decisions in this project: what was decided, when, what prompted it, and what it replaced. It exists so the reasoning can be found later, in particular when writing about the work.

## How this log works

- **One entry per decision**, numbered in the order they were made, newest at the bottom.
- **Entries are not rewritten.** When a decision changes, a new entry is added that says what changed and why, and the old entry's status becomes "Replaced by" with a link.
- **Add the entry when the decision is made**, in the same piece of work.
- **"What prompted it"** records the situation at the time, in gist, not word for word.
- **Record the alternatives**, including the ones that lost, and why.

Statuses: **Proposed**, **Decided**, **Built**, **Replaced by N**.

Template:

```markdown
## N. Title

- **Date:**
- **Status:**
- **What prompted it:**
- **Decision:**
- **Alternatives considered:**
- **What follows from it:**
```

## Index

| No. | Decision | Date | Status |
| --- | --- | --- | --- |
| [1](#1-working-name-cats-eyes) | Working name: Cat's Eyes | 17 Nov 2026 | Decided |
| [2](#2-the-road-is-planned-ahead-of-being-drawn) | The road is planned ahead of being drawn | 17 Nov 2026 | Proposed |
| [3](#3-seen-from-the-passenger-seat) | Seen from the passenger seat | 17 Nov 2026 | Decided |

## 1. Working name: Cat's Eyes

- **Date:** 17 November 2026
- **Status:** Decided
- **What prompted it:** Setting up repositories for several new projects. The idea was described as a generated night drive through the British countryside.
- **Decision:** Cat's Eyes, as a working name; the repository and folder are `cats-eyes`.
- **Alternatives considered:** Night Drive (plain and clear, but common), Unclassified (the British term for minor roads), Dipped Beam.
- **What follows from it:** The repository name becomes the address if it is published under `eleanorcox.rocks/<name>`.

## 2. The road is planned ahead of being drawn

- **Date:** 17 November 2026
- **Status:** Proposed
- **What prompted it:** The wish for road signs that match what is coming up. A sign can only be right if what it warns of is already decided when the sign is placed.
- **Decision:** A generator produces a plan of the road from a seed, well ahead of the car. Signs, scenery and other cars are placed from the plan. The plan has no drawing code in it, so it can be tested on its own, and the same seed always gives the same road (the shared determinism rule).
- **Alternatives considered:** Generating the road just in front of the camera as it is drawn. Simpler at first, but nothing could look ahead, so signs could not be truthful.
- **What follows from it:** The road plan is the first thing built, before anything is drawn.

## 3. Seen from the passenger seat

- **Date:** 17 November 2026
- **Status:** Decided
- **What prompted it:** Eleanor's first notes on the idea, brought over after the repository was set up, put the view in the passenger seat, with the thought of turning to see the driver. The docs had assumed the driver's seat.
- **Decision:** The view is from the passenger seat. Someone else drives; you watch.
- **Alternatives considered:** The driver's seat. Lost because it invites steering, which turns it into a driving game, and loses the driver as a character.
- **What follows from it:** "Watch or drive" becomes "what can the passenger do". The driver becomes something to design (open question 5). The camera sits on the left of the car.
