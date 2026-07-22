# GitHub Profile README Design Specification

## 1. Color Palette
A restrained, modern dark-mode palette designed for maximum contrast and readability.

*   **Base (Dark Neutral):** `#0d1117` (Matches GitHub's default dark mode background for seamless integration)
*   **Accent:** `#8b5cf6` (Electric Violet — A vibrant, energetic highlight color for primary elements and badges)
*   **Secondary (Muted Text):** `#8b949e` (Soft gray for secondary text, borders, and subtle elements)
*   **Text (Primary):** `#c9d1d9` (Off-white for high readability on the dark base)

## 2. Typography Approach
Consistent, clean, and legible across all platforms and GitHub's markdown renderer.

*   **Primary Font Style:** Geometric Sans-serif (Relying on system defaults like `-apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif` natively used by GitHub).
*   **SVGs and Shields:** Ensure all generated SVGs (like GitHub Readme Stats or custom banners) explicitly use the standard sans-serif font to avoid serif fallbacks.
*   **Monospace:** Use for any code snippets or technical references to maintain a developer-centric aesthetic.

## 3. Layout Grid
A strict, structured layout to avoid visual clutter and guide the reader's eye.

*   **Alignment:** Centered content (using `<div align="center">`) for banners, stats, and primary skill sections. Left-aligned for paragraph text (like the "About Me" section) for readability.
*   **Whitespace:** Generous spacing between sections. Use `<br><br>` or transparent spacing images between distinct logical blocks to let the content breathe.
*   **Grid Constraint:** Maximum of **3 visual blocks per row**. This applies to stat cards, highlighted project cards, or distinct skill categories. (Using flexbox/tables/Markdown grids).

## 4. Component Consistency Rule
Strict adherence to a single visual style for all interactive/graphical elements.

*   **Style Flavor:** `for-the-badge` (Bold, uppercase, modern, and highly legible). **NEVER MIX** with `flat`, `plastic`, or `social`.
*   **Corner Radius:** Sharp edges (0px radius). Because `for-the-badge` is inherently rectangular, any custom images, banners, or generated SVG cards should match this sharp-edged aesthetic.
*   **Color Family:** All badges should utilize the primary accent color (`#8b5cf6`), the dark base (`#0d1117`), or simple white/black for the logo depending on the badge's contrast needs. Do not use brand-specific colors (e.g., no green for Node, no red for Java); unify them under the custom palette.
