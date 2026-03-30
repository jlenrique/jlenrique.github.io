# Gamma asset library

This directory is the structured home for public image assets served to Gamma by stable GitHub Pages URLs.

## Purpose

Use this tree for production image assets that need unique, durable, public URLs.

## Top-level structure

- `shared/` for assets reused across multiple courses or projects
- `courses/` for course-specific assets

## Rules

1. Do not place new production assets in the repository root.
2. Use versioned filenames such as `..._v1.png`, `..._v2.png`.
3. Do not overwrite a file if the existing URL may already be in use.
4. Prefer direct image files such as `.png`, `.jpg`, `.jpeg`, `.webp`, or `.gif`.
5. Keep legacy root-level files in place unless they are deliberately archived later.
