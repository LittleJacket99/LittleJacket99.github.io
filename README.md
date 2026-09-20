# ED Hotspots Finder - Rings & Planets + EDMC Plugin Website

Official GitHub Pages site for the **ED Hotspots Finder - Rings & Planets** and **Hotspots Finder EDMC Plugin** project for **Elite Dangerous**.

**Live website:** https://littlejacket99.github.io/  
**Main project:** https://github.com/LittleJacket99/ED-Hotspots-Finder-Rings-and-Planets-with-EDMC-plugin  
**Latest release:** https://github.com/LittleJacket99/ED-Hotspots-Finder-Rings-and-Planets-with-EDMC-plugin/releases/latest

## About the site

The website is the public landing page for the two connected tools:

- **ED Hotspots Finder - Rings & Planets** — desktop multi-system search, filtering and analysis;
- **Hotspots Finder EDMC Plugin** — in-game Community Deposits lookup, RhinoSpotter synchronization and selected-deposit navigation.

It also documents the shared parts of the ecosystem:

- Rings & Asteroids Mining;
- Planets & Surface Mining;
- the shared **Community Deposits** database;
- RhinoSpotter 5.1+ `rs_api.py` integration;
- links to the Windows Finder executable, EDMC Plugin ZIP, source code and project documentation.

## Community Deposits

Community Deposits is the shared database used by both the Finder and EDMC Plugin for player-reported planetary surface-mining locations.

**Discover → Bookmark → Synchronize → Share → Search**

Compatible RhinoSpotter bookmarks can be synchronized through either client so useful discoveries can become searchable by other commanders.

RhinoSpotter is an independent EDMC plugin developed by **Fumlop** and is not bundled with this project.

## Website structure

- `index.html` — main landing page
- `assets/style.css` — site layout, colors and responsive styling
- `privacy/index.html` — privacy policy
- `.nojekyll` — serves the repository as a simple static GitHub Pages site

Application and plugin screenshots are loaded from the public project repository so the website remains aligned with the current interface.

## Privacy

The privacy page documents the current tools' use of:

- local Finder and EDMC Plugin configuration;
- Spansh requests from the Finder;
- Community Deposits queries and explicit synchronization;
- RhinoSpotter 5.1+ `rs_api.py` access;
- read-only Finder fallbacks for older RhinoSpotter SQLite/JSON storage;
- EDMC / Elite Dangerous status data used locally for deposit navigation;
- local CSV/XLSX exports;
- public GitHub release update checks.

The current project does **not** use the Google Sheets/OAuth workflow from the older pre-v1.0 tool.

## Hosting

The site is served directly from the `main` branch through **GitHub Pages**.

It is intentionally lightweight and uses no JavaScript framework, analytics, advertising or remote fonts.

## Project status

The website follows the current public **v1.0.2** release and links to the main repository for releases, documentation, issues and source code.
