# Ricardo Prieto Álvarez — Portfolio

A minimalist, highly functional portfolio website inspired by Swiss Typography (International Typographic Style) and Andrej Karpathy's text-based architecture. 

Designed for high contrast, strict grid alignment, and absolute clarity, prioritizing whitespace and clean typography.

## Design Philosophy

- **Typography**: Uses the Inter typeface with Helvetica Neue and sans-serif fallbacks. High-contrast hierarchy with large titles and small uppercase section tags.
- **Strict Grid Alignment**: 100% left-aligned content with no card blocks, borders (except dividing rules), icons, or decorations.
- **Premium Accents**: Whitespace serves as the main design element. Hover interactions are limited to instant (100ms or less) color and border transitions on text links.
- **Print Optimization**: Integrates specialized print styles (`@media print`) that adapt the layout, sizes, and padding so the entire portfolio prints beautifully on a single A4 page or converts perfectly to a PDF document.

## How to View

You can view the site by opening the `index.html` file directly in any modern browser, or run a simple local web server:

```bash
# Using Python
python3 -m http.server 8000

# Using Node.js (npx)
npx http-server
```

## How to Save as PDF

Click the **"Print Portfolio / Save as PDF"** link at the bottom of the page (hidden on print) or press `Cmd+P` / `Ctrl+P` in your browser. Select "Save as PDF" as the destination. The styles are pre-configured to ensure the entire page fits cleanly onto a single-page document.
