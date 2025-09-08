# Architecture Overview

## Layers
- UI Layer (Public): Single-file site (index.html) + docs.
- Knowledge Layer (Private): GPT prompts, Q&A, metadata (separate private repo).

## Data Model
- Workflow JSON schema (nodes, edges) used by the UI to render the flow.

## Boundaries
- No prompts or Q&A are stored here.
- Public repo holds only the demo implementation and documentation.

## Future Ports
- Import workflow.json from URL
- Export to Markdown/PNG
- Optional API endpoints
