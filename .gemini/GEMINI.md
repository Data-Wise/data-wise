# Data-Wise Gemini Knowledge Base

## Context

You are working in the Data-Wise ecosystem - tools for statistical research and mediation analysis.

## Key Projects

### Development Tools

- **emacs-r-devkit**: Emacs environment for R (macOS)
- **r-package-dev-gemini**: Gemini CLI extension for R (20 commands)
- **claude-r-dev**: Claude Code extension for R workflows
- **claude-statistical-research-mcp**: MCP server for statistical research
- **zsh-claude-workflow**: Shell automation for Claude
- **obsidian-cli-ops**: 3-vault Obsidian integration
- **homebrew-tap**: Homebrew formulas for Data-Wise tools

### R Packages (MediationVerse)

- **mediationverse**: Meta-package hub
- **medfit**: Infrastructure foundation  
- **probmed**: P_med effect sizes
- **rmediation**: Confidence intervals (on CRAN)
- **medrobust**: Sensitivity analysis
- **medsim**: Simulation
- **missingmed**: Missing data
- **mbco**: MBCO research archive

## R Package Standards

- S7 OOP for new code
- checkmate for input validation
- testthat edition 3 for tests
- roxygen2 for documentation
- CRAN submission standards

## Commands

When checking packages: `R CMD check --no-manual --as-cran`
Before push: `R CMD check --as-cran`

## Documentation

- MkDocs for tools
- pkgdown/altdoc for R packages (Academic Blue #0054AD)
- See docs-standards repo for configs

## Planning

- GitHub Projects: [Ecosystem Roadmap](https://github.com/users/Data-Wise/projects/1)
- Planning docs in `data-wise/planning/` folder
- ACTIVE_PROJECTS.md tracks current work
- MEDIATIONVERSE_SYNC.md coordinates R package releases
