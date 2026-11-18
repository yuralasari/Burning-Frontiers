# Burning Frontiers — prototype v0.1

Interactive ERA5 wind map for Borneo and Andes–Amazon, developed for *Simulations, Models, Twins*.

## Live site (after publishing)
GitHub repository Settings → Pages → Deploy from branch → main → /(root) → Save.

## Files
- `index.html` — static MapLibre interface; no build process required.
- `data/borneo.json` and `data/amazon.json` — sampled monthly U/V winds at 850 hPa from the provided ERA5 NetCDF files, for 2015, 2019 and 2024.

## How to publish
1. Create a public GitHub repository named `burning-frontiers`.
2. Upload `index.html`, `README.md`, and the `data` folder with both JSON files (maintain folder structure).
3. Commit to `main`.
4. Settings → Pages → Deploy from branch → `main` / `(root)` → Save.
5. Open `https://YOUR-USERNAME.github.io/burning-frontiers/` after deployment.

## Methodological notes
- 850 hPa is not surface wind. Monthly mean wind vectors cannot reconstruct fire propagation or smoke episodes.
- The data are spatially subsampled to keep the prototype fast.
- The wind field is atmospheric context, not evidence of El Niño, ignition, or responsibility.
- Planned next steps: add fire detections and rainfall anomalies, and compare climate-only and climate-plus-landscape models with out-of-sample validation.
