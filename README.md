# A4 Paper Placement Visualizer

A browser-based A4 layout designer for arranging document elements in millimetres and generating Python code with **ReportLab** or **fpdf2**.

**[Open A4 Placement Studio](https://Heed725.github.io/A4-Paper-Placement-Visualizer/)**

## Features

- Portrait (210 × 297 mm) and landscape A4 pages.
- Add text, boxes, horizontal and vertical lines, tables, image placeholders, and QR placeholders.
- Drag elements, resize with handles, and edit their geometry and styling.
- Margin guides, grid, snapping, zoom controls, and live pointer coordinates.
- ReportLab and fpdf2 code previews, plus editable JSON coordinates.
- Copy generated code, duplicate elements, change stacking order, and undo edits.
- A sample invoice layout and automatic saving in your current browser.

## Use

1. Open the live site or download and open `index.html` in a modern browser.
2. Add elements and place them on the page. Coordinates use millimetres from the top-left corner.
3. Select an element to edit its properties.
4. Choose **ReportLab**, **fpdf2**, or **Coordinates**, then copy the output.
5. Run generated Python code separately with the required Python package installed and any referenced assets available.

Image and QR elements are layout placeholders in the browser. The app generates code; Python does not execute on the website.

## Keyboard shortcuts

| Shortcut | Action |
| --- | --- |
| Arrow keys | Nudge the selected element |
| Shift + arrow keys | Nudge by 10 mm |
| Alt + drag | Temporarily ignore snapping |
| Ctrl / Cmd + D | Duplicate the selected element |
| Ctrl / Cmd + Z | Undo |
| Delete / Backspace | Delete the selected element |
| Escape | Deselect |

## Hosting

This is a static site with no build step. GitHub Pages publishes the repository root on `main`, using `index.html` as the homepage.

Google Fonts provides Schibsted Grotesk and JetBrains Mono when available; system fonts serve as fallbacks. Layout state is stored locally in the browser and is not synced between devices.

`A4-Placement-Studio.md` contains the supplied companion notes.
