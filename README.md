# DomainMapper

A simple, interactive tool to generate to-scale schematics of protein layouts.

Repository: https://github.com/bms-chem/DomainMapper

## Getting started

On first visit (or whenever there's no in-progress diagram), a start
screen offers a few ways in: start with a blank canvas, restore your last
session if one was auto-saved, import a UniProt accession, or load a
worked example. Work is auto-saved to your browser's local storage as you
go, so closing the tab and coming back later offers to restore where you
left off.

## Header toolbar

- **Undo / Redo** (`Ctrl+Z` / `Ctrl+Y`, or `Ctrl+Shift+Z`)
- **Load example**: display a worked example
- **Import UniProt**: enter an accession code to fetch domains, motifs, regions, and binding/active sites from UniProt and flexibly add them to a new protein; **Import JSON**: load a `.json` file, replaces current diagram
- **File name**: base name for all exports; **Export JSON**: full data + all settings that can be re-imported later; **Export image**: choose SVG or PNG (PNG adds an optional transparent background and a 96–600dpi resolution choice)
- **Reset**: clear canvas

## Global settings

Hidden by default — click **Formatting ▾** in the header toolbar to show these controls.

- Format text for protein names, domain names, annotations
- Axis length: sets absolute horizontal width of longest displayed protein; other proteins are always scaled in relation to the longest one.

## Proteins (sidebar list)

- **+ Add**: new protein
- Checkbox: show/hide in diagram
- Click name: select for editing
- ↑ / ↓: reorder
- ⧉: duplicate
- ✕: delete

## Details, Domains, Regions, Motifs & Annotations

- **Details**: Name, Length (aa), Offset (with ←/→ nudge buttons), and coordinate axis formatting (colour, weight)
- **Domains**: toggle showing start/end residues on each domain, format domain box appearance (shape, corner radius, border style/width/colour), and annotate protein domains
- **Regions**: label regions of domains, or areas of the protein (e.g. "disordered region")
- **Motifs**: annotate regions of interest (e.g. a binding site within a domain)
- **Annotations**: annotate sites of interest (e.g. a residue, mutation, or interaction partner)

Overlapping region labels, motif tags, and annotations stack vertically to try and avoid overlaps (up to a point).