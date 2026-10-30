# 灯谜工坊 / Lantern Riddle Workshop

A self-contained, offline-first lantern riddle workshop tool. No external JavaScript, fonts, CDNs, or libraries.

## Running it

Open `index.html` in a modern browser, or visit the GitHub Pages site after publishing. On some iPads, opening an HTML file through the Files preview can display the page without running its buttons; try the hosted website in Safari instead.

## Main functions

- 逐题闯关 and 自选谜题, including large-text presentation mode (放大演示)
- In-app editing of 题号、谜面、谜目、谜底、难度、猜谜方法、提示、注解
- TSV/CSV import with preview; JSON import/export and progress backup
- Difficulty and technique filters; 猜中/猜错/未挑战 tracking and summary

Export a JSON backup regularly. Browser localStorage is device- and browser-specific and may be cleared. Changes made on one device do not synchronize automatically to other devices.

## GitHub Pages

Create a new repository, add `index.html` at the repository root, and enable **Settings → Pages → Deploy from branch → main / (root)**. The URL should then follow `https://<account>.github.io/<repository>/` once deployment succeeds.

## Release status

v0.5: Large-text presenter mode introduced. Safari/iPad interactive testing remains outstanding. Print, keyboard shortcuts and swipe navigation are deferred.
