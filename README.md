# Cafe Mania — Website

A small responsive cafe website

## Pages
- `index.html` — home page (hero + guest favorites)
- `menu.html` — menu with category sidebar
- `about.html` — our story, team, atmosphere gallery, hours
- `cart.html` — shopping cart
- `checkout.html` — checkout form
- `responsive.html` — Assignment 3 Part 1 demo (media queries only, no Bootstrap)
- `confirmation.html` — order confirmation

## JavaScript responsibilities

- `script.js`: existing FAQ accordion, contact popup, toast, theme cycle and clock.
- `js/catalog.js`: catalog data, money formatting and safe element creation.
- `js/cart.js`: cart state, calculations, storage validation and demo order snapshot.
- `js/site-ui.js`: badges, keyboard navigation, sound preference and modal focus handling.
- `js/shop.js`: menu/favorites rendering, filters and cart controls.
- `js/checkout.js`: field validation, callbacks, step state and order review.
- `js/confirmation.js`: actual order summary and local rating.


## Assignment 2 (Flexbox & Grid) — where each task lives
- **Task 1, Flexbox navbar:** `#main-header .topbar` on every page (logo left, links right).
- **Task 2, Flexbox card row:** `.card-grid` on `index.html` — equal-height cards with a lift/shadow hover effect.
- **Task 3, Grid Areas layout:** `.menu-layout` on `menu.html` — `grid-template-areas` with header / sidebar / main / footer, sidebar holds category filters + kitchen hours.
- **Task 4, Image gallery:** `.gallery-grid` on `about.html` — 9-photo grid with a caption overlay on hover.

## Assignment 3 (Media Queries + Bootstrap) — where each task lives
- **Task 1, responsive typography:** media queries at 576px / 992px at the end of `css/style.css` (`h1`–`h3`, body text).
- **Task 2, card group (no Bootstrap):** `.mq-cards` in `css/media-queries.css`, page `responsive.html` — 3 / 2 / 1 cards per row.
- **Task 3, grid:** `container` + `row` / `col-*` on every page (hero `col-lg-6`, cards `col-lg-4` via `row-cols-lg-3`, cart/checkout `col-lg-8` + `col-lg-4`, menu sidebar `col-lg-3` + `col-lg-9`).
- **Task 4, spacing:** `m-*`, `p-*`, `gap-*` utilities, with responsive ones such as `mt-lg-4`, `pt-md-5`, `p-sm-4`.
- **Task 5, navbar:** `navbar navbar-expand-md` with `navbar-toggler` on every page (4 links: Home, Menu, About, Cart).
- **Task 6, buttons:** `btn-primary`, `btn-secondary`, `btn-outline-primary`, `btn-lg`, `btn-sm`; `btn-group` for the collection method in `cart.html`.
- **Task 7, carousel:** 9 slides with indicators and controls in `about.html`.
- **Task 8, cards:** Bootstrap `card` in a `row-cols-*` grid on `index.html` and `menu.html` (`card-deck` no longer exists in Bootstrap 5).
- **Task 9, form:** `form-control`, `form-select`, `input-group`, `form-check` in `checkout.html`.
- **Task 10, accessibility:** semantic `<nav>`, `<button>`, labels, `aria-*`, alt texts, `visually-hidden` control labels.

## Assignment 5 — Part 1
Cafe Mania now has a connected menu → cart → three-step checkout → confirmation flow.

## Assignment 6 — jQuery
The jQuery library is loaded on every page before `js/assignment6.js`.

| Task | Where to see it |
| :--- | :--- |
| Setup | `js/assignment6.js` logs “jQuery is ready!” when the page loads. |
| 1. Live filtering | `menu.html` search field filters the current category while typing. |
| 2. Autocomplete | Matching menu items appear under the search field; choose one to filter. |
| 3. Search highlighting | Matching words are marked in visible product names and descriptions. |
| 4. Scroll progress | A slim progress bar at the top of every page follows scrolling. |
| 5. Animated counter | `index.html` counts up to the real menu and category totals. |
| 6. Submit spinner | Contact and checkout submit buttons show “Please wait...” and disable briefly. |
| 7. Toast notifications | Existing toast announces cart updates, contact submission, and copy feedback. |
| 8. Copy to clipboard | `index.html` has a button to copy the menu URL. |
| 9. Lazy loading | Images use `data-lazy-src`; jQuery assigns `src` when they approach the viewport. |

Open `index.html` in a browser with internet access so the CDN-hosted jQuery and Bootstrap files can load.

### requirement

| Requirement | Implementation |
| :--- | :--- |
| Select and modify DOM elements | `js/shop.js`: `productCard`, product grid, cart rows;<br>`js/checkout.js`: summaries |
| Manipulating attributes (chosen option: rating stars) | `js/confirmation.js`: `renderRating`, `querySelectorAll`, classes and `aria-pressed` |
| Click event listeners | `js/shop.js`: add/remove/quantity buttons and category filters |
| Keyboard events | `js/site-ui.js`: navigation `keydown` handler |
| Callbacks (chosen option: multi-step form) | `js/checkout.js`: `changeStep(index, onStepChange)` invokes the `renderStep` callback |
| Switch statement | `js/shop.js`: `productsFor(category)` (Filter All, Coffee, Breakfast, Bakery, Lunch and Tea) |
| Objects and methods | `js/catalog.js`: product objects;<br>`js/cart.js`: cart object with `add`, `remove`, `setQuantity`, `subtotal`, `total` |
| Arrays and loops | `js/catalog.js`: products;<br>`js/shop.js`: `for…of` card/row rendering |


## Team
Aidos, Arnur, Mukhammajon.


