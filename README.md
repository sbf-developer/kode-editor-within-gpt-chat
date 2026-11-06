# Side code editor for ChatGPT practice

A self-contained code editor for writing answers while discussing programming with ChatGPT.

## Open the editor

1. Open [CS50_Editor.html](CS50_Editor.html) and download the raw file.
2. Open the downloaded file in Chrome or another modern browser.
3. Put its window beside your ChatGPT conversation.
4. Write your answer, choose **Copy answer**, and paste the code into the chat.

Everything the editor needs is bundled in the HTML file. No installation, build, account, or internet connection is required after downloading it.

**Copy answer copies source code as plain text**, without line numbers or screenshots. If automatic clipboard access is blocked, the editor offers a text-selection fallback.

## Reuse in another ChatGPT conversation

Share this repository and say:

> Use the code editor from https://github.com/sbf-developer/side-code-editor-within-gpt-chat for our practice. Give me one small coding problem at a time. Let me answer with code, pseudocode, or a mix, then review my attempt. Keep the solution hidden until I ask for it.

Ask ChatGPT to retrieve `CS50_Editor.html` from this repository or attach your downloaded copy. Interactive previews depend on the ChatGPT interface. This file does not install a native ChatGPT sidebar or enable Canvas; opening it in a separate browser window works independently of those features.

The editor cannot see the conversation, and ChatGPT cannot see unsent edits. Use **Copy answer** to share an attempt.

## Features

- CodeMirror editing with syntax highlighting and line numbers.
- C, Python, SQL, JavaScript, and plain text/pseudocode modes.
- Tab/Shift+Tab indentation, automatic indentation, bracket pairing and matching.
- Undo/redo, find/replace, and comment shortcuts.
- Dark/light themes and adjustable text size.
- Local browser draft saving, where browser storage is available.
- Open a source file and download your code using **Save code**.

The editor edits text; it does not compile or run programs. The bundled example is the vowel-counting exercise from our CS50 practice.

## Useful shortcuts

| Action | Shortcut |
| --- | --- |
| Indent / outdent | Tab / Shift+Tab |
| Undo / redo | Ctrl+Z / Ctrl+Shift+Z |
| Find / replace | Ctrl+F / Ctrl+H |
| Toggle comment | Ctrl+/ |
| Save source code | Ctrl+S |
| Select all code | Ctrl+A |
| Leave editor input | Esc |

On Mac, the editor also provides Command-key equivalents. Browser or OS shortcuts may take precedence.

Drafts are local to the browser and file location. Use **Save code** to keep a separate copy before moving the editor or clearing browser data.

## Files and maintenance

- `CS50_Editor.html`: complete offline editor, styles, scripts, and bundled dependencies.
- `AGENTS.md`: instructions for assistants reusing or maintaining the editor.

CodeMirror 5.65.16 is included under the MIT license. Its copyright and complete license notice are embedded in the HTML source.
