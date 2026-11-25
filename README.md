# CSS Multipage Website - Introduction to CSS

## 1. Problem Statement

Build a simple 3-page startup website (Home, About, Contact) with a shared external stylesheet to introduce foundational CSS concepts. The site uses **flexbox for layout**, basic color and typography styling, a reusable navigation bar, and a consistent visual theme across all pages. The focus is on learning how CSS selectors, the box model, and flexbox work together to create a clean, structured multipage layout.

---

## 2. Tech Stack

| Category | CSS Concepts |
|----------|-------------|
| **Reset & Box Model** | Universal selector `*`, `margin`, `padding`, `box-sizing: border-box` |
| **Flexbox Layout** | `display: flex`, `flex-direction`, `justify-content`, `align-items`, `flex: 1`, `gap` |
| **Typography** | `font-family`, `font-size`, `font-weight`, `line-height`, `text-align` |
| **Colors** | `color`, `background-color` with hex values (`#1a1a2e`, `#e94560`, `#333`, `#666`) |
| **Spacing** | `margin`, `padding` with px units, `margin: 0 auto` for centering |
| **Sizing** | `max-width`, `width: 100%`, `min-height: 100vh` |
| **Borders & Rounding** | `border`, `border-bottom`, `border-radius` |
| **Links & Buttons** | `text-decoration: none`, `cursor: pointer`, `display: inline-block` |
| **Selectors** | Element selectors (`nav`, `footer`), class selectors (`.card`, `.btn`), descendant selectors (`.nav-links a`), compound selectors (`.nav-links a.active`) |
| **External Stylesheet** | `<link rel="stylesheet" href="style.css">` shared across 3 HTML pages |
| **Form Styling** | `padding`, `border`, `border-radius`, `font-family: inherit` on inputs and textareas |
| **CSS Combinators** | Descendant (`.nav-links a`), child (`.features > .card`), adjacent sibling (`.hero h1 + p`), general sibling (`.contact-info h2 ~ p`) |
| **Transitions** | `transition` on `color`, `background-color`, `transform`, `box-shadow`, `border-color` with `:hover` and `:focus` |
| **Animations** | `@keyframes` (`fadeInUp`, `pulse`), `animation` shorthand, `opacity`, `transform: translateY()` / `scale()`, `infinite` |
| **Media Queries** | `@media (max-width: 768px)` for tablets, `@media (max-width: 480px)` for phones, switching flex rows to columns |

**Total Concepts:** ~15 core CSS properties and patterns focused on layout, typography, and color

---

## 3. Expected Outcomes

1. **Shared Stylesheet:** A single `style.css` file linked from all 3 pages providing a consistent look and feel
2. **Flexbox Navigation:** A horizontal nav bar using `display: flex` with `justify-content: space-between` for brand/links layout and `gap` for link spacing
3. **Active Page Indicator:** The current page link is highlighted with a colored `border-bottom` using a compound class selector (`.nav-links a.active`)
4. **Full-Height Layout:** The body uses `display: flex; flex-direction: column; min-height: 100vh` to push the footer to the bottom
5. **Card Layout:** Feature and value cards use `display: flex` with `flex: 1` for equal-width columns and `gap` for spacing
6. **Contact Form:** A two-column layout using flexbox — form fields stacked vertically on the left, contact info on the right
7. **Centered Content:** Main content area uses `max-width` and `margin: 0 auto` for a readable centered layout
8. **Reusable Button:** A `.btn` class used for both anchor links and form submit buttons with consistent styling
9. **Combinators:** Feature/value cards get a coloured top border via the child combinator, the hero tagline is italic via the adjacent sibling combinator, and contact details get a left accent via the general sibling combinator
10. **Hover & Focus Transitions:** Nav links change colour, the button grows slightly, cards lift with a shadow, and form fields highlight on focus — all smoothly
11. **Animations:** The hero and page headers fade in and slide up on page load; the brand logo pulses continuously
12. **Responsive Layout:** Below 768px, cards and the contact section stack vertically; below 480px, the nav stacks and spacing shrinks

---

## 4. Additional Notes

- **First CSS Project:** Intentionally minimal — no CSS variables or grid. Combinators, transitions, animations and media queries are added in clearly labelled sections at the bottom of `style.css`
- **Flexbox Only:** All layout is handled with flexbox to build a strong foundation before introducing CSS Grid
- **External CSS:** Demonstrates the standard practice of separating style from structure with a shared stylesheet
- **Multipage Pattern:** Shows how to maintain visual consistency across pages using shared classes and a single CSS file
- **CSS Concepts Deliberately Excluded (for future projects):** CSS custom properties (`--var`), `grid`, `position`, `z-index`, `@import`, `calc()`
- **Browser Compatibility:** All features supported in modern browsers (Chrome 88+, Firefox 85+, Safari 14+, Edge 88+)
