# 猜谜乐 · v1.0

随心制作。A self-contained lantern-riddle workshop app; no external libraries, fonts, or network requests.

## Use

Open `index.html` in a browser or visit the GitHub Pages site. On first visit, six supplied demo riddles are preloaded (including one deliberately mixed-language test entry); the app does not independently verify their riddle correctness. Use 逐题闯关 for sequential questions or 自选谜题 for audience choice. 主持 controls support reveals, marking 猜中 / 猜错, progress, and large-text presentation.

## Editing and importing

Use 编辑题库 to add/edit all eight fields: 题号、谜面、谜目、谜底、难度、猜谜方法、提示、注解. Import Excel TSV or CSV through 导入与备份. Check the import preview before replacing or appending.

## Demo restore and backups

Under 导入与备份 → 示范题库, select 恢复六道示范题. This **replaces** all questions, progress and session history after confirmation. Export a JSON backup first if you want to preserve your own changes. Backups include riddles and session data; importing a full backup restores both.

Data is stored in each browser's `localStorage` when available; it is not shared between visitors or devices. Clearing site data can erase it. Regular JSON backups are recommended. Existing v0.5 browser storage is retained by v1.0.

## GitHub Pages

Publish `index.html` in the repository root and enable GitHub Pages: Settings → Pages → Deploy from a branch → main → /(root).

## Limits and test status

No account, cloud database or sync. Keyboard shortcuts, swipe gestures and printing are intentionally deferred. This release's JavaScript syntax and static integrity are checked; test interaction on target browsers before important workshops.

## Customization

All user-facing strings are grouped in the `TEXT` block near the top of the inline script. Edit CSS custom properties in `:root` for colours. The six demo riddles are defined in `const sample`.

## Demo data provenance

The six built-in examples are taken directly from the supplied `灯谜工坊-备份-2026-10-30.json` riddle entries. The app does **not** import the backup’s results/history as default scores. Existing browser-local libraries remain in place on upgrade. To load the new examples in a browser that has already used the app, choose 导入与备份 → 恢复六道示范题 (export your existing library first). The user-supplied hints/notes, including placeholder text, are preserved as supplied.
