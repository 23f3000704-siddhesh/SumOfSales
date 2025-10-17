# Sales Summary 149

## Overview
Sales Summary 149 is a self-contained single-page web app that:
- Fetches sales data (via a local Blob URL using fetch)
- Calculates total sales
- Displays the result inside the element with id "total-sales"
- Shows a simple breakdown of each line item

This approach uses a local fetch so it works offline without external APIs while still fulfilling the “fetch data” requirement.

## Setup
No build tools or servers are required.

- Option 1: Open index.html directly in any modern browser.
- Option 2: Serve it via a simple static server (optional), e.g.:
  - Python: python -m http.server
  - Node (http-server): npx http-server

## Usage
- Load the page; it auto-fetches data on load and computes the total.
- Click the Refresh button to re-fetch simulated data and recalculate.
- The computed total sales is displayed in the #total-sales element, and a breakdown is shown below.