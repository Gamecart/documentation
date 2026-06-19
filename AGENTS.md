# Gamecart documentation instructions

## About this project

- This is the official public documentation site for Gamecart.
- The site is built with Mintlify.
- Pages are MDX files with YAML frontmatter.
- Configuration lives in `docs.json`.
- Use direct file edits unless a Mintlify MCP/tool is explicitly available in the current session.
- Package execution must use Socket Firewall, for example `sfw.cmd npx mint dev`.
- Do not add a versioned package manifest or dependency unless the user explicitly asks for it.

## Terminology

- Use "store" for a seller's Gamecart storefront.
- Use "dashboard" for the authenticated admin application at `dash.gamecart.gg`.
- Use "storefront" for the public buyer-facing store.
- Use "server integration" for delivery automation connected to a game server.
- Use "API reference" only for content generated from, or manually verified against, the current backend contract.

## Style preferences

- Public documentation is written in English by default.
- Internal vault documentation in `.docs/` remains Portuguese-BR.
- Use active voice and second person ("you").
- Keep sentences concise: one idea per sentence.
- Use sentence case for headings.
- Bold for UI elements: Click **Settings**.
- Code formatting for file names, commands, paths, and code references.

## Content boundaries

- Document public workflows, tutorials, API behavior, and webhook behavior that a seller or integration developer can rely on.
- Do not document internal-only endpoints, admin-only implementation details, secrets, callback tokens, provider credentials, or operational runbooks meant only for maintainers.
- Do not invent API or webhook payloads from memory. Check the backend REST resources, DTOs, generated OpenAPI, and relevant `.docs` contracts first.
- Keep API and webhook placeholders explicit until the verified contract is ready.
