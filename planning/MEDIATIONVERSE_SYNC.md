# MediationVerse Package Coordination

> **Coordinating releases and dependencies across 7 R packages**

---

## 📦 Package Overview

| Package | Version | CRAN | Dev Branch | Last Activity |
|---------|---------|------|------------|---------------|
| [mediationverse](https://github.com/Data-Wise/mediationverse) | 0.0.0.9000 | ❌ | `main` | 2025-12-09 (altdoc) |
| [medfit](https://github.com/Data-Wise/medfit) | 0.1.0.9000 | ❌ | `main` | 2025-12-04 (navbar) |
| [probmed](https://github.com/Data-Wise/probmed) | 0.0.0.9000 | ❌ | `main` | 2025-12-04 (pkgdown) |
| [rmediation](https://github.com/Data-Wise/rmediation) | 1.4.0 | ✅ | `main` | 2025-12-05 (docs) |
| [medrobust](https://github.com/Data-Wise/medrobust) | 0.1.0.9000 | ❌ | `main` | 2025-12-04 (pkgdown) |
| [medsim](https://github.com/Data-Wise/medsim) | 0.0.0.9000 | ❌ | `main` | 2025-12-04 (badges) |
| [missingmed](https://github.com/Data-Wise/missingmed) | — | ❌ | `scratch` | In development |

---

## 🔗 Dependency Graph

```
mediationverse (meta-package)
├── medfit (foundation)
│   ├── Used by: probmed, rmediation, medrobust, medsim, missingmed
├── probmed (P_med)
├── rmediation (CIs)  
├── medrobust (sensitivity)
├── medsim (simulation)
└── missingmed (missing data)
```

**Key Principle**: `medfit` changes require coordinated updates across all packages

---

## 🚀 Release Coordination

### Upcoming Releases

- **Next Release Window**: Q1 2025 (Jan-Mar 2025)
- **Target Packages**:
  - [ ] medfit - v0.1.0 (foundation - PRIORITY)
  - [ ] rmediation - v1.4.1 (update with medfit changes)

### Release Checklist (Per Package)

- [ ] All tests passing (`R CMD check --as-cran`)
- [ ] NEWS.md updated with changes
- [ ] Version bumped in DESCRIPTION
- [ ] README examples verified
- [ ] Vignettes render correctly
- [ ] Dependencies up-to-date
- [ ] CRAN comments addressed
- [ ] Tag created in GitHub
- [ ] Submit to CRAN

---

## ⚠️ Breaking Changes Protocol

### Before Making Breaking Changes

1. **Document** in `BREAKING_CHANGES.md`
2. **Notify** downstream package maintainers
3. **Coordinate** release timing
4. **Deprecate** gracefully (1-2 versions warning)
5. **Update** all examples and vignettes

### Current Breaking Changes in Pipeline

| Package | Change | Affects | Target Version | Status |
|---------|--------|---------|----------------|--------|
| | | | | |

---

## 🔄 S7 Migration Strategy

### Migration Order

1. **Phase 1**: `medfit` (foundation)
2. **Phase 2**: `probmed`, `rmediation` (depend on medfit)
3. **Phase 3**: `medrobust`, `medsim`, `missingmed`
4. **Phase 4**: `mediationverse` (meta-package update)

### Current Status

- [/] `medfit` - S7 migration in progress (v0.1.0.9000)
- [ ] `probmed` - Not started (waiting for medfit)
- [ ] `rmediation` - Not started (waiting for medfit)
- [ ] `medrobust` - Not started (waiting for medfit)
- [ ] `medsim` - Not started (waiting for medfit)
- [ ] `missingmed` - Not started (early development)
- [ ] `mediationverse` - Awaiting dependencies

---

## 📊 Quality Metrics

### Test Coverage

| Package | Coverage | Target |
|---------|----------|--------|
| medfit | | 80% |
| probmed | | 80% |
| rmediation | | 80% |
| medrobust | | 80% |
| medsim | | 80% |
| missingmed | | 80% |

### CRAN Check Status

Last checked: [Date]

- ✅ All packages passing
- ⚠️ Warnings: [List]
- ❌ Errors: [List]

---

## 🎯 Quarterly Goals

### Q1 2025

- [ ] Complete medfit S7 migration and CRAN submission
- [ ] Pilot altdoc on mediationverse (DONE ✅ 2025-12-09)
- [ ] Standardize pkgdown sites across all packages
- [ ] Run R CMD check --as-cran on all packages
- [ ] Prepare probmed and rmediation for Q2 submissions

---

## 📝 Meeting Notes

### [Date] - Sync Meeting

- **Attendees**:
- **Agenda**:
- **Decisions**:
- **Action Items**:
