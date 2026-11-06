# Kode

A self-contained code editor for working beside a ChatGPT conversation.

## Open Kode

1. Download [Kode.html](Kode.html) using GitHub's raw-file download.
2. Open it in Chrome or another modern browser.
3. Put its window beside your ChatGPT conversation.
4. Write your code, select **Copy answer**, and paste it into the chat.

Everything is bundled in the HTML file. No installation, build, account, or internet connection is required after downloading.

**Copy answer copies the active file's source as plain text**, without line numbers or screenshots. If automatic clipboard access is blocked, Kode provides a text-selection fallback.

## Files and tabs

- **New file** creates a blank file and opens its own editor tab.
- Switch files using the tabs or the file list.
- **Rename** changes the active file's name. Recognized extensions select its syntax mode.
- **Delete** removes the active file after confirmation.
- **Restore deleted** recovers the most recently deleted file, including its code. Only the latest deletion is retained.
- **Open** imports one or more source files into separate tabs. Existing files are preserved; duplicate imported names receive a number.
- **Save code** downloads the active file as a plain-text source file with its current name.

Each file has its own code, language, cursor position, and undo history while Kode stays open. File contents, names, language modes, the active tab, and the most recently deleted file are saved in browser storage when available. Undo history is retained during the session, not across reloads.

The last file can be deleted; Kode then opens a blank file so the workspace remains usable.

Names must be unique within the workspace and cannot contain slashes. Changing a language mode updates the active file's extension without overwriting another file.

## Reuse in another ChatGPT conversation

Share this repository and say:

> Use Kode from https://github.com/sbf-developer/side-code-editor-within-gpt-chat as my code editor. Retrieve Kode.html so I can reuse it beside this conversation.

For practice, you can add:

> Give me one small coding problem at a time. Let me answer with code, pseudocode, or a mix, then review my attempt. Keep the solution hidden until I ask.

Interactive previews depend on the ChatGPT interface. Kode does not install a native ChatGPT sidebar or enable Canvas. Opening it in a separate browser window works independently of those features.

Kode cannot see the conversation, and ChatGPT cannot see unsent edits. Copy your answer into the chat to share it.

## Editor features

- CodeMirror syntax highlighting and line numbers.
- C, Python, SQL, JavaScript, and plain text/pseudocode modes.
- Tab/Shift+Tab indentation, automatic indentation, bracket pairing and matching.
- Independent file tabs, undo/redo, find/replace, and comment shortcuts.
- Dark/light themes and adjustable text size.
- Offline use and browser-local workspace saving.

Kode edits text; it does not compile or run programs.

## Shortcuts

| Action | Shortcut |
| --- | --- |
| Indent / outdent | Tab / Shift+Tab |
| Undo / redo | Ctrl+Z / Ctrl+Shift+Z |
| Find / replace | Ctrl+F / Ctrl+H |
| Toggle comment | Ctrl+/ |
| Save active source file | Ctrl+S |
| Select all code | Ctrl+A |
| Leave editor input | Esc |
| Switch focused file tabs | Left / right arrow |

Command-key equivalents are provided on Mac. Browser or OS shortcuts may take precedence.

## Keeping your work

Workspace drafts stay in your browser and are not uploaded. Use **Save code** for each file to keep independent copies, especially before moving or renaming the downloaded HTML, changing browsers, or clearing browser data.

When old and new versions can access the same browser storage, Kode imports the previous single-file editor's saved draft on first use. If you downloaded the new version to another location and your draft does not appear, save your code in the old editor and use **Open** in Kode.

## Repository files

- `Kode.html`: complete offline editor with all styles, scripts, and dependencies.
- `AGENTS.md`: guidance for assistants reusing or maintaining Kode.

CodeMirror 5.65.16 is bundled under the MIT license. Its copyright and full license notice are embedded in the HTML source.
