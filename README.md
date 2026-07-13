# DomainMapper

A simple, interactive tool to generate to-scale schematics of protein layouts.

Repository: https://github.com/bms-chem/DomainMapper

## Layout

- Header: global settings, import/export
- Sidebar (left, scrolls independently): protein list + editor
- Canvas (right): live diagram

## Proteins (sidebar list)

- **+ Add**: new protein
- Checkbox: show/hide in diagram
- Click name: select for editing
- ↑ / ↓: reorder
- ⧉: duplicate
- ✕: delete

## Protein editor

- **Name**, **Length** (aa)
- **Show start/end residues on each domain**: on/off
- **Domain box**: format appearance of protein domains (shape, corner radius, border style/width/colour)
- **Coordinate axis**: format appearance of the residue coordinate axis (colour, weight)
- **Group labels**: label groups of domains, or areas of the protein (e.g. "disordered region")
- **Domains**: annotate protein domains
- **Motif marks**: annotate regions of interest (e.g. a binding site within a domain)
- **Annotations**: annotate sites of interest (e.g. a residue, mutation, or interaction partner)

Overlapping group labels, motif tags, and annotations stack vertically to try and avoid overlaps (up to a point).

## Global settings

- Format text for protein names, domain names, annotations
- Axis length: sets absolute horizontal width of longest displayed protein; other proteins are always scaled in relation to the longest one.

## Import / Export (header)

- **File name**: base name for all exports
- **Import…**: load a `.json` file, replaces current diagram
- **Export JSON**: full data + all settings that can be re-imported later
- **Export…**: choose SVG (vector) or PNG (raster); PNG also offers a transparent-background option and a resolution (dpi) setting
- **Load example…**: display a worked example (Class VI TRIM family, EGFR, HIF-1α, IpaH9.8, NRF2, SRC, TXN)
- **Undo / Redo**: step backward/forward through recent edits (`Ctrl+Z` / `Ctrl+Y`, or `Ctrl+Shift+Z`)
- **Reset**: clear to single blank protein

## Autosave / session restore

- Your work is saved automatically to this browser (debounced ~400ms after each edit) — no explicit save step needed.
- On reload, if a saved session exists, you'll be offered a **Restore your last session** option alongside the worked examples.
- **Reset** clears both the on-screen diagram and the saved session.


To do:
- ability to visually resize domains by dragging?
- import from uniprot accession?