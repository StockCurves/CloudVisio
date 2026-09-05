# Draw.io Fork Assessment

## Why Start from Draw.io

draw.io/diagrams.net already covers a large portion of the requested Visio-like editing surface:

- browser-based diagram editor
- open-source JavaScript codebase
- shape libraries
- custom shapes
- templates
- connector styles
- grid and snap behavior
- cloud storage integrations
- export formats
- `.vsdx` import

Starting from draw.io should be faster than building a full canvas editor, connector system, style panel, import/export layer, and storage integrations from scratch.

## Capabilities Likely Already Covered

| Area | Expected draw.io Coverage | Notes |
|---|---|---|
| Canvas editing | Strong | Selection, drag, resize, copy/paste, group, align |
| Shape libraries | Strong | Built-in libraries plus custom libraries |
| Custom shapes | Strong | XML-based geometry and connection points |
| Connector styling | Strong | Line pattern, color, thickness, waypoints, arrowheads |
| Export | Strong | SVG, PNG, PDF, XML/HTML |
| Cloud storage | Strong | Google Drive, OneDrive, Dropbox, GitHub/GitLab depending on deployment |
| `.vsdx` import | Partial | Must test real files |
| AI generation | Emerging/configurable | Needs CloudVisio-specific workflow |

## Likely Gaps to Fill

### Product and UX Gaps

- CloudVisio branding and simplified navigation.
- A more focused workflow for engineering diagrams.
- Easier custom template creation.
- Better default template organization.
- Better mobile/tablet behavior if needed.

### Domain Gaps

- Hardware and IC diagram symbol library.
- Signal-flow and control-loop presets.
- Engineering connector style presets.
- Block diagram conventions.
- Reusable diagram templates for technical documentation.

### Data and Workflow Gaps

- CloudVisio JSON semantic format.
- Markdown and Obsidian-friendly export.
- Git-friendly diff and validation.
- AI prompt-to-diagram pipeline.
- AI diagram repair pipeline.

### Compatibility Gaps

- More predictable `.vsdx` import behavior.
- Import test suite for real Visio files.
- Unsupported-feature reporting after import.
- Possible conversion from `.vsdx` to CloudVisio JSON.

## Fork Evaluation Checklist

1. Can the repository build locally?
2. Can the editor be deployed as a standalone web app?
3. Can the UI be customized without fighting the codebase?
4. Can custom shape libraries be bundled by default?
5. Can default connector styles and palettes be configured?
6. Can Google Drive and OneDrive integrations work in a self-hosted fork?
7. Can `.vsdx` import be tested and extended?
8. Can a CloudVisio JSON import/export layer be added?
9. Can AI generation be integrated cleanly?
10. Is the maintenance cost acceptable compared with building from scratch?

## Decision Gate

After the fork evaluation, choose one of two paths:

- Continue with draw.io fork if customization and storage integration are practical.
- Build a custom editor if draw.io customization is too costly or too hard to maintain.
