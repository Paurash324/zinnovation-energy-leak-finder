# Energy Leak Finder

A lightweight single-page web app that helps users estimate household appliance energy usage and identify the biggest sources of electricity consumption.

## Overview

Energy Leak Finder is built as a fast, dependency-free browser experience using plain HTML, CSS, and JavaScript. Add your appliances, enter their power ratings and usage hours, then calculate an estimated energy profile.

## Features

- Add and remove appliance rows dynamically
- Estimate appliance energy usage from wattage and daily runtime
- Sort results to surface the biggest energy leaks
- Visualize relative consumption with animated bars
- Dark, responsive interface for desktop and mobile screens
- Optional AI-generated energy-saving tips through a Groq API key
- No build step or package installation required

## Getting started

### Run locally

1. Clone the repository:

   ```bash
   git clone https://github.com/Paurash324/zinnovation-energy-leak-finder.git
   cd zinnovation-energy-leak-finder
   ```

2. Open `index.html` directly in a browser.

   For a local development server, use any static server, for example:

   ```bash
   python -m http.server 8000
   ```

3. Visit `http://localhost:8000`.

## How it works

1. Enter your electricity rate and billing preferences.
2. Add appliances and provide their wattage and average daily usage.
3. Select **Find my leaks** to calculate estimated consumption.
4. Review the ranked results and focus on the highest-impact appliances first.

The core calculator runs entirely in the browser. No data is sent to a backend for the standard calculation flow.

## Project structure

```text
.
├── index.html    # Complete application: markup, styles, and JavaScript
├── README.md     # Project documentation
└── .gitignore    # Local/editor files excluded from version control
```

## Customization

The app is intentionally self-contained. You can customize it by editing `index.html`:

- Update colors and typography in the CSS variables near the top of the file.
- Change the default appliance rows in the HTML.
- Adjust calculation or sorting behavior in the JavaScript section.
- Replace the optional AI tip integration with another provider or remove it.

## Deployment

Because this is a static site, it can be deployed to GitHub Pages, Netlify, Vercel, Cloudflare Pages, or any static hosting provider. Point the host at the repository root and use `index.html` as the entry file.

## Accessibility and privacy

The calculator is designed to work without an account or server. Avoid committing API keys or other secrets to the repository. If you use the optional AI feature, configure keys through a local development workflow rather than hard-coding them into `index.html`.

## License

No open-source license has been selected yet. Until a license is added, all rights are reserved by the copyright holder.
