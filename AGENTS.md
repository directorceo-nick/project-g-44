# AGENTS.md

## Architecture
- Static site with no build step. Netlify publishes `public/` (see `netlify.toml`).
- `public/index.html` holds everything: markup, the Tailwind config, styles, and the app script.
- The dataset lives in `createVerifiedMasterCodex()` inside the script. Every module renders from the `codex` object.
- Uploaded JSON goes through `normalizeCodexPayload()`, which accepts both the flat codex shape and the sectioned "01–08" shape.
- The SHA-256 seal is computed from a sorted-key canonical JSON (`canonicalizeJson`) and leaves out the `*_sha256_seal` keys.

## Conventions
- The owner supplied this file. Keep content, figures and identifiers exactly as given unless they ask for a change.
- Use toast notifications (`notify`) rather than `alert()` / `confirm()`.
- Libraries load from CDNs. Don't add a bundler unless the owner asks for one.
