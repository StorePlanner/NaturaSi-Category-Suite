# NaturaSì RELEX Category Suite
**Control Tower & Calculation Engine for Inventory Optimization**

## 📋 Overview
The RELEX Category Suite is a specialized, web-based Control Tower and calculation engine designed for the NaturaSì Grocery Business Unit. It bridges the gap between Central Headquarters' inventory optimization goals and the Store Managers' visual merchandising needs.

By processing raw Excel data, the suite mathematically converts real sales data, product dimensions, and supply chain constraints into perfectly calibrated ordering parameters (Presentation Minimums and Shelf Maximums) ready to be imported into RELEX Plain.

## 🚀 Key Features
- **Advanced Algorithmic Replenishment:** Dynamically calculates optimal shelf parameters based on weekly sales, delivery schedules (including Sunday buffers), and physical packaging matrices.
- **Assortment Diagnostics (Diag):** Automatically audits the store's inventory to flag anomalies such as dead stock, negative inventory, or missing "Must Have" products.
- **Delisting & Run-Out Management (Delist):** Identifies slow-moving or discontinued items and applies "Capital Protection" rules.
- **Opportunity Gap (Opp):** Scans the database to suggest new sub-category top-performers or mandatory items.
- **Booster Strategies:** Features toggleable global modifiers (High-Volume, Deep, Deep & Length).
- **Store Label Generator:** Instantly generates formatted .TXT files for shelf label printing systems (Frontalini).
- **Excel-like UI/UX:** Data grid supporting column drag-selection, multi-sort, filtering, and native Excel export.
- **Dynamic Dark Mode:** Adapts to OS/Browser theme preferences with manual override.

## 🛠️ Tech Stack
- **Frontend:** Pure HTML5, CSS3, Vanilla JavaScript (ES6+).
- **Data Processing:** SheetJS for client-side .xlsx parsing and exporting.
- **Architecture:** 100% Client-side. Privacy-first by design (data never leaves the browser).

## 📄 License
This software is proprietary. All rights reserved.
For more information on usage restrictions, please see the [LICENSE.md](LICENSE.md) file.

---
*Ideated, architected, and engineered by **Massimo Maggipinto**.*