# Product Requirements

## Product Goal

CloudVisio should become a web-based diagram editor with a user experience close to Microsoft Visio, while adding stronger support for AI-assisted diagram generation, Git-friendly files, Markdown workflows, and cloud storage.

The first target users are hardware, IC, system, and engineering users who need precise diagramming rather than only whiteboarding.

## Core Requirements

### Visio-Like Editing

- Create, select, drag, resize, rotate, align, group, ungroup, copy, paste, duplicate, and delete diagram objects.
- Support multi-page diagrams.
- Support layers, lock/unlock, show/hide, and object ordering.
- Support zoom, pan, grid, rulers, alignment guides, and snap behavior.

### Shapes and Templates

- Provide built-in basic shapes.
- Provide flowchart, system architecture, network, hardware, IC, and signal-flow templates.
- Allow users to create reusable custom templates.
- Allow templates to contain shapes, connectors, labels, default styles, and connection points.
- Support a template library that can be reused across files.

### Connectors and Line Styles

- Support straight, orthogonal, curved, and freeform connectors.
- Support adjustable waypoints.
- Support connector attachment to shape connection points.
- Support source and target arrowheads.
- Support line color, thickness, solid line, dashed line, dotted line, opacity, and labels.
- Support line style presets such as signal, clock, power, ground, data bus, feedback, and control path.

### Auto Snap and Layout

- Snap objects to grid.
- Snap connectors to connection points.
- Provide alignment guides.
- Provide object distribution and alignment commands.
- Support basic automatic layout for selected diagrams.

### File Storage

- Store files in Google Drive.
- Support OneDrive after Google Drive is stable.
- Support local file import/export.
- Keep files portable and not locked to one cloud account.

### Import and Export

- Import `.vsdx` files as a key compatibility feature.
- MVP `.vsdx` import should support basic shapes, text, connectors, line styles, and layout where practical.
- Export to SVG, PNG, and PDF.
- Export to CloudVisio JSON.
- `.vsdx` export is useful but should not be required for MVP.

### AI-Assisted Workflows

- Generate diagrams from prompts.
- Generate diagrams from Markdown, technical notes, or system specifications.
- Modify existing diagrams through natural language instructions.
- Use CloudVisio JSON as the AI-facing semantic format.

## Non-Goals for MVP

- Perfect Microsoft Visio compatibility.
- Full `.vsdx` round-trip import and export.
- Real-time multiplayer collaboration.
- Enterprise permission management.
- Full PDF/datasheet diagram reconstruction.
