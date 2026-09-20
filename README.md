# ED Hotspots Finder - Rings & Planets Website

Official GitHub Pages site for **ED Hotspots Finder - Rings & Planets**, an open-source Windows companion for **Elite Dangerous**.

**Live website:** https://littlejacket99.github.io/  
**Main project:** https://github.com/LittleJacket99/ED-Hotspots-Finder-Rings-and-Planets-with-EDMC-plugin  
**Latest release:** https://github.com/LittleJacket99/ED-Hotspots-Finder-Rings-and-Planets-with-EDMC-plugin/releases/latest

## About the site

The website is the public landing page for ED Hotspots Finder and focuses on the parts of the project most useful to commanders looking for mining and planetary data:

- multi-system search and filtering;
- **Rings & Asteroids Mining**;
- **Planets & Surface Mining**;
- the shared **Community Deposits** database;
- optional **RhinoSpotter** bookmark synchronization;
- links to the Windows download, source code and project documentation.

The general workflow is simple: define the systems or search area, then find the rings, hotspots, planets and known surface deposits that match the required conditions.

## Community Deposits

Community Deposits is a shared database of player-reported planetary surface-mining locations.

**Discover → Bookmark → Synchronize → Share → Search**

Compatible RhinoSpotter bookmarks can be synchronized through ED Hotspots Finder so useful discoveries can become searchable by other commanders.

RhinoSpotter is an independent EDMC plugin developed by **Fumlop** and is not bundled with this project.

## Website structure

- `index.html` — main landing page
- `assets/style.css` — site layout, colors and responsive styling
- `privacy/index.html` — privacy policy
- `.nojekyll` — serves the repository as a simple static GitHub Pages site

The logo and application screenshot are loaded from the public ED Hotspots Finder repository so the website remains aligned with the current application assets.

## Privacy

The privacy page documents the current desktop application's use of:

- local application settings;
- Spansh requests;
- Community Deposits queries and synchronization;
- read-only access to the local RhinoSpotter database;
- local CSV/XLSX exports.

The current application does **not** use the Google Sheets/OAuth workflow from the older pre-v1.0 tool.

## Hosting

The site is served directly from the `main` branch through **GitHub Pages**.

It is intentionally lightweight and uses no JavaScript framework, analytics, advertising or remote fonts.

## Project status

The website follows the current public release line of **ED Hotspots Finder - Rings & Planets** and links to the main repository for releases, documentation, issues and source code.
