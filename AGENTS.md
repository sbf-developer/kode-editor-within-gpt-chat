# Instructions for assistants

## Purpose

This repository stores Kode, the reusable offline editor in `Kode.html`.
Read `README.md` before helping a user reuse it.

## Reusing Kode in ChatGPT

- Retrieve the existing `Kode.html`; preserve the CodeMirror editor and multi-file workspace instead of replacing them with a basic textarea.
- Offer a downloadable HTML file or an interactive preview when the interface supports one.
- Do not claim Kode installs a native ChatGPT sidebar, opens Canvas, or grants access to unsent editor content.
- A separate browser window beside the chat is the independent workflow.
- **Copy answer** must copy only the active file's source text. Never substitute a screenshot, rendered editor page, line numbers, or the HTML implementation itself.
- During requested coding practice, give one small problem at a time and accept code, pseudocode, or a mix. Review submitted attempts; do not fill in solutions unless requested.
- Preserve all files and current attempts when updating a workspace. Use an unimplemented starter when starting a new exercise.

## Maintenance

- Name the product Kode and its downloadable file `Kode.html`.
- Keep it self-contained and usable offline.
- Preserve file creation, tabs, switching, renaming, deletion confirmation, recovery of the latest deletion, and local workspace saving.
- Keep each file's content, syntax mode, selection, and undo history independent during the session.
- Do not silently overwrite existing files when importing or renaming.
- Keep clipboard fallbacks, keyboard editing, language selection, and the embedded CodeMirror copyright and MIT license.
- Do not add an Exercise button or the removed tagline.
- Avoid publishing private workspace drafts or browser storage.
- Verify JavaScript syntax after code changes. Verify affected interactions when a browser is available, including persistence and copying plain source text.
- Keep claims accurate: syntax highlighting is not compilation or code execution.
