# KioskTotem
An HTML code where you could call an item to the cart, and go to chekout. The sold Item could be see in a sheet in Google Sheets

## How open
1. Extract all the file `project_matcha`.
2. Open the `index.html` on browser (Chrome, Firefox ou Edge).
3. Maintain structure the files: the HTML loads `css/styles.css` e `js/app.js`.

## Where modify
- `index.html`: structure of the screens and components HTML.
- `css/styles.css`: colors, fonts, exhausts, sizes, responsive and animations.
- `js/app.js`: behavior of totem, navegation, products, cart, payment and integration with Google Sheets.
- `assets/images/`: file reserved for images externals who you wanna add later.
- `docs/`: documents and notes of the project.

## Common customizations
- **Colors and appearance:** Start with the variables at the beginning of `css/styles.css` (`:root`).
- **Products and prices:** In `js/app.js`, look for the section that defines the products/catalog.
- **Product images:** In the current version, several images are embedded as Base64 inside `js/app.js`. This keeps the project portable, but makes the file larger and less convenient to edit. Be careful not to accidentally delete these blocks.
- **Google Sheets:** In `js/app.js`, look for `GOOGLE_SCRIPT_URL` and replace the example value with your published Apps Script URL.
- **Screen text:** Search for the exact text in `index.html` or `js/app.js`, depending on where it is generated.

## Observations
- **Google Fonts:** Google Fonts still require an internet connection; the main interface works locally, but these fonts may not load when offline.
- **Google Sheets integration:** Requires an internet connection and a valid Google Apps Script URL.
