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

## Details, Domains, Regions, Motifs & Annotations

- **Details**: Name, Length (aa), Offset, and coordinate axis formatting (colour, weight)
- **Domains**: toggle showing start/end residues on each domain, format domain box appearance (shape, corner radius, border style/width/colour), and annotate protein domains
- **Regions**: label regions of domains, or areas of the protein (e.g. "disordered region")
- **Motifs**: annotate regions of interest (e.g. a binding site within a domain)
- **Annotations**: annotate sites of interest (e.g. a residue, mutation, or interaction partner)

Overlapping region labels, motif tags, and annotations stack vertically to try and avoid overlaps (up to a point).

## Global settings

- Format text for protein names, domain names, annotations
- Axis length: sets absolute horizontal width of longest displayed protein; other proteins are always scaled in relation to the longest one.

## Header toolbar

- **Load example**: display a worked example
- **Reset**: clear canvas; **Undo / Redo** (`Ctrl+Z` / `Ctrl+Y`, or `Ctrl+Shift+Z`)
- **Import UniProt**: enter an accession code to fetch domains, motifs, regions, and binding/active sites from UniProt and add them to a new protein (also available from the start screen); **Import JSON**: load a `.json` file, replaces current diagram
- **File name**: base name for all exports; **Export JSON**: full data + all settings that can be re-imported later; **Export image**: choose SVG or PNG


To do:
- colour palettes (change the default at the very least)
- suggested features/functionality
- reverse vertical stacking for above line collision avoidance
- ability to re-order motifs in the list (which affects vertical stacking in the plot)