# Gamecart Docs

Official public documentation for Gamecart.

This site is built with Mintlify and lives in `projects/documentation`.

## Development

Run commands from this directory.

```bash
sfw.cmd npx mint dev
```

Socket Firewall is required for package execution in this workspace. Do not bypass it if a package is blocked.

## Content rules

- Public documentation is written in English by default.
- The internal `.docs/` vault remains in Portuguese-BR.
- Tutorial content can explain workflows, but it must not invent backend behavior.
- API reference content must be generated from, or manually verified against, the current backend REST resources, DTOs, and OpenAPI output.
- Webhook documentation must be based on current backend callback contracts and vault notes.
- Never publish secrets, internal-only endpoints, callback tokens, or placeholder credentials.

## Structure

- `docs.json` controls navigation, branding, and global settings.
- `index.mdx` is the documentation home page.
- `quickstart.mdx` is the first setup path.
- `tutorials/` contains task-oriented guides.
- `api-reference/` is reserved for generated or verified API documentation.
- `webhooks/` is reserved for public webhook documentation.

## Publishing changes

Mintlify deployment is handled outside this local template. Keep this repository as the source for published documentation content.
