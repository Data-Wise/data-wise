# 📦 Packages

> **MediationVerse R Package Status**

---

## Active Packages

| Package | Version | CRAN | Last Push | Status |
|---------|---------|------|-----------|--------|
| [mediationverse](https://github.com/Data-Wise/mediationverse) | dev | ❌ | Dec 10 | 🟢 altdoc complete |
| [medfit](https://github.com/Data-Wise/medfit) | dev | ❌ | Dec 4 | 🔴 S7 migration needed |
| [probmed](https://github.com/Data-Wise/probmed) | dev | ❌ | Dec 4 | 🟡 Awaiting medfit |
| [rmediation](https://github.com/Data-Wise/rmediation) | 1.4.0 | ✅ | Dec 5 | ✅ Stable |
| [medrobust](https://github.com/Data-Wise/medrobust) | dev | ❌ | Dec 4 | 🟡 Awaiting medfit |
| [medsim](https://github.com/Data-Wise/medsim) | dev | ❌ | Dec 4 | 🟡 Awaiting medfit |
| [missingmed](https://github.com/Data-Wise/missingmed) | early | ❌ | Nov 17 | 🔵 Early development |

**Legend**: 🔴 Blocked/Priority | 🟡 Waiting | 🟢 Active | ✅ Complete | 🔵 Future

---

## Dependency Chain

```
medfit (foundation) ← PRIORITY
   ↓
probmed, rmediation, medrobust, medsim
   ↓
missingmed
   ↓
mediationverse (meta-package)
```

**Key**: medfit changes require updates across all packages

---

## CRAN Submission Queue

| # | Package | Target | Blocker |
|---|---------|--------|---------|
| 1 | medfit | Q1 2025 | S7 migration |
| 2 | probmed | Q2 2025 | medfit release |
| 3 | rmediation | Q2 2025 | medfit changes |
| 4 | medrobust | Q3 2025 | - |
| 5 | medsim | Q3 2025 | - |

---

## Archive

| Package | Status | Notes |
|---------|--------|-------|
| [mbco](https://github.com/Data-Wise/mbco) | 📦 Archived | Research archive (2019) |
