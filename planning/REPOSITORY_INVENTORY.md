# Data-Wise Complete Ecosystem Inventory (Local + GitHub)

**Last Updated**: 2025-12-10

---

## 📊 Overview

### GitHub Status

- **On GitHub**: 14 repositories
- **Missing from GitHub**: 6 repositories (all in `dev-tools`)
- **Total Ecosystem Size**: **20 repositories**

### R Packages

- **Active Development** (`~/projects/r-packages/active/`): 6 packages
- **On CRAN**: 1 package (rmediation)
- **Scratch** (`~/projects/r-packages/scratch/`): 1 package structure
- **Archive**: Empty

---

## 🗂️ Complete Repository List

### Layer 1: Standards

| Repository | Location | GitHub | Status |
|------------|----------|--------|--------|
| docs-standards | `dev-tools/` | ✅ [Public](https://github.com/Data-Wise/docs-standards) | Active |

---

### Layer 2: IDE

| Repository | Location | GitHub | Status |
|------------|----------|--------|--------|
| emacs-r-devkit | `dev-tools/` | ✅ [Public](https://github.com/Data-Wise/emacs-r-devkit) | Active |

---

### Layer 3: AI Engines & Workflows

| Repository | Location | GitHub | Status | Notes |
|------------|----------|--------|--------|-------|
| claude-r-dev | `dev-tools/` | ✅ [Public](https://github.com/Data-Wise/claude-r-dev) | Active | MkDocs site |
| r-package-dev-gemini | `dev-tools/` | ✅ [Public](https://github.com/Data-Wise/r-package-dev-gemini) | Active | 20 commands |
| **claude-statistical-research** | `dev-tools/` | ❌ **LOCAL ONLY** | Active | **MCP server! Needs GitHub** |
| zsh-claude-workflow | `dev-tools/` | ❌ **LOCAL ONLY** | Active | Shell automation |
| obsidian-cli-ops | `dev-tools/` | ❌ **LOCAL ONLY** | Active | Obsidian integration |

**FOUND**: `claude-statistical-research` exists locally with MCP server!

---

### Layer 4: R Packages (MediationVerse)

| Package | Location | GitHub | CRAN | Status |
|---------|----------|--------|------|--------|
| mediationverse | `r-packages/active/` | ✅ [Public](https://github.com/Data-Wise/mediationverse) | ❌ | Meta-package |
| medfit | `r-packages/active/` | ✅ [Public](https://github.com/Data-Wise/medfit) | ❌ | Foundation (S7) |
| probmed | `r-packages/active/` | ✅ [Public](https://github.com/Data-Wise/probmed) | ❌ | P_med effect sizes |
| rmediation | `r-packages/active/` | ✅ [Public](https://github.com/Data-Wise/rmediation) | ✅ | Confidence intervals |
| medrobust | `r-packages/active/` | ✅ [Public](https://github.com/Data-Wise/medrobust) | ❌ | Sensitivity analysis |
| medsim | `r-packages/active/` | ✅ [Public](https://github.com/Data-Wise/medsim) | ❌ | Simulation |
| missingmed | `r-packages/scratch/` | ✅ [Public](https://github.com/Data-Wise/missingmed) | ❌ | Early development |
| mbco | (unknown location) | ✅ [Public](https://github.com/Data-Wise/mbco) | N/A | Research archive |

**Note**: All active R packages are in `~/projects/r-packages/active/`

---

### Layer 5: Applications & Tools

| Repository | Location | GitHub | Status | Notes |
|------------|----------|--------|--------|-------|
| examark | (unknown location) | ✅ [Public](https://github.com/Data-Wise/examark) | Active | Canvas QTI converter |
| unm-revealjs | (unknown location) | ✅ [Public](https://github.com/Data-Wise/unm-revealjs) | Active | Quarto extension |
| **homebrew-tap** | `dev-tools/` | ❌ **LOCAL ONLY** | Active | Formula repository |
| **workspace-auditor** | `dev-tools/` | ❌ **LOCAL ONLY** | Active | Dev tool |

---

## 🚨 Repositories Missing from GitHub (6)

### HIGH PRIORITY - Should Push to GitHub

1. **claude-statistical-research** (`dev-tools/`)
   - Contains MCP server (mentioned in Data-Wise README!)
   - Solves the "missing MCP server" mystery
   - **Action**: Push to `Data-Wise/claude-statistical-research-mcp`

2. **zsh-claude-workflow** (`dev-tools/`)
   - Shell-based Claude automation
   - Complements `claude-r-dev`
   - **Action**: Push to `Data-Wise/zsh-claude-workflow`

3. **obsidian-cli-ops** (`dev-tools/`)
   - Your 3-Vault Obsidian system integration
   - Mentioned in your user rules/memories
   - **Action**: Push to `Data-Wise/obsidian-cli-ops`

### MEDIUM PRIORITY

4. **homebrew-tap** (`dev-tools/`)
   - Contains Homebrew formulas (likely for Data-Wise tools)
   - Useful for macOS installation
   - **Action**: Push to `Data-Wise/homebrew-tap`

5. **workspace-auditor** (`dev-tools/`)
   - Development utility
   - **Action**: Evaluate if this should be public

6. **data-wise** (`dev-tools/`)
   - The super project itself!
   - **Action**: Already exists, but ensure `planning/` is committed

---

## 📂 Directory Structure Summary

```
~/projects/
├── dev-tools/          (10 projects)
│   ├── claude-r-dev               ✅ GitHub
│   ├── claude-statistical-research ❌ LOCAL ONLY (MCP!)
│   ├── data-wise                   ✅ GitHub
│   ├── docs-standards              ✅ GitHub
│   ├── emacs-r-devkit             ✅ GitHub
│   ├── homebrew-tap                ❌ LOCAL ONLY
│   ├── obsidian-cli-ops            ❌ LOCAL ONLY
│   ├── r-package-dev-gemini        ✅ GitHub
│   ├── workspace-auditor           ❌ LOCAL ONLY
│   └── zsh-claude-workflow         ❌ LOCAL ONLY
│
└── r-packages/
    ├── active/          (6 packages - all on GitHub)
    │   ├── medfit
    │   ├── mediationverse
    │   ├── medrobust
    │   ├── medsim
    │   ├── probmed
    │   └── rmediation
    ├── archive/         (empty)
    ├── scratch/         (missingmed structure)
    └── selected         (not a directory)
```

---

## 🎯 Updated Ecosystem Totals

- **Total Repositories**: 20 (14 on GitHub + 6 local only)
- **Dev Tools**: 10 total (4 on GitHub + 6 local)
- **R Packages**: 8 total (8 on GitHub, 6 actively developed locally)
- **Applications**: 2 (2 on GitHub)
- **Standards**: 1 (1 on GitHub)

---

## 📋 Immediate Actions Required

### 1. Push Missing Repositories to GitHub ⭐ URGENT

**Claude Statistical Research MCP**

```bash
cd ~/projects/dev-tools/claude-statistical-research
git init
git add .
git commit -m "Initial commit: Claude statistical research MCP server"
gh repo create Data-Wise/claude-statistical-research-mcp --public --source=. --push
```

**Other Tools** (similar process for):

- `zsh-claude-workflow` → `Data-Wise/zsh-claude-workflow`
- `obsidian-cli-ops` → `Data-Wise/obsidian-cli-ops`
- `homebrew-tap` → `Data-Wise/homebrew-tap`
- `workspace-auditor` → `Data-Wise/workspace-auditor`

### 2. Update Data-Wise README

Current README shows 20 repos badge but only lists 14. Update to reflect:

- **Dev Tools**: 10 repos
- **R Packages**: 8 repos
- **Total**: 20 repos

### 3. Organize Project Structure

**Decision Needed**: Should applications like `examark` and `unm-revealjs` be moved to `dev-tools` or stay separate?

---

## 🔍 Key Discoveries

1. ✅ **Found the MCP Server!** `claude-statistical-research` exists locally
2. ✅ **Active R Package Development**: All 6 packages in `r-packages/active/`
3. ✅ **More AI Tools**: `zsh-claude-workflow` and `obsidian-cli-ops`
4. ⚠️  **6 repos not yet on GitHub** - missing from public ecosystem
5. 📊 **Actual ecosystem is 30% larger** than GitHub suggests (20 vs 14 repos)

---

## Next Steps

1. **Review this inventory** - confirm all projects identified
2. **Decide which repos should be public** vs private
3. **Push critical repos** (especially MCP server)
4. **Update planning documents** with complete 20-repo ecosystem
5. **Determine missing repo locations** (examark, unm-revealjs, mbco)
