# 📘 Bootstrap 5 — Learning Documentation

_(Progress Log)_

---

## 1. Containers & Grid System

### 1.1 Container

- The `.container` class provides a **centered, fixed-width layout**.
- Its width adjusts at each breakpoint, enabling structured and responsive layouts.

### 1.2 Row

- The `.row` class creates a **horizontal wrapper** for columns.
- Ensures columns align correctly using Bootstrap’s flexbox-based grid.

### 1.3 Columns

- Bootstrap uses a **12-column grid system**.

- Example used: `col-12 col-md-6`:

  - `col-12` → full width on extra small & small screens.
  - `col-md-6` → half width on medium screens and above.

- This enables automatic responsive behavior **without custom CSS**.

### 1.4 Responsive Containers — Deep Dive

- Responsive containers remain **full-width until their specified breakpoint**, and from that breakpoint upward they become **fixed max-width**.
- `container-sm`, `container-md`, `container-lg`, etc. each activate at different breakpoints.
- Helps maintain readable content widths across various screen sizes.

---

## 2. Flexbox & Spacing Utilities

### 2.1 Flexbox Utilities

- `d-flex` activates flex behavior; `flex-column` or `flex-row` control direction.
- Responsive utilities (`flex-md-row`) adjust layouts at breakpoints.
- `justify-content-*` aligns items along the main axis.
- `align-items-*` aligns items along the cross axis.
- `gap-*` adds spacing between flex items without extra markup.
- `flex-fill` allows an element to expand into leftover space.

### 2.2 Spacing Utilities

- Spacing classes: `m-*`, `p-*`, `mt-*`, `py-*`.
- Scale ranges from `0` to `5`.
- Useful for creating consistent spacing across sections.

---

## 3. Components

### 3.1 Buttons

- Bootstrap provides multiple button **variants**: `btn-primary`, `btn-secondary`, `btn-danger`.
- **Outline buttons** (`btn-outline-*`) offer transparent background + colored border.
- Sizes: `btn-sm`, `btn-lg`.
- **Full-width buttons** using `w-100` or `d-grid` utilities.
- **Button groups** (`btn-group`) visually group related actions.

### 3.2 Cards & Responsive Grid

- Cards include `.card`, `.card-body`, `.card-title`, `.card-text` for structured content.
- `.card-header` and `.card-footer` create defined sections.
- `.card-img-top` places an image above the card body.
- `.card-img` + `.card-img-overlay` enables text overlays on images.
- Cards arranged responsively using `.row`, `.col-*`, and `g-*` gutters.

### 3.3 Navbar

- Built using `navbar`, `navbar-expand-*`, and background utilities.
- `.navbar-brand` displays the site or project name.
- Navbar collapse uses `data-bs-toggle="collapse"` and `data-bs-target="#navbarSupportedContent"`.
- Navigation items inside `.navbar-nav`; alignment via `ms-auto`.

### 3.5 Alerts

- Contextual alerts: `alert alert-*` (success, warning, danger, etc.).
- Dismissible alerts use `alert-dismissible fade show` and `btn-close`.
- Badges inside alerts emphasize status or updates.

### 3.6 Badges

- Built with `badge` + contextual colors like `bg-primary`, `bg-danger`, `bg-success`.
- Can be used inline with text, inside buttons, or as standalone labels.
- The `rounded-pill` class creates smooth, pill-shaped badges.

### 3.7 List Groups

- List groups use the `list-group` wrapper and `list-group-item` for individual items.
- `list-group-item-action` makes items interactive with hover and click behavior.
- Contextual variants (`list-group-item-primary`, `list-group-item-warning`, etc.) highlight important items.

### 3.8 Progress Bars

- Progress bars use a `.progress` wrapper and an inner `.progress-bar` element.
- The bar's fill level is controlled by setting its width (e.g., `50%`).
- Optional styles: `bg-*` colors, `progress-bar-striped`, `progress-bar-animated`.

### 3.9 Pagination

- Pagination is built using a `pagination` wrapper and `page-item` elements.
- Navigation links use the `page-link` class.
- Active and disabled states indicate the current page or unavailable navigation options.

### 3.10 Breadcrumbs

- Breadcrumbs represent page hierarchy using a `breadcrumb` wrapper.
- Each level is displayed using `breadcrumb-item`.
- The final item represents the active page and typically uses `aria-current="page"`.

### 3.11 Spinners

- Spinners visually indicate loading states without requiring JavaScript.
- Two types are available: `spinner-border` (border animation) and `spinner-grow` (pulsing grow animation).
- Color utilities like `text-primary`, `text-success`, and size variants such as `spinner-border-sm` customize appearance.

### 3.12 Tables

- Tables use the `table` class for consistent styling.
- Enhancements include `table-striped`, `table-hover`, and `table-bordered` to improve readability.
- Themes like `table-dark` provide alternate color styling.

### 3.13 Images & Thumbnails

- Responsive images use `img-fluid` so they scale with the parent container.
- `img-thumbnail` adds a bordered, padded, rounded frame.
- Shape utilities like `rounded`, `rounded-circle` modify appearance.

### 3.14 Ratio

- The `ratio` utility maintains fixed aspect ratios for embedded content.
- Common ratios include `ratio-16x9` and `ratio-4x3`.
- Applied to a wrapper containing iframes or media to ensure consistent responsive scaling.

### 3.15 Utility Add-Ons

- **Borders:** Add edges using `border`, directional borders like `border-top`, and color variants such as `border-primary`.
- **Shadows:** Visual depth provided using `shadow-sm`, `shadow`, and `shadow-lg`.
- **Text Colors:** Text styling with utilities like `text-primary`, `text-success`, and alignment helpers like `text-center`.
- **Background Colors:** Apply contextual backgrounds using `bg-primary`, `bg-warning`, or `bg-dark`, often paired with `text-white`.
- **Display Utilities:** Control display behavior using `d-block`, `d-inline`, `d-none`, with responsive versions like `d-md-block`.
- **Sizing Utilities:** Adjust element size using width (`w-25`, `w-50`, `w-100`) and height (`h-25`, `h-50`, `h-100`) utilities.

### 3.16 Accordion

- Accordions organize collapsible sections where users can expand and collapse content panels.
- Uses an `accordion` wrapper containing multiple `accordion-item` elements.
- Toggling is enabled with `data-bs-toggle="collapse"` and `data-bs-target="#id"`.
- `data-bs-parent` ensures that only one accordion item stays open at a time within the group.

### 3.17 Dropdowns

- Dropdowns reveal a menu of actions when triggered.
- Built using a `dropdown` wrapper containing a trigger element with `data-bs-toggle="dropdown"`.
- Menu items are defined inside a `.dropdown-menu` with each option as a `.dropdown-item`.
- Alignment utilities like `dropdown-menu-end` allow positioning the menu to the right.

### 3.18 Modal

- Modals display content in a centered popup overlay.
- Triggered using buttons with `data-bs-toggle="modal"` and `data-bs-target="#modalId"`.
- The modal structure includes `.modal-dialog` and `.modal-content` wrappers.
- Sections like `.modal-header`, `.modal-body`, and `.modal-footer` organize content.
- Closing behavior uses `data-bs-dismiss="modal"` on buttons or the close icon.

### 3.19 Offcanvas

- Offcanvas panels slide in from the left, right, top, or bottom of the screen.
- Triggered using `data-bs-toggle="offcanvas"` with a matching `data-bs-target="#id"`.
- Structure includes `.offcanvas-header` and `.offcanvas-body` for organized content.
- Supports dismiss actions using `data-bs-dismiss="offcanvas"`.
- Common uses include navigation menus, filters, and side panels.

### 3.20 Carousel

- Carousels create sliding presentations of images or content.
- Built with a `carousel` wrapper containing `.carousel-inner` and multiple `.carousel-item` elements.
- The first slide is marked using `.active`.
- Navigation controls (`carousel-control-prev` / `carousel-control-next`) allow manual slide switching.
- Indicators (dots) are added using `.carousel-indicators` for quick navigation.
- Supports `data-bs-ride="carousel"` for automatic cycling.

### 3.21 Popovers

- Popovers display small floating panels containing a title and message.
- Activated using elements with `data-bs-toggle="popover"`.
- Popovers require JavaScript initialization to function.
- Useful for offering additional context or explanations without cluttering the UI.

### 3.22 Tooltips

- Tooltips show brief hint text on hover or focus.
- Enabled by adding `data-bs-toggle="tooltip"` to an element.
- Placement can be controlled using `data-bs-placement` (top, bottom, left, right).
- Require JavaScript initialization like popovers.
- Best used for short helper text or clarifications.

### 3.23 Toasts

- Toasts are lightweight notification elements that briefly appear on the screen.
- They support auto-hide behavior and manual dismissal.
- Structure includes `.toast`, `.toast-header`, and `.toast-body`.
- Triggered and controlled via Bootstrap’s Toast JavaScript API.

### 3.24 Scrollspy

- Scrollspy automatically updates navigation links based on scroll position.
- Requires `data-bs-spy="scroll"` and a `data-bs-target` pointing to a navigation element.
- Highlights the active section as the user scrolls through content.
- Works inside any scrollable container, not just the body.

## 4. Forms

### 4.1 Form Controls

- Bootstrap styles inputs using `form-control` for text fields, emails, passwords, and textareas.
- Labels receive consistent styling with `form-label`.
- Helper text uses `form-text` for subtle guidance.

### 4.2 Select Menus

- Styled using `form-select`.
- Automatically match the styling of other form controls.

### 4.3 Checkboxes & Radios

- Built using the `form-check` wrapper.
- Inputs use `form-check-input` and labels use `form-check-label`.
- `form-check-inline` places multiple options on the same line.

### 4.4 Textarea

- Styled with `form-control` and supports adjustable `rows`.

### 4.5 Validation States

- `is-valid` and `is-invalid` provide visual feedback.
- Can be paired with `.valid-feedback` or `.invalid-feedback`.

### 4.6 Submit Buttons

- Any Bootstrap button class can be used for form submission.
- `w-100` makes the button span the full width.
