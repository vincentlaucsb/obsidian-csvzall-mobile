# csvzall Mobile

<img src="https://raw.githubusercontent.com/vincentlaucsb/csvzall/refs/heads/master/assets/csvzall-logo-theme-safe.png" alt="csvzall logo: a reciprocating saw cutting through a spreadsheet" width="760">

Open and edit CSV files directly inside Obsidian mobile with the bundled
csvzall WASM viewer.

csvzall Mobile is the phone and tablet companion to
[csvzall for Obsidian](https://github.com/vincentlaucsb/obsidian-csvzall). It
does not install the desktop helper binary and does not require a local server.

If csvzall Mobile saves you time, please star this repository. It helps other
Obsidian users find the plugin and helps me gauge demand for continued mobile
support.

## What It Does

- Opens `.csv` files in an Obsidian mobile pane.
- Loads the bundled WASM viewer without installing a desktop helper binary.
- Supports basic CSV editing and saving back to the vault file.
- Includes an Obsidian-style mobile toolbar button for opening navigation.
- Stays inert on desktop so it does not compete with the desktop csvzall plugin
  for CSV ownership.

## Requirements

- Obsidian mobile.
- A vault containing `.csv` files.
- No external `csvzall` binary is required.

## Desktop Version

For desktop-native features such as chart generation, SQLite queries, large-file
viewing through the native helper process, and managed helper binary updates,
install [csvzall for Obsidian](https://github.com/vincentlaucsb/obsidian-csvzall).

It is safe to keep both plugins in the same synced vault. The desktop plugin is
desktop-only, and csvzall Mobile only registers itself as a CSV handler on
Obsidian mobile.

## Privacy and Network Use

csvzall Mobile does not collect telemetry and does not download executable code
at runtime. The WASM viewer assets are embedded in `main.js` and materialized
into the plugin directory when the plugin loads.

## Limitations

- Mobile support is focused on CSV viewing and editing.
- Charts, SQLite queries, and desktop helper-process features live in the
  desktop plugin.
- Very large files may still exceed what a mobile device can comfortably hold in
  memory.

## Development

This repository is generated from
[vincentlaucsb/obsidian-csvzall](https://github.com/vincentlaucsb/obsidian-csvzall).
The TypeScript source snapshot used for review lives in `mobile-src/` and
`src/`. Do not edit generated plugin assets or source snapshots here by hand;
make source changes in the desktop/source repository and sync this distribution
repo.
