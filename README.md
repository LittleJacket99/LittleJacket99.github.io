# ED Hotspots & Landables Finder website

Static GitHub Pages site for `LittleJacket99/LittleJacket99.github.io`.
No build dependencies, scripts, analytics, remote fonts or credentials.

## Publish

1. Create the public repository `LittleJacket99.github.io` under LittleJacket99.
2. Upload these files to the root of `main`, preserving `privacy/` and `assets/`.
3. In Settings → Pages, choose Deploy from a branch → main → / (root) → Save.
4. Wait for deployment and check `https://littlejacket99.github.io/` and `/privacy/`.
5. Ensure HTTPS is enabled. Do not configure a custom domain.

## Search Console verification

Use the Google account that owns or edits the OAuth Cloud project.
Add a **URL-prefix** property for `https://littlejacket99.github.io/` in
[Search Console](https://search.google.com/search-console). A Domain property
requires DNS control and is not the appropriate method for this Pages subdomain.
Choose HTML tag verification. Paste Google's exact meta tag into `index.html`
at the marked comment inside `<head>`. Commit, wait for Pages deployment,
check the live page source, and verify. Keep the tag after verification.
No placeholder verification value is included.

## OAuth checkpoint — do not change configuration yet

Homepage candidate: `https://littlejacket99.github.io/`
Privacy candidate: `https://littlejacket99.github.io/privacy/`
Authorized-domain candidate (no protocol or path): `littlejacket99.github.io`

`github.io` appears on the Public Suffix List, which supports treating this
account subdomain as a top private domain under Google's guidance. This is
not proof that Google accepts this particular domain. After the public site
and ownership verification are working, inspect Google's Authorized Domains
validation and record the result before saving OAuth changes. Do not change
scopes, client type, publishing status or branding as part of deploying this site.
Domain acceptance alone does not complete OAuth app verification.

References:
- https://developers.google.com/identity/protocols/oauth2/production-readiness/brand-verification
- https://support.google.com/webmasters/answer/9008080
- https://publicsuffix.org/list/public_suffix_list.dat

## Release link

The homepage points to GitHub Releases, with an explicit notice that the Windows
EXE is not yet published. On September 13, 2026, v7.11 had zero release assets.
Remove that notice only after a working distribution build is actually uploaded;
then add the exact verified Windows asset URL if desired. Do not upload OAuth
JSON files, tokens or personal configuration here.

## Privacy source audit

Reviewed v7.11 implementation at app repository commit
`018034f8125285ed61e96758263a436ff80d1155`.
The unchanged engine blob is `a4172a8546748668e4a02e7b034e7440913b525d`.

- `hotspots_engine.py`: SCOPES, app_data_dir, get_credentials, config persistence,
  Google Sheets read/write/copy/style operations, Spansh requests and CSV/summary output.
- `hotspots_finder_gui.py`: connection/template buttons, scan controls and activity log.
- `HotspotsFinder.spec`: bundled OAuth client resource; never a separate website file.
- `docs/HotspotsFinder_Template_AppsScript_v9.gs`: spreadsheet maintenance reference.

Important distinctions retained in the policy: broad spreadsheets scope versus
the app's selected-sheet behavior; system-name transfer to Spansh; local exports
outside AppData; no partial results table on STOP does not imply no local files;
existing tabs not replaced by template copies does not imply no functional repairs.

The Limited Use statement describes this project's use and transfer commitments;
it is not a Google approval claim. Re-review this policy when implementation changes.

For local preview, run `python -m http.server 8000` in this directory and open
`http://localhost:8000/`. Python is only a developer preview convenience.
