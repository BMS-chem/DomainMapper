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

Overlapping group labels, motif tags, and annotations will stack to try and avoid collisions.

## Global settings

- Format text for protein names, domain names, annotations
- Axis length: sets absolute horizontal width of longest displayed protein; other proteins are always scaled in relation to the longest one.

## Import / Export (header)

- **File name**: base name for all exports
- **Import JSON**: load a `.json` file, replaces current diagram
- **Export JSON**: full data + all settings that can be re-imported later
- **Import UniProt**: enter an accession code to fetch domains, motifs, regions, and binding/active sites from UniProt and add them to a new protein
- **Export image**: choose SVG or PNG
- **Load example**: display a worked example
- **Undo / Redo** (`Ctrl+Z` / `Ctrl+Y`, or `Ctrl+Shift+Z`)
- **Reset**: clear canvas


To do:
- ability to visually resize domains by dragging?
- feedback/feature request/bug reporting?
- rename Group label functionality as Region label
- colour palettes (change the default at the very least)
- suggested features/functionality
- suggested consolidatoin/reorganisation of the UI to retain functionality but make tidier/cleaner
- recreate worked examples from uniprot import
- add custom umami tracking events for different exports, imports, worked examples
- change footer to: Privacy • GitHub • License
- Privacy gives statement along the lines of: DM uses Umami Analytics to collect anonymous usage statistics such as page visits and activity. Umami and DomainMapper do not record any actual input entered by a user. Umami does not use cookies for analytics and does not collect personally identifiable information or track users across websites.