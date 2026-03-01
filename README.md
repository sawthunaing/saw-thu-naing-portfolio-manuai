# Saw Thu Naing — Portfolio Website

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/sawthunaing/portfolio)
[![.NET](https://img.shields.io/badge/.NET-8.0-512BD4?logo=dotnet)](https://dotnet.microsoft.com/)
[![Blazor](https://img.shields.io/badge/Blazor-WebAssembly-512BD4?logo=blazor)](https://blazor.net/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> Personal portfolio website for **Saw Thu Naing** — Senior Full-Stack .NET Developer with 10+ years of experience in FinTech and streaming systems.

## Live Demo

🌐 **[sawthunaing.vercel.app](https://sawthunaing.vercel.app)**

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | Blazor WebAssembly (.NET 8) |
| Language | C# |
| Styling | Custom CSS (Dark Minimal Theme) |
| Icons | Font Awesome 6 + Devicons |
| Fonts | JetBrains Mono + Inter |
| Deployment | Vercel (Static Hosting) |
| CI/CD | GitHub Actions |

## Features

- **Hero Section** — Animated typing effect, tech stack icons, GitHub link
- **About** — Professional summary, stats, education, certifications
- **Experience** — Interactive timeline of 5+ roles across FinTech & streaming
- **Projects** — Grid of 6 featured projects with tech tags
- **Skills Matrix** — Proficiency bars across 4 categories + tech tag cloud
- **Blog/Writing** — 6 technical article cards
- **Contact Form** — Functional contact form with social links
- **Dark Minimal Theme** — Black (#0a0a0a), Neon Green (#39ff14), Slate Gray (#64748b)

## Getting Started

### Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)

### Run Locally

```bash
git clone https://github.com/sawthunaing/portfolio.git
cd portfolio/SawThuNaingPortfolio
dotnet restore
dotnet run
```

Open [https://localhost:5001](https://localhost:5001) in your browser.

### Build for Production

```bash
cd SawThuNaingPortfolio
dotnet publish -c Release -o ../publish
```

The static files will be in `publish/wwwroot/`.

## Deploy to Vercel

### Option 1: One-Click Deploy

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/sawthunaing/portfolio)

### Option 2: Manual Setup

1. Fork this repository
2. Connect to [Vercel](https://vercel.com)
3. Set build command: `cd SawThuNaingPortfolio && dotnet publish -c Release -o ../publish`
4. Set output directory: `publish/wwwroot`
5. Deploy!

### Option 3: GitHub Actions CI/CD

Add these secrets to your GitHub repository:

| Secret | Description |
|--------|-------------|
| `VERCEL_TOKEN` | Your Vercel API token |
| `VERCEL_ORG_ID` | Your Vercel organization ID |
| `VERCEL_PROJECT_ID` | Your Vercel project ID |

Every push to `main` will automatically deploy to Vercel.

## Project Structure

```
portfolio/
├── SawThuNaingPortfolio/
│   ├── Pages/
│   │   └── Home.razor          # Main portfolio page (all sections)
│   ├── Layout/
│   │   └── MainLayout.razor    # Navigation + footer layout
│   ├── wwwroot/
│   │   ├── css/
│   │   │   └── app.css         # Dark minimal theme styles
│   │   └── index.html          # Entry point with JS utilities
│   ├── App.razor               # Router configuration
│   ├── _Imports.razor          # Global using statements
│   └── Program.cs              # App entry point
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions CI/CD
├── vercel.json                 # Vercel deployment config
└── README.md
```

## Color Palette

| Color | Hex | Usage |
|-------|-----|-------|
| Background | `#0a0a0a` | Primary background |
| Surface | `#111111` | Secondary background |
| Card | `#161616` | Card backgrounds |
| Neon Green | `#39ff14` | Accent, highlights |
| Slate Gray | `#64748b` | Secondary text |
| Text Primary | `#e2e8f0` | Main text |

## Contact

- **Email:** sawthunaing@gmail.com
- **LinkedIn:** [linkedin.com/in/sawthunaing](https://linkedin.com/in/sawthunaing)
- **GitHub:** [github.com/sawthunaing](https://github.com/sawthunaing)
- **Phone:** +44 7405 473363

---

Built with ❤️ using **Blazor WebAssembly** and **C#**
