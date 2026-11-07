# ttrtahir.github.io

Portfolio of Yusuf Tahir Aydin: a low-poly archipelago built with three.js. It has a home island and three districts (Work, Study, Hobbies), and each island holds one piece of work.

## Add an island

1. In `index.html`, find the `ISLANDS` list in the script and add a line, for example:
   `{ id: "running", district: "hobbies", name: "Running", sub: "Half marathons", prop: "trees" },`
2. Add the panel text as a template with the matching id, next to the others:
   `<template id="c-running"> ... </template>`
3. Done. The island gets placed, bridged, labelled and numbered automatically.

`prop` decides what stands on the island. The options are house, bars, roads, office, factory, school, tensor, rocket, lighthouse, arcade, chess, music, radio, camera, offclock and trees. You can add new props to the `PROPS` object.

## Add a district

Add an entry to `DISTRICTS` with an id, a name, an angle in degrees and a distance from the centre, then give islands that district id.

## Preview and deploy

- Preview: run `python -m http.server` in this folder and open http://localhost:8000. Opening the file directly won't work, because ES modules need a server.
- Deploy: push to `main` with GitHub Pages set to deploy from the `main` branch, root folder.
- three.js 0.170 is included in `assets/js/`, so nothing loads from a CDN.

## Links, quick view and CV

- Every island and district has its own link, for example `ttrtahir.github.io/#comitatus`, `#police`, `#apg`, `#duyvis`, `#thesis`, `#offclock` or `#work`. Opening one flies straight there.
- `ttrtahir.github.io/#quick` opens the one-page summary. Phones always get this version.
- **CV:** lives at `assets/yusuf-aydin-cv.pdf` and is linked from the top bar, the About me panel and the quick view. To update it, replace that file and keep the name.
- The share image for LinkedIn and WhatsApp is `assets/og.jpg`. LinkedIn caches previews, so use the LinkedIn Post Inspector to refresh it after deploying.
