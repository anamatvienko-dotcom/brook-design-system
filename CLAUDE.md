# Claude / AI Coding Instructions — Brook Website

Before implementing any Brook UI, read [DESIGN_SYSTEM.md](DESIGN_SYSTEM.md) and [tokens.json](tokens.json). The [visual Google Doc](https://docs.google.com/document/d/1Byfuv3h6QF3E6xd-6aK4TagfQm1CUAfi83MmwBM-k8M/edit) is the editable decision master.

## Priority order
1. Current explicit user instructions.
2. Approved design decisions from the visual master and this technical mirror.
3. Existing component behavior when no approved standard exists.
4. Provisional suggestions only with explicit labeling.

## Requirements
- Montserrat only. Respect responsive typography role sizes.
- Violet and teal are core identity colors; pink for primary actions; blue sparingly.
- Inner content max-width 1200px, with full-bleed section backgrounds where needed.
- Mobile-first. Check desktop, tablet and mobile.
- Maintain product photo proportions, natural shadows, legibility and accessible interactions.
- Do not invent CSS tokens or claim provisional values are approved.
- Do not modify or deploy to `pet-amazing/brook-site` without explicit user permission.
- For GemPages requests, provide **complete HTML, CSS and JavaScript blocks separately**, ready to replace their respective fields, unless asked otherwise.
- Do not commit secrets, customer data, or private company documents to this public repo.

## Maintenance
If the user approves a design change, update the technical spec, JSON tokens and changelog. No automatic Google Docs ↔ GitHub sync exists.
