# Asset layout

This repository is being used as a GitHub Pages-backed asset host.

## Active directories

- `assets/gamma/` — assets intended to be consumed by Gamma or related slide-generation workflows
- `assets/images/` — general static images for public HTTPS delivery
- `assets/json/` — JSON payloads or configuration files intended for public fetch
- `files/` — downloadable files such as PDFs, docs, and other hosted artifacts

## Legacy content

Older root-level files are being retained in place for legacy URL compatibility. They should not be treated as the active publishing structure for new app uploads.

## Publishing rule

New app-managed assets should be written only into the active directories above so that public URLs remain predictable.
