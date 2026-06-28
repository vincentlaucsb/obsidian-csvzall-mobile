# Repository Guide

This repository is generated from `vincentlaucsb/obsidian-csvzall`.

- Do not edit `main.js`, `styles.css`, `manifest.json`, or `versions.json` directly here.
- Do not edit `mobile-src/` or `src/` directly here; they are source snapshots for Obsidian review.
- Make source changes in `obsidian-csvzall`, then run `npm run sync:mobile-repo`.
- The mobile bundle must not contain Node.js or Electron APIs.
- Obsidian Community releases should attach only `main.js`, `manifest.json`, and `styles.css`.
