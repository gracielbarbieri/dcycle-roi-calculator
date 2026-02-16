# Dcycle ROI Calculator

Interactive ROI calculator that helps companies estimate their annual savings by adopting [Dcycle](https://www.dcycle.io) ESG solutions.

![Dcycle](https://albaselvaortiz.github.io/dcycle-landing/logo_dcycle.png)

## Live Demo

Deploy to GitHub Pages and access at `https://<username>.github.io/dcycle-roi-calculator/`

## Features

### Savings Blocks
- **Consultancy Savings** - Calculate cost savings from replacing external ESG consultancy with Dcycle. Shows per-solution percentage reduction, hours saved, consultancy cost/hour, and total savings.
- **Internal Team Efficiency** - Estimate salary savings from reducing internal ESG workload. Auto-calculates "with Dcycle" hours from industry benchmarks and selected solutions. Shows time reduction %, fully loaded cost/hour, and total internal savings.

### Solutions & Data
- **6 Dcycle Solutions**: Climate Change (GHG), Ecovadis, Life Cycle Analysis (LCA), ISOs, Procurement / Supply Chain, EINF
- **11 Industry Benchmarks**: Based on real Dcycle client data - Food & Beverage, Healthcare, Industrial, Logistics, Chemical, Retail, Energy, Construction, Tech, Finance, and Other
- **17 Countries**: Pre-configured with local employer overhead rates and working hours (EU, UK, US, Switzerland, Scandinavia)
- **8 Currencies**: EUR, GBP, USD, CHF, SEK, NOK, DKK, HUF (auto-set by country, manually overridable)

### Internationalization
- **7 Languages**: English, Spanish, French, German, Italian, Portuguese, Dutch
- Full i18n system with ~80 translation keys per language
- Auto-switches language on country selection

### Output
- **Real-time ROI calculation** with total annual savings breakdown
- **PDF Report Generation** - Branded A4 PDF with lead capture form (name, company, email)
- **Fully Responsive** - Works on desktop, tablet, and mobile

## Tech Stack

- **Single HTML file** - No build tools, no frameworks, no dependencies to install
- Vanilla JavaScript with `data-i18n` attribute-based translation engine
- CSS custom properties for Dcycle design system (`--dc-blue: #2947FE`, Inter font)
- [jsPDF 2.5.1](https://github.com/parallax/jsPDF) + [jspdf-autotable 3.8.2](https://github.com/simonbengtsson/jsPDF-AutoTable) via CDN for PDF generation
- [Inter](https://fonts.google.com/specimen/Inter) font via Google Fonts

## Quick Start

### Option 1: Open directly
Simply open `index.html` in any modern browser.

### Option 2: Local server
```bash
# Python 3
python3 -m http.server 8080

# Node.js (npx)
npx serve .
```
Then visit `http://localhost:8080`

### Option 3: GitHub Pages
1. Push this repo to GitHub
2. Go to **Settings > Pages**
3. Set source to `main` branch, root folder (`/`)
4. Your calculator will be live at `https://<username>.github.io/dcycle-roi-calculator/`

## How It Works

1. **Select your country** - Auto-sets currency, language, overhead rate, and working hours
2. **Choose your industry** - Loads real benchmark data for ESG task hours
3. **Pick Dcycle solutions** - Check the solutions relevant to your company (both blocks show % reduction per solution)
4. **Adjust inputs** - Fine-tune hourly rates, team size, salaries
5. **See your ROI** - Instant calculation of annual savings
6. **Download PDF** - Fill in your details and get a branded report to share with your team

## Project Structure

```
dcycle-roi-calculator/
  index.html    # Complete single-file application (HTML + CSS + JS)
  README.md     # This file
  LICENSE       # MIT License
  .gitignore    # Git ignore rules
```

## License

MIT License - See [LICENSE](LICENSE) for details.

---

Built for [Dcycle](https://www.dcycle.io)
