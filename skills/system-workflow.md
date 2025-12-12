# System Workflow Skill

**Owner:** Stat-Wise (Statistics/Causal Inference Professor)  
**System:** macOS (Apple Silicon)  
**Updated:** December 12, 2025

---

## System Configuration

### Shell Environment
- **Shell:** Zsh with Antidote plugin manager + Powerlevel10k
- **Config location:** `~/.config/zsh/.zshrc` (NOT default ~/.zshrc)
- **Local bin:** `~/.local/bin` (custom scripts)

### Editor
- **Primary:** Emacs (`$EDITOR = emacsclient`)
- **Secondary:** VS Code (for workspaces)

### Key Tools
| Tool | Purpose |
|------|---------|
| `gh` | GitHub CLI |
| `git` | Version control |
| `R` / `Rscript` | Statistical computing |
| `tree` | Directory visualization |
| `rg` (ripgrep) | Fast search |
| `fd` | Fast find |
| `fzf` | Fuzzy finder |

---

## Project Structure

```
~/projects/
├── r-packages/                    # R PACKAGE ECOSYSTEM
│   ├── active/                    # 5 development packages
│   │   ├── medfit/               # Foundation (P0 priority)
│   │   ├── probmed/              # P_med effect size
│   │   ├── medrobust/            # Sensitivity analysis
│   │   ├── medsim/               # Simulation infrastructure
│   │   └── mediationverse/       # Meta-package
│   ├── stable/
│   │   └── rmediation/           # CRAN-ready (v1.4.0)
│   └── PROJECT-BOARD.md          # ADHD task board
│
├── dev-tools/                     # DEVELOPER TOOLS
│   └── data-wise/                # Project management hub
│       ├── planning/             # NOW.md, ROADMAP.md, PACKAGES.md
│       ├── bin/                  # medplan, medcheck scripts
│       └── skills/               # This file
│
└── research/
    └── mediation-planning/        # Technical coordination
        ├── API-CONTRACTS.md
        ├── DEVELOPMENT-STANDARDS.md
        ├── DEPENDENCY-MAP.md
        ├── ECOSYSTEM-COORDINATION.md
        └── SHELL-PROTOCOL.md
```

---

## MediationVerse Ecosystem

### Dependency Chain (Critical Path)
```
medfit (foundation) ──┬──→ probmed ────→ mediationverse
                      ├──→ rmediation ─→ mediationverse
                      ├──→ medrobust ──→ mediationverse
                      └──→ medsim ─────→ mediationverse
```

### Package Status
| Package | Version | Branch | Status |
|---------|---------|--------|--------|
| medfit | 0.1.0.9000 | dev | 🔴 P0 - Foundation |
| probmed | 0.0.0.9000 | main | 🟡 Awaiting medfit |
| rmediation | 1.4.0 | develop | ✅ CRAN-ready |
| medrobust | 0.1.0.9000 | claude/* | 🟡 In development |
| medsim | 0.0.0.9000 | main | 🟡 Framework ready |
| mediationverse | 0.0.0.9000 | main | 🟡 Shell only |

### S7 Classes (shared across ecosystem)
- `MediationData` — Simple mediation (X → M → Y)
- `SerialMediationData` — Serial mediation (X → M1 → M2 → Y)
- `BootstrapResult` — Bootstrap inference results
- `ProductNormal` — Product of normals distribution (RMediation)
- `PmedResult` — P_med effect size (probmed)

---

## Custom Commands

### medplan — Planning Navigation
```bash
medplan           # Quick status overview
medplan board     # Open PROJECT-BOARD.md
medplan now       # Open NOW.md (current focus)
medplan tech      # Open technical docs folder
medplan github    # Open GitHub Projects board
medplan all       # Open everything
medplan sync      # Push mediation-planning to GitHub
```

### medcheck — Ecosystem Health Monitor
```bash
medcheck          # Quick health status (default)
medcheck status   # Same as above
medcheck deps     # Check dependency consistency
medcheck versions # Show all package versions
medcheck git      # Git status across all repos
medcheck tests    # Run tests across ecosystem
medcheck full     # All checks combined
```

---

## Shell Execution Protocol

### Pre-Action Statement
Before any action, state:
- **What:** Action in plain language
- **Why:** Purpose/benefit
- **Affected:** Files/folders with paths
- **Risk:** 🟢 Read | 🟡 Modify | 🔴 Destructive
- **Est:** Time estimate

### Confirmation
| Input | Action |
|-------|--------|
| `1` | Proceed with this action |
| `2` | Proceed and show full results |
| `3` | Accept all similar actions (batch) |
| `0` | Skip/abort |

### Auto-Execute Rules
- 🟢 **Read-only:** Auto-execute (no confirmation)
- 🟡 **Modify:** Confirm with 1/2/3/0
- 🔴 **Destructive:** Always confirm, note rollback

### Progress Tracking
- Multi-step: `[Step 2/5]` or `[2/5 ✓]`
- After 3+ actions: summarize completed work
- Stopping points: `⏸️ Good place to pause`

---

## R Package Development Aliases

```bash
# Navigation
cd ~/projects/r-packages/active/medfit  # or use: cdrpkg medfit

# Development cycle
rload        # devtools::load_all()
rdoc         # devtools::document()
rtest        # devtools::test()
rcheck       # devtools::check()
rdev         # document + test + check (full cycle)

# Specific tests
rtest1 "pattern"    # Run tests matching pattern

# Git workflow
rpkgcommit "msg"    # Document + test + commit

# Package creation
rnewfun name        # Create R/name.R
rnewtest name       # Create tests/testthat/test-name.R
```

---

## GitHub Organization

- **Organization:** Data-Wise
- **Projects Board:** https://github.com/users/Data-Wise/projects/1
- **Repos:** 30 total (7 R packages, 8 dev tools, 15 other)

### Key Repos
| Repo | Purpose |
|------|---------|
| medfit | Foundation R package |
| probmed | P_med effect size |
| rmediation | CIs for mediation (CRAN) |
| medrobust | Sensitivity analysis |
| medsim | Simulation infrastructure |
| mediationverse | Meta-package |
| mediation-planning | Technical coordination docs |
| data-wise | Project management hub |

---

## Response Preferences

### Default Tools
- **Statistics:** R (tidyverse, ggdag)
- **Documents:** Quarto
- **Math:** LaTeX notation always

### Response Level
- **Expert/Concise** — No basic explanations
- Use VanderWeele notation for mediation

### Modes
| Mode | Focus |
|------|-------|
| `[Refine]` | Rewrite input as detailed prompt, don't answer |
| `[Researcher]` | Asymptotics, proofs, formal tone |
| `[Coder]` | R package dev, show Python equivalent |
| `[Teacher]` | Graduate-level, DAG-first pedagogy |
| `[Personal]` | Casual, home/travel/ABQ topics |

---

## ADHD Workflow Support

### Task Management
- Break multi-step into numbered checklist
- End responses with **Next: [specific action]**
- Include time estimates (~5 min, ~30 min)
- Flag context switches: ⚠️

### Decision Support
- Provide default recommendation
- Limit to 2-3 options with comparison
- Low-stakes: "Either works — I'd default to X"
- High-stakes: "Important choice — affects Y"

### Progress Visibility
- Step counters: `[Step 2/5 ✓]`
- Celebrate completions: ✅ **Done!**
- Summarize after 3+ decisions

### Session Continuity
- Track files modified
- Offer session summaries at natural endpoints
- Search past conversations when context referenced

---

## Quick Reference Card

```
CONFIRM:   1=proceed | 2=show | 3=batch | 0=skip
RISK:      🟢=read   | 🟡=modify | 🔴=destructive
PROGRESS:  [X/Y ✓]
COMMANDS:  medplan | medcheck | rdev | rpkgcommit
ZSHRC:     ~/.config/zsh/.zshrc
PACKAGES:  ~/projects/r-packages/active/
PLANNING:  ~/projects/research/mediation-planning/
```
