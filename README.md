# Davood Tofighi - Academic Website

Personal academic website built with [Quarto](https://quarto.org).

**Live site:** [https://data-wise.github.io](https://data-wise.github.io)

## Structure

```
├── index.qmd         # Homepage
├── research.qmd      # Research interests
├── publications.qmd  # Publication list
├── software.qmd      # Software/packages
├── teaching.qmd      # Teaching info
├── _quarto.yml       # Site configuration
└── assets/           # Images, CV, etc.
```

## Local Development

```bash
# Preview
quarto preview

# Build
quarto render
```

## Deployment

Automatically deployed via GitHub Actions on push to `main`.

---

Part of the [Data-Wise](https://github.com/Data-Wise) ecosystem.
