# Roadmap

## Phase 0: Repository and Planning

- Confirm GitHub repository: `StockCurves/CloudVisio`.
- Add development documentation.
- Decide initial license and open-source scope.
- Decide whether to fork draw.io directly into this repository or use a separate upstream fork.

## Phase 1: Draw.io Fork Evaluation

- Fork or clone draw.io/diagrams.net.
- Run the project locally.
- Document build steps.
- Identify configuration points.
- Test basic UI customization.
- Test adding custom shape libraries.
- Test default line and connector styles.

## Phase 2: CloudVisio MVP Customization

- Add CloudVisio branding.
- Add engineering-focused template library.
- Add connector style presets.
- Add simplified template creation workflow.
- Keep core Visio-like editing behavior.

## Phase 3: Storage

- Validate Google Drive save/open in the fork.
- Add custom Google OAuth configuration if needed.
- Validate OneDrive behavior after Google Drive is stable.
- Define file naming and project folder conventions.

## Phase 4: Visio Import

- Collect representative `.vsdx` test files.
- Build import compatibility checklist.
- Test shape, text, connector, style, and layout preservation.
- Document unsupported features.
- Decide whether to rely on draw.io import or build a CloudVisio import adapter.

## Phase 5: CloudVisio JSON

- Define JSON Schema.
- Build JSON import/export.
- Add validation tests.
- Add Markdown/Git-friendly workflows.

## Phase 6: AI Workflows

- Generate diagrams from prompts.
- Generate diagrams from Markdown/spec documents.
- Convert AI output into CloudVisio JSON.
- Add AI-assisted diagram repair after import.

## Phase 7: Advanced Features

- `.vsdx` export.
- Collaboration.
- Comments.
- Enterprise sharing and permissions.
- Advanced template marketplace or package system.
