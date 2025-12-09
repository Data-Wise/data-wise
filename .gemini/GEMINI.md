# Data-Wise Gemini Knowledge Base

## Context

You are working in the Data-Wise ecosystem - tools for statistical research and mediation analysis.

## Key Projects

### Development Tools

- **emacs-r-devkit**: Emacs environment for R (macOS)
- **r-package-dev-gemini**: Gemini CLI extension for R

### R Packages (MediationVerse)

- **mediationverse**: Meta-package hub
- **medfit**: Infrastructure foundation
- **probmed**: P_med effect sizes
- **rmediation**: Confidence intervals
- **medrobust**: Sensitivity analysis
- **medsim**: Simulation

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
- pkgdown for R packages (Academic Blue #0054AD)
- See docs-standards repo for configs
