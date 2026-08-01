# Course Flowchart Builder

_by Shreyas Tayal_

An interactive, browser-based tool for mapping out university course prerequisites — built to plan which optional courses to take now based on what they unlock later.

🔗 **Live tool:** `https://shreyas-tayal.github.io/Course_Flowchart_Builder/`

## What it does

- Add courses as **nodes** and connect them with **arrows** showing prerequisite relationships
- **Quick-add** a course along with its prerequisite(s) in one step
- **Move mode** — drag nodes around to organize the layout
- **Delete mode** — click any node or arrow to remove it
- **Code view** — bulk add/edit connections as plain text (similar to Mermaid), instead of clicking through forms one at a time
- **Save / Load** — export your flowchart as a file and load it back in later
- **Export** the finished diagram as an SVG or PNG image

## How to use

1. Open the live link above (or open `index.html` directly in any browser — no install needed)
2. Add nodes and arrows using the side panel, or paste a list into Code view
3. Drag nodes into a layout that makes sense to you
4. Download the result as an image, or save the file to keep editing later

## Repo structure

```
├── index.html      # the flowchart tool (open this)
├── Y2/             # Year 2 flowchart — PNG, SVG, and JSON save file
├── Y3/             # Year 3 flowchart — PNG, SVG, and JSON save file
└── combined/       # combined Y2 + Y3 flowchart — PNG, SVG, and JSON save file
```

Each folder holds the exported outputs for that flowchart:
- **`.png`** / **`.svg`** — image snapshots of the diagram
- **`.json`** — the save file, which can be loaded back into the tool to keep editing

The `Y2`, `Y3`, and `combined` folders are personal course-planning material for this repo owner's own university — not required for the tool itself to run.

## Running locally

No build step or dependencies required. Just clone the repo and open `index.html` in a browser:

```
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
open index.html
```