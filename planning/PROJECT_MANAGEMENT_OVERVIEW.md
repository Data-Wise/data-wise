# Data-Wise Project Management

> **Central coordination hub for the Data-Wise ecosystem**

---

## 🎯 Purpose

This `planning/` folder serves as the central project management hub for coordinating development across **20+ Data-Wise repositories** organized in a 5-layer architecture.

---

## 📁 Planning Structure

### Recommended Documents

#### **1. Roadmaps & Vision**

- `ECOSYSTEM_ROADMAP.md` - High-level multi-year strategic vision
- `QUARTERLY_GOALS.md` - 3-month objectives per layer
- `RELEASE_CALENDAR.md` - Coordinated release schedule across packages

#### **2. Active Project Tracking**

- `ACTIVE_PROJECTS.md` - Currently in-progress initiatives
- `PROJECT_STATUS.md` - Weekly status dashboard
- `BLOCKERS.md` - Cross-repo blockers and dependencies

#### **3. Architecture & Standards**

- `ARCHITECTURE_DECISIONS.md` - ADRs (Architecture Decision Records)
- `STANDARDS_CHANGELOG.md` - Changes to ecosystem-wide standards
- `DEPENDENCY_MAP.md` - Inter-package dependency visualization

#### **4. R Package Coordination**

- `MEDIATIONVERSE_SYNC.md` - Coordinating the 7 MediationVerse packages
- `CRAN_SUBMISSION_TRACKER.md` - CRAN submission status/timeline
- `BREAKING_CHANGES.md` - Coordinating breaking changes across packages

#### **5. AI Engine Development**

- `AI_PARITY_TRACKER.md` - Feature parity between Claude/Gemini tools
- `MCP_ROADMAP.md` - MCP server development plans
- `KNOWLEDGE_BASE_SYNC.md` - Keeping `.gemini/` and `.claude/` aligned

#### **6. Documentation Strategy**

- `DOCS_MIGRATION_PLAN.md` - MkDocs/pkgdown migration status
- `WEBSITE_ROADMAP.md` - GitHub Pages strategy
- `STYLE_GUIDE.md` - Documentation standards

#### **7. Community & Onboarding**

- `CONTRIBUTOR_GUIDE.md` - How to contribute to Data-Wise
- `ONBOARDING_CHECKLIST.md` - New developer setup
- `FAQ.md` - Common questions

---

## 🔄 Suggested Workflow

### Weekly Cycle

```
Monday    → Review ACTIVE_PROJECTS.md, update status
Wednesday → Check BLOCKERS.md, coordinate solutions  
Friday    → Update PROJECT_STATUS.md, plan next week
```

### Monthly Cycle

```
Week 1 → CRAN submission coordination
Week 2 → Architecture review (ADRs)
Week 3 → Documentation sprint
Week 4 → AI engine feature parity check
```

### Quarterly Cycle

```
Q1 → Review ECOSYSTEM_ROADMAP.md
Q2 → Update QUARTERLY_GOALS.md
Q3 → Plan RELEASE_CALENDAR.md
Q4 → Year-end retrospective
```

---

## 🎨 Layer-Specific Priorities

### Standards Layer

- Maintain `docs-standards` configs
- Coordinate MkDocs Material theme updates
- Standardize GitHub Actions workflows

### IDE Layer  

- `emacs-r-devkit` feature development
- Integration with AI engines
- User experience improvements

### AI Engines Layer

- **Claude**: `claude-r-dev` enhancements
- **Gemini**: `r-package-dev-gemini` parity
- **MCP**: Statistical research server expansion

### R Packages Layer

- **MediationVerse**: Coordinated 7-package releases
- CRAN compliance across all packages
- S7 OOP migration strategy
- Cross-package integration testing

### Applications Layer

- `examark` feature development
- User feedback integration
- Production deployment strategy

---

## 📊 Metrics to Track

- [ ] **Package Health**: CRAN check status, test coverage
- [ ] **Documentation Coverage**: % pages with examples
- [ ] **AI Parity**: Feature count Claude vs Gemini
- [ ] **Dependencies**: Circular dependency detection
- [ ] **Release Cadence**: Packages released per quarter
- [ ] **Blockers**: Average resolution time
- [ ] **Standards Compliance**: % repos following standards

---

## 🔗 Integration Points

### GitHub Integration

- Project boards for each layer
- Milestone tracking across repos
- Issue templates standardized

### Automation Opportunities

- Daily automated check: R CMD check all packages
- Weekly digest: PR summary across repos
- Monthly report: Ecosystem health dashboard

---

## 🚀 Getting Started

1. **Immediate**: Create `ACTIVE_PROJECTS.md` with current work
2. **This Week**: Draft `QUARTERLY_GOALS.md` for Q1 2025
3. **This Month**: Establish `MEDIATIONVERSE_SYNC.md` coordination
4. **This Quarter**: Complete `ECOSYSTEM_ROADMAP.md` vision

---

**Questions to Consider:**

- Which planning documents are most urgent for your current workflow?
- Should planning files be version-controlled or kept local?
- Do you want integration with external tools (Notion, Jira, etc.)?
- How granular should project tracking be (package-level vs feature-level)?
