EconomyShopGUI Price Calculator Configurator is A web-based tool for Minecraft server administrators using the EconomyShopGUI plugin.
-SIMPLE CONFIG
<img width="1050" height="1480" alt="IMG_20260911_073121" src="https://github.com/user-attachments/assets/6ff74ceb-da94-4687-8a57-83965ee6fa54" />
-ADVANCED CONFING CRAFTABLE ITEMS USING THE BASE ITEM CALCULATOR
<img width="1058" height="1472" alt="IMG_20260911_073111" src="https://github.com/user-attachments/assets/1473e570-473d-4be7-8407-549cbf537b25" />
-GLOBAL SETTINGS
<img width="490" height="784" alt="IMG_20260911_073052" src="https://github.com/user-attachments/assets/4332497e-f2d9-485d-9cbd-0b94122c0419" />



Everything runs directly in the browser. No installation, no backend, no build step.

# EconomyShopGUI Calculator — Feature List

## 1. Core Purpose
- Browser-based tool (single HTML file, no install, no backend) that generates ready-to-use `.yml` shop configuration files for the **EconomyShopGUI** Minecraft plugin.
- Two independent workflows: **Simple Config** (manual pricing) and **Advanced Config** (automatic crafting-based pricing).

## 2. Minecraft Version & Item Data
- Fetches real item and recipe data for any Minecraft version from the PrismarineJS `minecraft-data` dataset.
- Version picker with search; automatic fallback chain if a version's data isn't available, with a visible banner.
- Caches the version list locally for 24h to avoid repeated network calls.

## 3. Simple Config Tab
- Live search across all items for the selected Minecraft version; click to add.
- Per-item fields: display name, buy price, sell on/off toggle.
- Multiple shop **pages**, each with its own configurable GUI row count (1–6).
- Bulk actions: multi-select rows, bulk delete, bulk price multiply.
- Bulk text paste (add many items at once from pasted text).
- Drag-and-drop row reordering.
- Category auto-detection/filtering (ores, food, wood, etc.).
- Live validation warnings (e.g., sell price higher than buy price).
- Live YAML preview (current page or full file).

## 4. Advanced Config Tab (automatic price calculator)
- Define **base resources** (e.g., raw ores) with manual prices.
- **Recursive crafting-cost engine**: walks the real recipe graph and computes the cheapest achievable price for every item craftable — directly or through multiple recipe tiers — from those base resources.
- Results land in a **review pool** where you can:
  - Filter, sort (by name, price, category, source), and search
  - See each item's source (Base / Recipe / Raw) and category
  - Manually override a computed price — the override now correctly propagates into any other item crafted from it, with a visual "edited" tag and a one-click reset back to the computed value
  - Bulk-select items to push into shop pages, bulk-multiply, bulk-remove
- Recalculating after changing a base price properly refreshes all downstream prices.
- Same multi-page / GUI-rows / drag-reorder support as Simple Config.

## 5. Global Pricing Controls
- Global **buy modifier** and **sell modifier** multipliers applied on top of every item's base price, with live preview of the final numbers.

## 6. Import / Export
- Export the current page or the full config as a valid EconomyShopGUI `.yml` file.
- Import an existing shop `.yml` (robust YAML parsing handles real-world files regardless of key order or formatting).
- Import/export base-resource price lists separately.
- Copy-to-clipboard and file-download options.

## 7. Presets
- Ready-made starter packs (Ores & Ingots, Wood & Building, Food & Farming, Mob Drops) to quickly seed base resources or item lists.

## 8. Editing Safety & Convenience
- Full **undo/redo** history.
- Confirmation dialogs (styled, in-app — not disruptive browser popups) before destructive actions (clear items, delete page, bulk delete).
- Automatic local persistence — all work is saved to the browser and restored on next visit, with a warning if the browser's storage is full.
- Keyboard navigation (arrow keys + Enter) in the item search dropdowns.

## 9. Interface
- Light/dark theme toggle (defaults to your system preference on first visit).
- Icon previews for every Minecraft item, with a graceful fallback if an icon fails to load.
- Mobile-friendly responsive layout.
- Screen-reader-friendly labels and live status announcements.

## 10. Danger Zone
- One-click "wipe everything" option to reset all locally stored data.

📄 License
Free to use and modify.
