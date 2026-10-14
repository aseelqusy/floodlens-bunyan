# FloodLens — deployment-ready website

This is a static website. No Node.js, build step, or backend is required.

## Add your two images

1. Put your QGIS-exported **August 16, 2026** image at `assets/before.png`.
2. Put your QGIS-exported **August 28, 2026** image at `assets/after.png`.
3. Ensure both images have **identical dimensions, geographic extent, orientation, and alignment** for a meaningful slider comparison. Export matching map canvases from QGIS; avoid mismatched cropping.
4. Open `index.html` to preview. Missing-image placeholders will disappear once images are added.

## Deploy (Netlify)

1. Go to https://app.netlify.com/drop
2. Drag the **floodlens-deploy folder** (not just index.html) onto the upload area.
3. Netlify will give you a public URL. You can change the site name in site settings.

## Deploy (GitHub Pages)

1. Create a repository, upload all files including `assets/`.
2. In Settings > Pages, choose Deploy from branch, main, root.
3. Wait for the Pages URL to become available.

## Important scientific scope

This is a **visual comparison prototype**, not an automatic flood detector. No flood occurrence, flood area, or damage estimate is asserted. Planned API, database, map, and detection features are explicitly labeled future work.

## Image size / performance

For best performance, export images at the same size, ideally 1600–2400 px wide, optimized for web. The site references local PNG files and otherwise uses only Google Fonts (which can fall back to system fonts if offline).

## Customization

- Edit titles, descriptions, team members, and sources in `index.html`.
- Change colors at the top of `styles.css`.
- `script.js` handles slider, image fallback, and mobile menu.
