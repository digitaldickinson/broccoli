# Broccoli - journalism mindmapper
<img width="400" height="261" alt="Screenshot 2026-01-30 at 12 13 48" src="https://github.com/user-attachments/assets/8be9eef2-f30e-4570-936e-41705f96aabf" />

A single-page mind-mapping app for journalism students. Break a big project into manageable chunks, then export a structured Word document to use as the backbone of your write-up or reflection.

Live demo (with sample data): https://journalism.cards/broccoli/

## Features

### Node types
Seven node types, each tailored to journalism workflows:

| Node | Purpose |
|---|---|
| **Section Heading** | Top-level grouping. Requires a "Lesson learned" before export. |
| **Source** | A person, document, or dataset you've drawn on. |
| **Reading / Research** | Academic or background reading, with a Harvard reference field and key takeaway. |
| **Contact** | A person with role, email, phone, and website fields. |
| **Industry Example** | A real-world case study or comparable story. |
| **Task** | A checklist of to-do items with tick-off support. |
| **Free Text** | General notes that don't fit another type. |

### Canvas
- **Pan** — click and drag the background
- **Zoom** — scroll wheel, or the +/− buttons (bottom-right), or ↑ / ↓ arrow keys
- **Move nodes** — drag any node; use arrow keys for fine-grained nudging (hold Shift for larger steps)
- **Reset view** — press `Z`

### Editing
- Select a node to open its editor in the sidebar
- **Relink a node** — click the dashed line connecting it, then click its new parent node
- **Outline view** — toggle the list icon in the toolbar to see a structured outline of the whole map

### Saving and loading
- Work is **auto-saved to your browser** after every change — safe to close and return later
- **Save** — downloads a `.json` project file for backup or sharing
- **Load** — opens a previously saved `.json` file
- **New map** — clears the canvas (prompts for confirmation first)
- **Undo / Redo** — up to 20 steps (toolbar buttons or Ctrl/Cmd+Z / Ctrl/Cmd+Shift+Z)

### Word export
The Export button is locked until every Section Heading has a "Lesson learned" filled in (the numbered badge turns green when ready). The exported `.doc` file contains:
- Each section with its lesson learned, followed by all its child nodes in hierarchy order
- A **Contacts Directory** listing all Contact nodes (alphabetical)
- A **Reference List** of all Harvard references from Reading nodes (alphabetical)

### Keyboard shortcuts

| Key | Action |
|---|---|
| `H` | Add Section Heading (from centre node) |
| `S` | Add Source (under selected node) |
| `R` | Add Reading/Research (under selected node) |
| `C` | Add Contact (under selected node) |
| `D` | Add Task (under selected node) |
| `E` | Add Industry Example (under selected node) |
| `T` | Add Free Text (under selected node) |
| `Z` | Reset canvas view |
| `↑ / ↓` | Zoom in / out (when no node is selected) |
| `Arrow keys` | Nudge selected node (hold Shift for larger steps) |
| `Backspace / Delete` | Delete selected node (and its children) |
| `Ctrl/Cmd+Z` | Undo |
| `Ctrl/Cmd+Shift+Z` | Redo |
| `Escape` | Cancel relink mode |

## Getting started

Open `broccoli.html` in any modern browser — no installation or internet connection required. To try it out with real data, load `Broccoli_Map_30-01-2026.json` using the Load button in the toolbar.

## Deployment

The entire app is a single HTML file with no local dependencies. It loads React, Tailwind CSS, and Lucide icons from CDNs, so it works anywhere a browser can open a file — including inside a VLE.

## Notes

- Mobile experience has some rough edges.
- The app uses your browser's localStorage for auto-save, so clearing site data will erase unsaved work. Use the Save button to keep a local backup.

## Credits

Based on an idea by Dr Liz Hannaford. The principle: a whole head of broccoli looks like hard work; cut it into florets and suddenly those healthy habits seem manageable. Same idea applies to big journalism projects.

Broccoli was coded, in part, using AI.
