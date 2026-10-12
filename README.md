# ShopEase – Responsive Store Landing Page

A simple, responsive landing page for an online store, built with **HTML and CSS only**.

## How to run it
1. Keep `index.html`, `style.css` and the `images` folder in the same folder.
2. Double-click `index.html` to open it in a browser.
3. To see the mobile layout, make the browser window narrow, or open
   DevTools (right-click > Inspect) and click the device toolbar icon.

## Files
| File / folder   | What it is                                        |
|-----------------|---------------------------------------------------|
| `index.html`    | Page structure: header, hero, products, about, footer |
| `style.css`     | All styling, including the media queries           |
| `images/`       | Four placeholder product images (SVG)              |
| `screenshots/`  | `desktop.png` and `mobile.png`                     |

## Design choices
- **Colour scheme:** one bright accent colour (orange) for buttons, prices and the
  logo, against dark grey and white. A single accent keeps the page clean and draws
  the eye to the "Shop Now" buttons. All colours are stored as CSS variables in
  `:root`, so the theme can be changed in one place.
- **Sticky header:** the logo and navigation menu stay at the top while scrolling.
  The menu links jump to each section (`#home`, `#products`, `#about`, `#contact`)
  with smooth scrolling.
- **Hero banner:** a gradient background gives a bold first impression without
  needing a large image file.
- **Product cards:** white cards with rounded corners and a soft shadow. Each card
  has an image, name, short description, price and a "Shop Now" button. Cards lift
  slightly on hover to feel interactive.
- **Layout tools:** CSS Grid for the product cards, and Flexbox for the header,
  feature boxes and footer columns.
- **Responsive design (media queries):**
  - Desktop (above 992px): 4 product cards per row.
  - Tablet (992px and below): 2 cards per row, smaller hero heading.
  - Mobile (600px and below): 1 card per row, the header stacks the logo above
    the menu, and the feature boxes and footer columns stack vertically.
- **Simplicity:** no frameworks or JavaScript. The images are lightweight SVG files,
  so the page loads quickly and works offline.

## Testing
Tested at 1366px (desktop laptop) and 390px (phone) widths; see the `screenshots` folder.
