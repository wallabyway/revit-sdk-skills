---
name: revit-sdk-skills
description: >-
  Top-level steering file for the Revit SDK documentation knowledge base.
  Use this file to decide which Revit API reference files to read.
  Provides a categorized index of all markdown files under docs/,
  organized by Revit API version (2025, 2026) and technical domain.
---

# Revit SDK Skills

This folder contains searchable Revit API reference documentation generated for GitHub Pages.
It is organized by Revit release year (`revit-api-2025/`, `revit-api-2026/`).

## For Agents: How to use this knowledge base

1. **Identify the Revit API version** the user is asking about (2025 or 2026).
   If no version is specified, default to `revit-api-2026/`.
2. **Read the per-year `SKILL.md`** first — it contains a flat list of every topic file and is the fastest way to confirm a namespace exists.
   - [revit-api-2025/SKILL.md](revit-api-2025/SKILL.md)
   - [revit-api-2026/SKILL.md](revit-api-2026/SKILL.md)
3. **Use the per-year `INDEX.md`** when you need to map a specific type or class name to the file that contains it.
   - [revit-api-2025/INDEX.md](revit-api-2025/INDEX.md)
   - [revit-api-2026/INDEX.md](revit-api-2026/INDEX.md)
4. **Retrieve only the topic files relevant to the question.**
   Each topic file covers one namespace group with full type documentation.
   Concatenate the retrieved files in memory before answering.

## Categorized Topic Index

The files below are grouped by domain. Read the files whose descriptions match the user's question.

### Application & Command Lifecycle

| File | What it covers | Read when asking about |
|------|----------------|------------------------|
| [applicationservices.md](revit-api-2026/applicationservices.md) | `Autodesk.Revit.ApplicationServices` | Application object, product info, language type, journaling |
| [attributes.md](revit-api-2026/attributes.md) | `Autodesk.Revit.Attributes` | Transaction mode, regeneration option, journaling attributes on commands |
| [creation.md](revit-api-2026/creation.md) | `Autodesk.Revit.Creation` | Creating areas, family instances, items via the Creation namespace |
| [db-macros.md](revit-api-2026/db-macros.md) | `Autodesk.Revit.DB.Macros` | Macro recording and macro-related types |

### General Database Types (Autodesk.Revit.DB)

These files are split alphabetically by type name within the main `DB` namespace.

| File | Coverage | Read when asking about |
|------|----------|------------------------|
| [db-a.md](revit-api-2026/db-a.md) | DB types starting with A | Adaptive components, annotations, arcs, arrays |
| [db-b-c.md](revit-api-2026/db-b-c.md) | DB types starting with B-C | Bounding boxes, categories, curves, connectors, colors |
| [db-d.md](revit-api-2026/db-d.md) | DB types starting with D | Datum, dimensions, doors, direct shapes, documents |
| [db-e.md](revit-api-2026/db-e.md) | DB types starting with E | Edges, elements, events, export, electrical basics |
| [db-f.md](revit-api-2026/db-f.md) | DB types starting with F | Families, filters, floors, fills, forms |
| [db-g-i.md](revit-api-2026/db-g-i.md) | DB types starting with G-I | Geometry, graphics, grids, IFC basics, images |
| [db-j-l.md](revit-api-2026/db-j-l.md) | DB types starting with J-L | Joints, levels, links, lines, loads |
| [db-m.md](revit-api-2026/db-m.md) | DB types starting with M | Materials, mep basics, models, rooms (partial) |
| [db-n-p.md](revit-api-2026/db-n-p.md) | DB types starting with N-P | Options, parameters, phases, planes, points |
| [db-r.md](revit-api-2026/db-r.md) | DB types starting with R | Reference, reinforcement, roofs, rooms |
| [db-s.md](revit-api-2026/db-s.md) | DB types starting with S | Selection, settings, shafts, sites, solids, stairs |
| [db-t.md](revit-api-2026/db-t.md) | DB types starting with T | Tables, text, transactions, transforms |
| [db-u-v.md](revit-api-2026/db-u-v.md) | DB types starting with U-V | Units, UVs, views (partial) |
| [db-w-z.md](revit-api-2026/db-w-z.md) | DB types starting with W-Z | Walls, windows, worksets, XYZ |

### Analysis, Energy & Simulation

| File | Coverage | Read when asking about |
|------|----------|------------------------|
| [db-analysis-a-e.md](revit-api-2026/db-analysis-a-e.md) | `Autodesk.Revit.DB.Analysis` [A-E] | Analysis display styles, energy data, analytical models |
| [db-analysis-f-v.md](revit-api-2026/db-analysis-f-v.md) | `Autodesk.Revit.DB.Analysis` [F-V] | Field domains, HVAC loads, spatial field managers, view-specific data |
| [db-analysis-z.md](revit-api-2026/db-analysis-z.md) | `Autodesk.Revit.DB.Analysis` [Z] | Zone-related analysis types (2026 only) |

### Architecture

| File | Coverage | Read when asking about |
|------|----------|------------------------|
| [db-architecture-b-s.md](revit-api-2026/db-architecture-b-s.md) | `Autodesk.Revit.DB.Architecture` [B-S] | Building pads, rooms, room tags, stairs, spatial elements |
| [db-architecture-t-w.md](revit-api-2026/db-architecture-t-w.md) | `Autodesk.Revit.DB.Architecture` [T-W] | Topography, wall types, architectural utilities |

### MEP (Mechanical, Electrical, Plumbing)

| File | Coverage | Read when asking about |
|------|----------|------------------------|
| [db-mechanical-a-r.md](revit-api-2026/db-mechanical-a-r.md) | `Autodesk.Revit.DB.Mechanical` [A-R] | Ducts, mechanical equipment, systems, terminals, spaces |
| [db-mechanical-s-z.md](revit-api-2026/db-mechanical-s-z.md) | `Autodesk.Revit.DB.Mechanical` [S-Z] | Zone equipment, mechanical settings |
| [db-electrical-a-e.md](revit-api-2026/db-electrical-a-e.md) | `Autodesk.Revit.DB.Electrical` [A-E] | Cable trays, circuits, electrical equipment, conduit, demand factors |
| [db-electrical-g-w.md](revit-api-2026/db-electrical-g-w.md) | `Autodesk.Revit.DB.Electrical` [G-W] | Lighting, panels, power, wire types |
| [db-plumbing.md](revit-api-2026/db-plumbing.md) | `Autodesk.Revit.DB.Plumbing` | Pipes, fittings, plumbing fixtures, flow, losses |
| [db-fabrication.md](revit-api-2026/db-fabrication.md) | `Autodesk.Revit.DB.Fabrication` | Fabrication parts, services, hangers, spools |
| [db-lighting.md](revit-api-2026/db-lighting.md) | `Autodesk.Revit.DB.Lighting` | Lighting fixtures, photometric data |
| [db-pointclouds.md](revit-api-2026/db-pointclouds.md) | `Autodesk.Revit.DB.PointClouds` | Point cloud imports, filters, scans |

### Structural Engineering

| File | Coverage | Read when asking about |
|------|----------|------------------------|
| [db-structure-a-c.md](revit-api-2026/db-structure-a-c.md) | `Autodesk.Revit.DB.Structure` [A-C] (2026) / [A-D] (2025) | Analytical models, beams, braces, columns |
| [db-structure-e-r.md](revit-api-2026/db-structure-e-r.md) | `Autodesk.Revit.DB.Structure` [E-R] | Floors, foundations, framing, rebar, loads |
| [db-structure-s-z.md](revit-api-2026/db-structure-s-z.md) | `Autodesk.Revit.DB.Structure` [S-Z] | Structural settings, walls, zones |
| [db-structure-structuralsections-s.md](revit-api-2026/db-structure-structuralsections-s.md) | `Autodesk.Revit.DB.Structure.StructuralSections` | Structural section shapes and profiles |
| [db-steel.md](revit-api-2026/db-steel.md) | `Autodesk.Revit.DB.Steel` | Steel connections, detailing, fabrication |

### Geometry, Graphics & Visualization

| File | Coverage | Read when asking about |
|------|----------|------------------------|
| [db-directcontext3d.md](revit-api-2026/db-directcontext3d.md) | `Autodesk.Revit.DB.DirectContext3D` | Custom 3D graphics, buffers, rendering primitives |
| [db-visual-a-g.md](revit-api-2026/db-visual-a-g.md) | `Autodesk.Revit.DB.Visual` [A-G] | Appearance assets, materials, visual parameters |
| [db-visual-h-w.md](revit-api-2026/db-visual-h-w.md) | `Autodesk.Revit.DB.Visual` [H-W] | Schemas, textures, visual proxies |

### Events, Storage & External Services

| File | Coverage | Read when asking about |
|------|----------|------------------------|
| [db-events-a-r.md](revit-api-2026/db-events-a-r.md) | `Autodesk.Revit.DB.Events` [A-R] | Document events, element events, failures, pre/post events |
| [db-events-r-w.md](revit-api-2025/db-events-r-w.md) | `Autodesk.Revit.DB.Events` [R-W] (2025) | Remaining event types in 2025 |
| [db-events-u-w.md](revit-api-2026/db-events-u-w.md) | `Autodesk.Revit.DB.Events` [U-W] (2026) | Remaining event types in 2026 |
| [db-extensiblestorage.md](revit-api-2026/db-extensiblestorage.md) | `Autodesk.Revit.DB.ExtensibleStorage` | Custom schemas, entity storage, fields |
| [db-externalservice.md](revit-api-2026/db-externalservice.md) | `Autodesk.Revit.DB.ExternalService` | External services, server registration |

### Interoperability

| File | Coverage | Read when asking about |
|------|----------|------------------------|
| [db-ifc.md](revit-api-2026/db-ifc.md) | `Autodesk.Revit.DB.IFC` | IFC export, import, options, classification |

### Exceptions

| File | Coverage | Read when asking about |
|------|----------|------------------------|
| [exceptions-a-r.md](revit-api-2026/exceptions-a-r.md) | `Autodesk.Revit.Exceptions` [A-R] | Revit API exceptions and error conditions |
| [exceptions-s-w.md](revit-api-2026/exceptions-s-w.md) | `Autodesk.Revit.Exceptions` [S-W] | Additional exception types |

## Version Notes

- `revit-api-2026/` is the newer release and contains a few extra files (e.g., `db-analysis-z.md`, `db-events-u-w.md`) and slight namespace splits compared to 2025.
- `revit-api-2025/` uses `db-structure-a-d.md` where 2026 uses `db-structure-a-c.md`.
- When in doubt, search both years' `INDEX.md` files for the type name.

## Retrieval Strategy

- **Broad question** (e.g., "How do I create a duct?"): read the per-year `SKILL.md`, then the relevant domain files (e.g., MEP files).
- **Specific type question** (e.g., "What methods does `Duct` have?"): read the per-year `INDEX.md` to locate the exact file, then read only that file.
- **Cross-domain question**: retrieve the primary domain file plus any related files (e.g., structure + geometry + exceptions).
