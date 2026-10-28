# NaturaSì RELEX Category Suite
**Control Tower & Calculation Engine for Inventory Optimization**
*Release: V1.5.10 BETA*

## 📋 Overview
The RELEX Category Suite is a specialized, web-based Control Tower and calculation engine designed for the NaturaSì Grocery Business Unit. It bridges the gap between Central Headquarters' inventory optimization goals and the Store Managers' visual merchandising needs.

By processing raw Excel data, the suite mathematically converts real sales data, product dimensions, and supply chain constraints into perfectly calibrated ordering parameters (Presentation Minimums and Shelf Maximums) ready to be imported into RELEX Plain.

## 🚀 Key Features (V1.5.10 BETA)
- **Advanced Algorithmic Replenishment:** Dynamically calculates optimal shelf parameters based on weekly sales, delivery schedules (including Sunday buffers), and physical packaging matrices.
- **Glassmorphism UI:** Redesigned sticky headers with high-transparency blur effects and frosted glass secondary buttons for a macOS-like experience.
- **Dynamic Color Paradigm:** Introduction of "Life" (Emerald Green) and "Death" (Coral Red) variables for intuitive status identification across Light/Dark modes.
- **Dark Mode CSS Fixes:** Resolved inline style overrides on alert modal footers and button contrasts in dark theme mode.
- **Smart Filtering:** Dynamic "Invert Selection" capability in filter popups and contextual search placeholders.
- **Excel-like UI/UX:** Data grid supporting column drag-selection, multi-sort, filtering, native Excel export (View vs. Full Tab), and quick row-copy via right-click.
- **Assortment Diagnostics (Diag):** Automatically audits the store's inventory to flag anomalies such as dead stock, negative inventory, or missing "Must Have" products.
- **Interactive Changelog:** Direct access to the evolutionary version history directly from the main header.
- **Phase-Out Capping Protocol:** Enhanced logic for Status 20 products (Pre-Eliminated) to apply logistical capping (Max = Case Pack) instead of complete delisting if the product is still active.

## 🛠️ Tech Stack
- **Frontend:** Pure HTML5, CSS3, Vanilla JavaScript (ES6+).
- **Data Processing:** SheetJS for client-side .xlsx parsing and exporting.
- **Architecture:** 100% Client-side. Privacy-first by design (data never leaves the browser).

## 📄 License
This software is proprietary. All rights reserved.
For more information on usage restrictions, please see the [LICENSE.md](LICENSE.md) file.

---
*Ideated, architected, and engineered by **Massimo Maggipinto**.*
