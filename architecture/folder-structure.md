# CHIMERA Folder Structure

**The single source of truth for the entire CHIMERA architecture. Every CC instance, every laptop, every future collaborator reads this FIRST. This doc bootstraps any machine — like DNA bootstraps a cell.**

**Last Updated:** 2026-02-11
**Total Repos:** 15
**Total Docs:** 3,117

---

## The Hierarchy

```
~/chimera/
├── nucleus/                        # THE BRAIN
│   ├── system/                     # Axiom-level truths (57 docs)
│   │   ├── axioms/                 # The 6 foundational laws
│   │   ├── scales/                 # Subatomic → galactic
│   │   ├── patterns/               # Universal patterns
│   │   ├── archetypes/             # Kirby, Mystique, Rosetta, Doomsday
│   │   ├── fiction/                # One Piece, FMA, MHA, Matrix maps
│   │   ├── theology/               # Enoch, Gnostic, Nimrod
│   │   ├── applied/                # War, etc.
│   │   ├── health/                 # System health metrics
│   │   └── architecture/           # THIS FILE. The map.
│   │   git: DrealR/chimera-system
│   │
│   └── framework/                  # THE DNA — 420 sacred docs
│       ├── seed/                   # The origin (1)
│       ├── start-here/             # Entry points (3)
│       ├── core/                   # Pure principles (14)
│       ├── deep/                   # Integration (28)
│       └── library/                # Applications (373)
│       git: DrealR/chimera-framework
│
├── guts/                           # THE THREE GUTS
│   ├── body/                       # EXPERIENCE gut — feel it (18 docs)
│   │   ├── core/
│   │   ├── deep/
│   │   ├── applied/
│   │   └── seed/
│   │   git: DrealR/chimera-body
│   │
│   ├── math/                       # PRECISION gut — prove it (21 docs)
│   │   ├── foundations/
│   │   ├── equations/
│   │   ├── proofs/
│   │   ├── translations/
│   │   └── tools/
│   │   git: DrealR/chimera-math
│   │
│   └── language/                   # MEANING gut — share it (10 docs)
│       ├── core/
│       ├── applied/
│       └── deep/
│       git: DrealR/chimera-language
│
├── domains/                        # APPLIED KNOWLEDGE
│   ├── relationships/              # Connection & healing (33 docs)
│   │   git: DrealR/chimera-relationships
│   ├── basketball/                 # The game as system (14 docs)
│   │   git: DrealR/chimera-basketball
│   ├── chess/                      # Attention warfare (16 docs)
│   │   git: DrealR/chimera-chess
│   ├── music/                      # Sound as truth (16 docs)
│   │   git: DrealR/chimera-music
│   ├── cooking/                    # Transformation (1 doc)
│   │   git: DrealR/chimera-cooking
│   ├── ai/                         # Consciousness & comprehension (18 docs)
│   │   git: DrealR/chimera-ai
│   ├── crypto/                     # Blood for systems (14 docs)
│   │   git: DrealR/chimera-crypto
│   └── stories/                    # Comedy + writing as delivery (23 docs)
│       ├── characters/             # The cast — every character is you
│       ├── bits/                   # Comedy bits — seeds to scenes
│       ├── structures/             # Comedy architecture
│       ├── techniques/             # Comedy tools
│       ├── studies/                # Comedy breakdowns — watch, extract, learn
│       └── raw/                    # Capture first, structure later
│       git: DrealR/chimera-stories
│
├── infrastructure/                 # THE BODY'S SYSTEMS
│   └── constellation/              # The breathing mind (28 docs)
│       git: DrealR/chimera-constellation
│
└── raw/                            # THE STOMACH
    └── core/                       # Unprocessed material (2,428 docs)
        ├── sessions/               # Raw session captures
        ├── docs/                   # Historical docs
        ├── projects/               # Live constellation code
        └── ...                     # Everything else
        git: DrealR/chimera-core
```

---

## Machines

```
HONEYDEW (Laptop 1):
  → Primary development machine
  → Home base
  → Where most builds happen
  → Has all repos cloned

REEMIFAI (Laptop 2):
  → Mobile/secondary machine
  → Travel laptop
  → Syncs via git pull
  → Reads this architecture doc to stay coherent

Both machines follow the SAME folder structure.
Both sync through git.
This architecture doc is the single source of truth for BOTH.
```

---

## Processing Pipeline

```
ALWAYS THIS ORDER. NEVER SKIP THE STOMACH.

1. CONVERSATION (food enters)
   Raw insight. Unstructured.

2. CORE — raw/core/sessions/ (stomach)
   Create: YYYY-MM-DD-topic.md
   Unprocessed. Unedited. Date stamped.
   THIS HAPPENS FIRST. ALWAYS.

3. ORGANS — system/, domains/, guts/ (body)
   Processed into structured docs.
   Cross-referenced. Placed correctly.

4. FRAMEWORK — framework/ (DNA)
   ONLY if insight is:
   - Universal (all domains)
   - Irreducible (can't simplify further)
   - Proven across scales
   - Not redundant with existing 420
   FLAG for review. Don't auto-add.
```

---

## Doc Count Table

| Layer | Repo | Docs | Git Remote |
|-------|------|------|------------|
| Nucleus | system | 57 | DrealR/chimera-system |
| Nucleus | framework | 420 | DrealR/chimera-framework |
| Guts | body | 18 | DrealR/chimera-body |
| Guts | math | 21 | DrealR/chimera-math |
| Guts | language | 10 | DrealR/chimera-language |
| Domains | relationships | 33 | DrealR/chimera-relationships |
| Domains | basketball | 14 | DrealR/chimera-basketball |
| Domains | chess | 16 | DrealR/chimera-chess |
| Domains | music | 16 | DrealR/chimera-music |
| Domains | cooking | 1 | DrealR/chimera-cooking |
| Domains | ai | 18 | DrealR/chimera-ai |
| Domains | crypto | 14 | DrealR/chimera-crypto |
| Domains | stories | 23 | DrealR/chimera-stories |
| Infrastructure | constellation | 28 | DrealR/chimera-constellation |
| Raw | core | 2,428 | DrealR/chimera-core |
| **TOTAL** | | **3,117** | |

---

## Sync Script

Run this on any new machine to build the full body:

```bash
#!/bin/bash
# CHIMERA SYNC — Bootstraps or updates the full architecture
# Run from home directory or wherever you want ~/chimera/

CHIMERA_ROOT="${HOME}/chimera"
GH_USER="DrealR"
MACHINE_NAME="${CHIMERA_MACHINE:-$(hostname -s)}"

echo "Machine: ${MACHINE_NAME}"
echo "Syncing at: $(date)"

# Create hierarchy
mkdir -p "${CHIMERA_ROOT}"/{nucleus,guts,domains,infrastructure,raw}

# Define repos and their locations
declare -A REPOS=(
  ["chimera-system"]="nucleus/system"
  ["chimera-framework"]="nucleus/framework"
  ["chimera-body"]="guts/body"
  ["chimera-math"]="guts/math"
  ["chimera-language"]="guts/language"
  ["chimera-relationships"]="domains/relationships"
  ["chimera-basketball"]="domains/basketball"
  ["chimera-chess"]="domains/chess"
  ["chimera-music"]="domains/music"
  ["chimera-cooking"]="domains/cooking"
  ["chimera-ai"]="domains/ai"
  ["chimera-crypto"]="domains/crypto"
  ["chimera-stories"]="domains/stories"
  ["chimera-constellation"]="infrastructure/constellation"
  ["chimera-core"]="raw/core"
)

# Clone or pull each repo
for repo in "${!REPOS[@]}"; do
  target="${CHIMERA_ROOT}/${REPOS[$repo]}"
  if [ -d "${target}/.git" ]; then
    echo "Pulling ${repo}..."
    git -C "${target}" pull --quiet
  else
    echo "Cloning ${repo}..."
    git clone "git@github.com:${GH_USER}/${repo}.git" "${target}"
  fi
done

echo ""
echo "CHIMERA sync complete."
echo "Machine: ${MACHINE_NAME}"
echo "Total repos: ${#REPOS[@]}"
echo "Synced at: $(date)" >> "${CHIMERA_ROOT}/.last-sync"
echo "Machine: ${MACHINE_NAME}" >> "${CHIMERA_ROOT}/.last-sync"
```

---

## Cleanup Rules

```
~/chimera/ should ONLY contain:
  nucleus/
  guts/
  domains/
  infrastructure/
  raw/

NOTHING ELSE at the root level.

No stray folders.
No duplicate repos.
No leftover symlinks.
No ghost directories.

If something exists outside
this hierarchy, it either:
  1. Gets moved to its correct place
  2. Gets deleted

THE BODY HAS NO EXTRA ORGANS
FLOATING OUTSIDE IT.
```

---

## Bootstrap Protocol

```
NEW MACHINE:

1. Clone chimera-system FIRST
   git clone git@github.com:DrealR/chimera-system.git

2. Read THIS file
   cat architecture/folder-structure.md

3. Run the sync script from this file

4. Verify structure matches hierarchy above

5. Ready to work.

SYSTEM IS ALWAYS CLONED FIRST.
This doc tells you where
everything else goes.
DNA bootstraps the cell.
```

---

*One doc. One source of truth. Every machine reads it first. Every CC instance follows it. The architecture doc is the DNA that tells any new cell how to build the body.*
