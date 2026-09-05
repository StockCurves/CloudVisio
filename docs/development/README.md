# CloudVisio Development Docs

This folder contains the planning and development workflow documents for CloudVisio.

CloudVisio is planned as a web-based Visio-like diagram editor, built by evaluating and likely forking draw.io/diagrams.net first, then adding CloudVisio-specific templates, storage, import, and AI workflows.

## Documents

- [Product Requirements](./product-requirements.md)
- [Development Priorities](./development-priorities.md)
- [Draw.io Fork Assessment](./drawio-fork-assessment.md)
- [File Format Strategy](./file-format-strategy.md)
- [Roadmap](./roadmap.md)

## Current Direction

The current recommendation is:

1. Start from draw.io/diagrams.net instead of building the full editor from scratch.
2. Keep a CloudVisio semantic JSON format for AI, Git, Markdown, and structured workflows.
3. Support `.vsdx` import as an important compatibility feature.
4. Do not make full `.vsdx` export or perfect Visio round-trip fidelity part of the MVP.
5. Prioritize Visio-like editing, custom templates, connector styles, snap/alignment, and cloud file storage.
