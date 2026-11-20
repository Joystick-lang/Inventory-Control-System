# Inventory Control System: Hypermarket Branch

A browser-based inventory control tool for a single UAE hypermarket branch, built with illustrative data (100 items) and all costs in AED. It runs entirely in the browser using plain HTML, CSS and JavaScript, with SheetJS for Excel import and export and Chart.js for charts. No server or framework is needed.

## Features
- Upload an .xlsx file with ten required columns, with clear errors for missing or invalid data
- ABC classification by annual usage value (A to 80% cumulative, B to 95%, C the rest)
- Per-item daily demand, EOQ, safety stock (95% service level, z = 1.65) and reorder point
- Red "Order now" or green "OK" flag, with recommended order quantity, order value (AED) and days of cover
- What-if panel to change lead time and demand and watch the flags update instantly
- Dashboard cards and charts: ABC share, and stock versus reorder point
- Search, sort and filter by category, class and status
- Export all results, including calculated columns, to .xlsx

## Code structure
All formulas sit together in one commented section of the script, so each calculation is easy to find and explain.

## Limitations
The data is illustrative. EOQ ignores shelf life, and the safety stock formula assumes normally distributed demand and a fixed lead time.

## Usage
Open the HTML file in a browser, then load the sample data or upload your own file.

Built with AI assistance (Claude).
