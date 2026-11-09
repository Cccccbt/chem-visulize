# chem-visulize

Interactive chemistry visualizations in the browser.

## Atomic Orbital Viewer

`index.html` — a 3D atomic orbital viewer (three.js) with periodic-trend charts.
It is a single static page with no build step; libraries and fonts load from CDNs.

## Bomb Calorimeter

`index.html#calorimeter` — an animated cutaway of a bomb calorimeter with a live
temperature trace. Pick a sample, ignite it, and follow the worked calculation
(q = C·ΔT → ΔU → ΔH), or run it in reverse to calibrate the calorimeter constant.

### Run locally

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

### Deploy

Served by GitHub Pages from the `main` branch root:
https://cccccbt.github.io/chem-visulize/
