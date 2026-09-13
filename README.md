# Smart Time Table

A static class-schedule display page, plus a standalone PDF-renaming utility.

## Live demo

https://2bca27.pages.dev

## Overview

This repository contains two independent, self-contained HTML tools:

- **`index.html`** — a class timetable page ("Time Table 1st Year") that shows the current and upcoming class based on a hardcoded weekly schedule, with day/night theming and a per-day schedule viewer.
- **`pdf-renamer.html`** — a standalone, client-side PDF renaming tool (built with `pdf-lib`) that lets you rename and re-download a PDF file entirely in the browser, with no server involved.

Both are plain static HTML/CSS/JavaScript pages with no build step and no backend.

## Features

**`index.html`:**
- Shows the current class and the next upcoming class based on the time of day.
- A per-day schedule viewer covering Monday through Friday.
- An announcements section.
- Day/night theming.

**`pdf-renamer.html`:**
- Rename a PDF file and download the renamed copy, entirely client-side.
- Day/night theming, consistent with `index.html`.

## Tech stack

HTML, CSS, and vanilla JavaScript. `pdf-renamer.html` additionally uses the [pdf-lib](https://pdf-lib.js.org/) library, loaded from a CDN.

## Setup

```bash
git clone https://github.com/D-Majumder/Smart-Time-Table.git
cd Smart-Time-Table
```

Open `index.html` or `pdf-renamer.html` directly in a browser, or serve the folder with any static file server.

**Note:** the weekly schedule shown in `index.html` is hardcoded in the page's JavaScript — editing it means updating the schedule data directly in the file.

## License

This project is licensed under the **GNU General Public License v3.0**. See [LICENSE](./LICENSE) for the full text.
