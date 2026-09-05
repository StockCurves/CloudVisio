# Development Priorities

## Priority Summary

CloudVisio should prioritize a strong Visio-like web editing experience before advanced AI and full Visio compatibility.

## P0: MVP Foundation

### Editor Foundation

- Fork and run draw.io/diagrams.net locally.
- Confirm build, packaging, and deployment path.
- Identify how to customize the editor UI, shape libraries, default styles, storage options, and import/export commands.

### Visio-Like Editing

- Preserve and validate canvas editing features:
  - shape creation
  - selection
  - drag and resize
  - copy/paste
  - grouping
  - alignment
  - zoom/pan
  - pages
  - layers

### Template System

- Create a CloudVisio template pack.
- Add hardware, IC, system architecture, and signal-flow diagram symbols.
- Define initial template categories.
- Make template creation easier than editing raw draw.io XML.

### Connector and Style Presets

- Define default connector presets:
  - signal
  - clock
  - power
  - ground
  - data bus
  - feedback
  - control path
- Ensure each preset controls line color, thickness, pattern, arrowheads, and label behavior.

## P1: Storage and Compatibility

### Google Drive

- Verify Google Drive save/open behavior in the forked version.
- Decide whether a custom OAuth app is needed.
- Test file creation, update, rename, and conflict behavior.

### Visio Import

- Build a `.vsdx` import test set.
- Test shape, text, connector, color, dashed line, arrowhead, and layout preservation.
- Document unsupported Visio features.
- Decide whether to use draw.io import directly or build an adapter into CloudVisio JSON.

### CloudVisio JSON

- Define a semantic JSON schema for diagrams.
- Use the schema for AI generation, Git diff, Markdown embedding, validation, and future automation.

## P2: Product Differentiation

### AI Generation

- Generate CloudVisio JSON from prompts.
- Convert CloudVisio JSON into draw.io-compatible diagrams.
- Add AI-assisted diagram repair after Visio import.

### OneDrive

- Add and validate OneDrive storage after Google Drive is stable.

### Markdown and Git Workflows

- Export diagrams with a Markdown-friendly reference format.
- Support Git-friendly file review and schema validation.

## P3: Advanced Compatibility

- Add `.vsdx` export if there is enough demand.
- Improve Visio round-trip fidelity.
- Add real-time collaboration.
- Add enterprise permission and sharing workflows.
