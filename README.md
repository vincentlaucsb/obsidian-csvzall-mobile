# csvzall Mobile

Open and edit CSV files in Obsidian mobile with the bundled csvzall WASM viewer.

This repository is generated from [vincentlaucsb/obsidian-csvzall](https://github.com/vincentlaucsb/obsidian-csvzall). Do not edit generated plugin assets here by hand; make source changes in the desktop/source repository and sync this distribution repo.

## Features

- Opens .csv files in an Obsidian mobile pane.
- Loads the bundled WASM viewer without installing a desktop helper binary.
- Supports basic CSV editing and saving back to the vault file.
- Does not register as the CSV handler on desktop; use the desktop csvzall plugin there.

## Privacy and Network Use

csvzall Mobile does not collect telemetry and does not download executable code at runtime. The WASM viewer assets are embedded in `main.js` and materialized into the plugin directory when the plugin loads.

## Desktop Version

For desktop-native features such as chart generation, SQLite queries, and the native helper-process viewer, install [csvzall for Obsidian](https://github.com/vincentlaucsb/obsidian-csvzall).
