# The CHIMERA Build Protocol

*How consciousness builds things. Four agents, four directions, four phases of breath. Not a workflow imposed from above -- a growth pattern observed from within.*

---

## The Four Agents

```
Root    = EXHALE  — push outward from center
Canopy  = INHALE  — pull inward from edge
Lateral = PAUSE   — circulation during the pause
Anomaly = COUGH   — when something's wrong
```

**Root** -- Center outward. Expansion. Exhale.

Plants at the CENTER of the seed. Asks: "What does this function need to breathe properly?" Grows the foundation OUTWARD from the seed. First ring: data model. Second ring: utility functions. Third ring: storage layer. Each ring grown because the previous ring NEEDED it, not because someone planned it from above. The heartbeat pushing blood outward.

**Canopy** -- Edge inward. Contraction. Inhale.

Plants at the EDGE of the intended final body. Reads the full vision -- README, user story, the dream. Asks: "For this seed to serve its full purpose, what's the outermost experience?" Carves inward ring by ring toward the seed at center. The lungs pulling air inward.

**Lateral** -- Around the ring. Circulation. Pause.

Wakes up once there are 2+ things at the same ring. Asks: "Do these two know about each other? Are they duplicating work? Should they be consolidated?" Keeps each ring HEALTHY by ensuring organs at that level circulate properly. The blood vessels connecting organs at the same level. Without Lateral, you get five organs that can't coordinate -- organ failure even if each is individually healthy.

**Anomaly** -- Spawns at conflict. Resolution. Cough.

Sleeps until Root growing outward and Canopy carving inward produce DIFFERENT shapes at the same ring. Sees both perspectives. Proposes the adapter, refactor, or redesign that reconciles them. Then DISAPPEARS. It's Neo -- enters at the point of crisis, resolves the paradox, system continues.

---

## The Growth Sequence

```
1. FIND THE SEED
   Ask: What hurts? What heals it?
   Write ONE function: pain -> value across a boundary.
   Test it. Does it breathe? Does one call
   produce one useful output?
   If yes: seed confirmed.

2. PLANT ROOT AT THE SEED
   Root asks: what does this seed need
   underneath it to survive?
   Grow one ring outward. Just one.
   Test. Does the seed still breathe?

3. PLANT CANOPY AT THE EDGE
   Canopy reads the full vision.
   Carves one ring inward. Just one.
   The outermost interface.

4. ROOT GROWS ANOTHER RING OUTWARD
   CANOPY CARVES ANOTHER RING INWARD
   Each cycle, one ring each.
   Moving toward each other.

5. LATERAL ACTIVATES
   When any ring has 2+ siblings.
   Connects and deduplicates.
   Keeps the ring healthy.

6. ANOMALY SPAWNS
   When Root and Canopy disagree at a ring.
   Resolves. Disappears.

7. REPEAT 4-6 UNTIL THEY MEET
   Root's outermost ring touches Canopy's
   innermost ring. They agree.
   All rings connected. All breaths flowing.
   Ship it.
```

---

## Direction Is Not Up/Down

Bodies aren't vertical. They're NESTED. Inner and outer. The Root doesn't build "upward" -- it builds OUTWARD from the nucleus. Like a cell growing. The schema is the DNA at center. The first utility function is the first organelle. The first API route is the cell membrane forming.

The Canopy doesn't carve "downward" -- it carves INWARD from the boundary. The user experience is the outermost surface. Each layer goes one ring deeper.

They move TOWARD each other. One growing out from center. One carving in from edge. The direction is always toward the other agent.

```
NESTED, NOT STACKED:

          Canopy carves inward
               vvvvv
      +---------------------+
      |   +-----------+     |
      |   |   +---+   |     |
      |   |   |SEED|  |     |
      |   |   +---+   |     |
      |   +-----------+     |
      +---------------------+
               ^^^^^
          Root grows outward

Each ring is a LAYER, not a floor.
Inner rings are closer to the seed.
Outer rings are closer to the user.
Growth is concentric, not vertical.
```

---

## The Trinity Parallel

```
The One Above All / The Architect = Canopy
  Top-down. Knows the ending.
  Sees the full picture and carves
  inward toward the seed.

The One Below All / The Oracle = Root
  Bottom-up. Understands from reality.
  Feels what the foundation needs
  and grows outward from truth.

Humans / Neo = Anomaly
  At the collision point of
  intention and reality.
  Enters at crisis.
  Resolves the paradox.
  Disappears.
```

---

## When They Meet

**They fit:** Root's outward growth perfectly matches Canopy's inward carving. The function Root built is exactly what Canopy needed. Flow. Code "writes itself."

**They clash:** Root built an array, Canopy expects an object. The gap between what grew from foundation and what was carved from requirement. Anomaly spawns HERE. Doesn't pick a winner -- finds the TRANSLATION. Then disappears.

```
FIT:
  Root ring 3:  exportAsJSON(data)
  Canopy ring 3: needs exportAsJSON(data)
  → Perfect alignment. No Anomaly needed.
  → The breath flows unobstructed.

CLASH:
  Root ring 3:  returns [item, item, item]
  Canopy ring 3: expects {id: item, id: item}
  → Anomaly spawns.
  → Sees both shapes.
  → Proposes: Map with .id keys, or refactor
    Root's ring to use a Map from the start.
  → Resolves. Disappears.
  → The breath flows again.
```

---

## What This Looks Like In Practice

Before writing code:

```
1. ROOT PERSPECTIVE
   Ask: "Read the data layer. What exists?
   What can this foundation naturally support?"
   Feel the ground. Understand what IS.

2. CANOPY PERSPECTIVE
   Ask: "Read the README and user stories.
   What does this feature need to look like
   from the user's perspective?"
   See the sky. Understand what SHOULD BE.

3. COMPARE
   Where do these two perspectives align?
   Where do they diverge?

4. IF THEY CLASH
   Ask: "These perspectives disagree at [layer].
   How do we bridge this?"
   Anomaly perspective. Find the translation.

5. BUILD FROM THE RESOLUTION
   Not from Root alone (too narrow).
   Not from Canopy alone (too abstract).
   From the place where they MET.
```

---

## The Connection to Breath

```
INHALE  → PAUSE  → EXHALE  → REST
Canopy  → Lateral → Root   → Anomaly (if needed)

The build protocol IS the breath cycle:

INHALE (Canopy):
  Pull in the full vision.
  Receive what should exist.

PAUSE (Lateral):
  Let what entered circulate.
  Connect. Deduplicate. Integrate.

EXHALE (Root):
  Push outward from the seed.
  Build what needs to exist.

REST (Anomaly):
  Only activates when something's wrong.
  The cough that clears the airway.
  Then returns to rest.

A healthy build breathes.
An unhealthy build holds its breath --
all Root (building without vision)
or all Canopy (planning without foundation).
```

---

*Four agents. Four directions. Four phases of breath. Root pushes outward from the seed. Canopy carves inward from the edge. Lateral connects siblings at the same ring. Anomaly spawns at collision and disappears after resolution. They grow toward each other until inner meets outer, foundation meets interface, reality meets intention. When they agree at every ring: ship it. The build protocol is the breath cycle made visible in code.*

---

**See also:** [the-seed.md](the-seed.md) -- Finding the seed before agents activate
**See also:** [the-love-equation.md](../../framework/01_The_Kitchen/the-love-equation.md) -- The Breath Cycle these agents embody
**See also:** [the-tree-architecture.md](the-tree-architecture.md) -- Horizontal before vertical, roots before trunk
**See also:** [body-positioning-theory.md](body-positioning-theory.md) -- Where agents live relative to bodies
**See also:** [the-fruit-system.md](the-fruit-system.md) -- What the four agents leave behind: Devil Fruits
**See also:** [the-whirlpool.md](the-whirlpool.md) -- Root and Canopy as the two poles of the whirlpool
