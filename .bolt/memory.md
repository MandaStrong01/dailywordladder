# Project memory

## Product intent & audience

- Word ladder game (single-page web game).

## Brand personality & voice

- TBD — no brand/voice details surfaced yet.

## Visual design & UX direction

- Static standalone HTML game UI; assets include PNG icons, a web manifest, and a share card.
- Inferred: no framework/UI library; vanilla HTML/CSS/JS in one `index.html`.

## Decisions, constraints & rationale

- Project was originally a standalone static `index.html` with no build step or dependencies; running `npm`/`package.json` commands failed with "no package.json found".
- Added a Vite build configuration to enable build and publish.
- `index.html` kept at project root as Vite entry point.
- Static assets (PNG icons, manifest, share card) moved into `public/` so Vite copies them as-is into output.
- Build now succeeds and produces `dist/`; project is ready to publish.

## Open questions & assumptions

- Publish/deploy target is not specified (assumed static host compatible with `dist/`).
- No tests or linting introduced yet.
- Brand/voice and detailed UX/aesthetic direction not yet defined.