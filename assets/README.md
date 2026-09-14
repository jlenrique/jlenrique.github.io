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

## Size budget

GitHub Pages enforces a **1 GB hard limit** on the total deployed site size. Keep total repository content (excluding `.git/`) well under 1 GB. Recommended operating target is **≤ 700 MB** to leave headroom for new content without risking deployment failures.

When the site approaches the limit the `deploy` job will fail with *"Deployment failed, try again later."* at the `syncing_files` stage. To recover:

1. Prune obsolete storyboard snapshots, staging packs, or large binaries.
2. Verify the content size with `du -sh --exclude=.git .` and confirm it is safely under 1 GB.
3. Push the pruning commit to `main`; the next `pages build and deployment` run will succeed once the content is within budget.
