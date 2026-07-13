# DomainMapper

A simple, interactive tool to generate to-scale schematics of protein layouts.

Repository: https://github.com/bms-chem/DomainMapper

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
- **Import**: load a `.json` file, replaces current diagram
- **Export JSON**: full data + all settings that can be re-imported later
- **Export image**: choose SVG (vector) or PNG (raster); PNG also offers a transparent-background option and a resolution (dpi) setting
- **Load example**: display a worked example (Class VI TRIM family, EGFR, HIF-1α, IpaH9.8, NRF2, SRC, TXN)
- **Undo / Redo** (`Ctrl+Z` / `Ctrl+Y`, or `Ctrl+Shift+Z`)
- **Reset**: clear canvas


To do:
- ability to visually resize domains by dragging?
- import from uniprot accession?
- google analytics for tracking
- feedback/feature request/bug reporting?
- rename Group label functionality as Region label
- colour palettes (change the default at the very least)
- rename imports to "Import JSON" and "Import UniProt"
- suggested features/functionality
- suggested consolidatoin/reorganisation of the UI to retain functionality but make tidier/cleaner
