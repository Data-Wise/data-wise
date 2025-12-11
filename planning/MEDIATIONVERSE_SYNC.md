# MediationVerse Package Coordination

> **Coordinating releases and dependencies across 7 R packages**

---

## 📦 Package Overview

| Package | Version | CRAN | Dev Branch | Last Release |
|---------|---------|------|------------|--------------|
| [mediationverse](https://github.com/Data-Wise/mediationverse) | | | `main` | |
| [medfit](https://github.com/Data-Wise/medfit) | | | `main` | |
| [probmed](https://github.com/Data-Wise/probmed) | | | `main` | |
| [rmediation](https://github.com/Data-Wise/rmediation) | | | `main` | |
| [medrobust](https://github.com/Data-Wise/medrobust) | | | `main` | |
| [medsim](https://github.com/Data-Wise/medsim) | | | `main` | |
| [missingmed](https://github.com/Data-Wise/missingmed) | | | `main` | |

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

- **Next Release Window**: [Date Range]
- **Target Packages**:
  - [ ] Package 1 - v0.x.0
  - [ ] Package 2 - v0.x.0

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

- [ ] `medfit` - S7 migration complete
- [ ] `probmed` - Not started
- [ ] `rmediation` - Not started
- [ ] `medrobust` - Not started  
- [ ] `medsim` - Not started
- [ ] `missingmed` - Not started
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

- [ ] Goal 1
- [ ] Goal 2
- [ ] Goal 3

---

## 📝 Meeting Notes

### [Date] - Sync Meeting

- **Attendees**:
- **Agenda**:
- **Decisions**:
- **Action Items**:
