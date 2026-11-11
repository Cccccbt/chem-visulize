# chem-visulize

Interactive chemistry visualizations in the browser.

`index.html` is a single static page with no build step; libraries and fonts load
from CDNs. The header bar switches between tools, grouped by topic, and the home
page (`index.html` or `#home`) lists them all.

| Topic | Tool | URL |
| --- | --- | --- |
| Atomic structure | Atomic Orbital Viewer — every occupied orbital of an element or ion in 3D | `#orbitals` |
| Atomic structure | Quantum Number Explorer — one orbital from n, l, mₗ, mₛ | `#quantum` |
| Atomic structure | Periodic Trends — the periodic table as a 3D bar chart | `#trends` |
| Chemical bonding | Lewis Structure Viewer — Lewis structure from a formula, step by step, with formal charges, resonance and VSEPR shape | `#lewis` |
| Chemical bonding | VSEPR Model — 3D electron-domain geometry with lone pairs and bond angles; optional polarity view (bond dipoles, net dipole, δ+/δ−) | `#vsepr` |
| Thermochemistry | Bomb Calorimeter — animated cutaway with q = C·ΔT → ΔU → ΔH | `#calorimeter` |

### Adding a tool

1. Add its markup as a `<div class="app" id="…" hidden>` with a `.viewer` and a `.panel`.
2. Add one entry to `TOPICS` in the last `<script>` (site map + router). The header
   nav, the home page card and routing are all generated from that list.

### Run locally

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

### Deploy

Served by GitHub Pages from the `main` branch root:
https://cccccbt.github.io/chem-visulize/

