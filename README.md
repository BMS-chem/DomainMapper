# DomainMapper

A simple, interactive tool to generate to-scale schematics of protein layouts.

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
- **Transparent background**: checkbox, applies to SVG/PNG export
- **Export SVG**: vector
- **Export PNG**: raster
- **Load example…**: display a worked example (Class VI TRIM family, EGFR, HIF-1α, NRF2, SRC, TXN)
- **Reset**: clear to single blank protein


To do:
- add name and version to footer(?) w/ my name too
- check that SVG export includes editable text, font selection, etc
- check resolution of PNG export (300 dpi/600 dpi options?)
- add undo/redo button?
- ability to visually resize domains by dragging?
- mention github repo in help panel
- import from uniprot accession?