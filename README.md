EconomyShopGUI Price Calculator
A web-based tool for Minecraft server administrators using the EconomyShopGUI plugin. It lets you build, edit, and export shops.yml configuration files visually — no manual YAML editing required.

Everything runs directly in the browser. No installation, no backend, no build step.

✨ Features
🧩 Simple Config
Add items one by one via search

Set buy and sell prices per item

Edit display names inline

Drag & drop to reorder

Bulk actions: multiply, duplicate, delete, auto-sell

Multi-page support (page1, page2, ...)

Live YAML preview (per page or full file)

🧪 Advanced Config
Define prices for base resources (e.g. cobblestone = 1)

The calculator walks all crafting recipes and computes prices for every craftable item automatically

Edit any computed price manually

Manually-added base resources are marked with → for easy identification

Select items and push them to the current page with one click

⚙ Global Settings
Minecraft Version – auto-loaded from minecraft-data, always up to date (26.1, 1.21.11, 1.21.10, ...)

Buy Modifier – multiplier applied to all buy prices at export

Sell Modifier – multiplier applied to all sell prices at export (e.g. 0.25 = sell is 4× lower than buy)

Live formula preview showing exactly how prices are computed

Danger Zone – wipe all data with one click (permanent)

📥 Import / Export
Import existing shops.yml files directly

Paste base resources in bulk

Export always includes all pages of the file

Copy the full YAML to clipboard

📦 Presets
Pre-made packs with hundreds of items already configured with balanced buy/sell prices:

Preset	Items	Source
Ores	18	Ores.yml
Blocks	81	Blocks.yml
Brewing	18	Brewing.yml
Colour	85	Colour.yml
Drops	10	Drops.yml
Farming	35	Farming.yml
Misc	23	Misc.yml
Redstone	11	Redstone.yml
Items with sell: -1 in the source are automatically imported as not sellable.

🎨 Interface
Dark / Light theme toggle

Responsive layout

Item icons from minecraftitemids.com

Live validation warnings (e.g. sell > buy)

Undo / Redo (Ctrl+Z / Ctrl+Y)

Keyboard shortcuts and command palette

🚀 How to Use
Download the calculator.html file.

Open it in any modern browser (Chrome, Edge, Firefox).

Pick a Minecraft version from ⚙ Global Settings.

Add items manually in Simple Config — or define base resources and let Advanced Config compute everything.

Export the .yml file and drop it into your server's plugins/EconomyShopGUI/shops/ folder.

🛠 Built With
Plain HTML, CSS, and JavaScript — no frameworks, no dependencies.

Official item and recipe data from minecraft-data (PrismarineJS).

Item icons rendered from minecraftitemids.com.

✅ Why Use It
No more YAML errors — the tool generates clean, valid EconomyShopGUI files.

Consistent pricing — apply a single buy/sell modifier across all items.

Automatic recipe math — no need to manually compute crafting costs.

Fast iteration — presets, bulk actions, and import/export make shop creation a matter of minutes.

📄 License
Free to use and modify.
