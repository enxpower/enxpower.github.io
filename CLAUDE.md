# CLAUDE.md

## Project

This repository is the official public AGI&M Assets Inc. website served from `agim.ca`.

## Operating Context

This repository belongs to AGI&M Assets Inc., a Canadian holding company that owns and develops energy infrastructure, power equipment, and autonomous industrial systems businesses across North America.

## Current Purpose

The current practical purpose is to publish a lightweight static corporate website at `agim.ca` with clear holding-company positioning, public metadata, responsive layout, and links to related businesses and documents.

## Architecture

The repository is a static HTML website.

Known structure from inspection:

- `index.html` is the public website entry point.
- `CNAME` points the site to `agim.ca`.
- `index.html` contains canonical URL metadata, favicon reference, Open Graph metadata, Twitter card metadata, and JSON-LD Organization data.
- No root `README.md` was found during inspection.
- No root `package.json` was found during inspection.

Deployment is likely GitHub Pages because the repository contains a root `CNAME`, but Pages settings were not verified.

## Brand / UI Rules

This repository contains public HTML and corporate pages. Apply these rules to every public page change:

- Desktop, tablet, and mobile layouts must be precisely responsive.
- Every release must be checked for responsive layout before publishing.
- Horizontal scrolling must be prevented on all screen sizes.
- Every public HTML page must include proper social preview metadata.
- Every public HTML page must include a strongly relevant title, description, favicon, and preview image.
- PNG preview images are preferred over SVG when social sharing compatibility matters.
- Use the correct company VI based on the brand involved.
- If no company brand applies, use Andy Gong / GONG-VI.
- Do not use dark color schemes unless the repository's VI explicitly requires it.
- Do not expose private source, credentials, or internal logic in public pages.
- All code, comments, filenames, and UI copy must be English.

For AGI&M repositories:

- Use AGI&M VI.
- Keep the tone serious, institutional, execution-oriented, and infrastructure-grade.
- Avoid generic startup styling.
- Avoid playful or consumer-app visuals.
- Use clean hierarchy, credible business language, and restrained visual treatment.

## Hard Rules

- Do not modify unrelated files.
- Do not add dependencies unless explicitly approved.
- Do not change deployment structure unless explicitly approved.
- Do not change public routes unless explicitly approved.
- Do not commit credentials, tokens, API keys, OAuth secrets, private keys, or environment variable values.
- Do not put secrets in frontend HTML or public JavaScript.
- Keep changes minimal, purposeful, and reversible.
- All generated repository content must be English-only.
- Update docs/todo-next.md at the end of every coding session.

## Session Handoff Rule

Every coding session must end by updating:

- docs/decision-log.md if a decision changed
- docs/change-log.md if files changed
- docs/todo-next.md with exact next steps

If docs/change-log.md does not exist and files were changed, create it.
