# Personal Academic Website Knowledge

## SKILL.md - Claude Skill for Website Development

### Purpose
Development and maintenance of Davood Tofighi's personal academic website at data-wise.github.io

### Site Details
- **URL**: https://data-wise.github.io
- **Platform**: Quarto
- **Theme**: Warm Academic (custom SCSS)
- **Repo**: github.com/Data-Wise/data-wise.github.io
- **Local**: ~/projects/dev-tools/data-wise.github.io

### Owner
- **Name**: Davood Tofighi, Ph.D.
- **Title**: Associate Professor, Department of Mathematics & Statistics
- **Institution**: University of New Mexico
- **Office**: SMLC 228
- **Email**: dtofighi@unm.edu (JS-protected on site)

### Profile Links
- Google Scholar: user=hzQ60YcAAAAJ
- ORCID: 0000-0001-8523-7776
- GitHub: Data-Wise
- LinkedIn: davood-tofighi-b6176ab8
- UNM: math.unm.edu/people/academic-personnel/davood-tofighi

### Color Palette
```
cream:       #faf8f5  (background)
dark-brown:  #78350f  (header/footer)
amber:       #b45309  (primary/links)
gold:        #d97706  (accent/logo)
warm-gray:   #3d3d3d  (text)
light-cream: #f5f0eb  (subtle bg)
tan:         #d4a373  (borders)
```

### Typography
- Headings: Playfair Display, Georgia, serif
- Body: Source Sans Pro, system fonts

### File Structure
```
_quarto.yml           - Site config
warm-academic.scss    - Theme styles
index.qmd             - Homepage
research.qmd          - Research
publications.qmd      - Publications
software.qmd          - Software/mediationverse
teaching.qmd          - Teaching
assets/
  logo-placeholder.svg
  profile-placeholder.svg
```

### Key Features
- Layout 1: Logo header + compact bio (80px photo)
- Email: JS obfuscation (u + '@' + d pattern)
- Auto-deploy: GitHub Actions on push
- Dark mode: Supported

### Commands
```bash
quarto preview          # Local dev
quarto render           # Build
git push                # Deploy (auto)
```

### Placeholders to Replace
- assets/profile-placeholder.svg → profile.jpg
- profile.jpg or profile.png (your actual photo)
- assets/logo-placeholder.svg → real logo
- publications.qmd → full publication list

### Research Areas
- Causal inference, DAG-based mediation analysis
- Sensitivity analysis (statistical, Monte Carlo)
- GLMMs, multivariate statistics
- ML in health data
- Drug delivery optimization

### Professional
- Associate Editor: Frontiers in Psychology
- Funding: NASA, NSF, NIH
