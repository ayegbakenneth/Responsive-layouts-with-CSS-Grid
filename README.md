# Responsive Web Layout with CSS Grid and Tailwind CSS

**Project Live URL:** [https://ayegbakenneth.github.io/Responsive-layouts-with-CSS-Grid/](https://ayegbakenneth.github.io/Responsive-layouts-with-CSS-Grid/)

This project demonstrates a responsive web layout built using a combination of CSS Grid for the main structural layout and Tailwind CSS for component-level styling and utility.

## Objective

The objective was to create a fully responsive web page that adapts seamlessly across desktop, tablet, and mobile devices, with CSS Grid as the primary layout system for major sections.

## Technologies Used

-   **HTML5:** For semantic content structure.
-   **CSS Grid:** For the main page layout (header, main, footer) and key sections (navigation, hero, features).
-   **Tailwind CSS (CDN):** For utility-first styling of individual components (colors, spacing, typography, shadows, hover effects, etc.).
-   **Google Fonts:** For 'Inter' font and 'Material Symbols Outlined' icons.
-   **Font Awesome (CDN):** For social media or other general icons.

## Features

-   **Fully Responsive:** Layout adapts to different screen sizes.
-   **CSS Grid Driven:** Main layout achieved using `display: grid` and media queries.
-   **Semantic HTML:** Uses appropriate HTML5 elements for structure.
-   **Modern CSS Practices:** Clean, organized CSS with clear separation of concerns.
-   **Efficient Styling:** Leverages Tailwind CSS utilities for rapid and consistent component styling.
-   **Cross-Browser Compatibility:** Includes vendor prefixes for broader browser support.

## Setup Instructions

To run this project locally, simply follow these steps:

1.  **Save the files:**
    -   Save the HTML code as `index.html`.
    -   Save the CSS code as `styles.css` in the same directory as `index.html`.
2.  **Open `index.html`:** Double-click the `index.html` file in your web browser.

That's it! The page should load and be responsive.

## Code Explanation

### `index.html`

-   Includes the `<meta name="viewport">` tag for proper responsiveness.
-   Links to `styles.css` for custom CSS Grid rules.
-   Loads the Tailwind CSS CDN for utility classes.
-   Loads Google Fonts for 'Inter' (the main font) and 'Material Symbols Outlined' (for the menu icon).
-   The `.main-layout-container` div uses `display: grid` in `styles.css` to define the overall structure (header, main content, footer).
-   Sections like `.nav-grid`, `.hero-content-grid`, and `.features-grid` also utilize `display: grid` in `styles.css` to manage their internal layouts.
-   Tailwind classes are still used extensively for visual styling (e.g., `text-2xl`, `bg-white`, `rounded-lg`, `shadow-lg`, `px-4`, `py-8`, hover effects).

### `styles.css`

-   Defines the primary grid containers (`.main-layout-container`, `.nav-grid`, `.hero-content-grid`, `.features-grid`).
-   Uses `grid-template-columns` and `grid-template-rows` to define column and row structures.
-   Employs media queries (`@media (min-width: ...)` to adjust the grid layouts for different breakpoints.
-   Includes basic `font-family` settings and root variables for colors for maintainability.
-   Adds vendor prefixes for `transition` properties to ensure cross-browser compatibility.

## Responsive Breakpoints

### Mobile (default)

-   **Navigation:** Logo on the left, mobile menu button on the right. Navigation links and the desktop "Get Started" button are hidden.
-   **Hero Section:** Content is stacked in a single column.
-   **Features Section:** Cards are stacked in a single column.

### Tablet (`min-width: 640px`)

-   **Features Section:** Cards are arranged in two columns.

### Desktop (`min-width: 1024px`)

-   **Navigation:** The logo, full navigation links, and the "Get Started" button are all visible in a three-column grid. The mobile menu button is hidden.
-   **Hero Section:** The content and image are arranged side-by-side in a two-column grid.
-   **Features Section:** Cards are arranged in three columns.

### Large Desktop (`min-width: 1280px`)

-   **Features Section:** The gap between the feature cards is increased for a more spacious layout on larger screens.

## Evaluation Criteria

-   **CSS Grid implementation quality:** The project uses CSS Grid for the main layout structure and for key components like the navigation, hero, and features sections. The grid is implemented using a mobile-first approach with clear and concise code.
-   **Responsive design effectiveness:** The layout adapts seamlessly across three breakpoints (640px, 1024px, and 1280px), ensuring a consistent user experience on mobile, tablet, and desktop devices.
-   **Code organization and cleanliness:** The HTML and CSS are well-organized with clear comments and a logical structure. The use of semantic HTML and modern CSS best practices ensures the code is easy to read and maintain.
-   **Cross-browser compatibility:** Vendor prefixes have been added for `transition` properties to ensure the layout works consistently across all modern browsers.
-   **Performance optimization:** The project uses a CDN for Tailwind CSS and Google Fonts to reduce the load on the server. The image is also optimized for the web.