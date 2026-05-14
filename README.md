# DST Visualizer

Web-based visualizer for Tajima DST embroidery files.

**Live tool:** https://nt-rhoback.github.io/dst-visualizer/

## What it does

- Drop a `.dst` file → renders the stitched design with selectable thread colors
- Drop a color-card PDF → auto-applies Madeira Polyneon / Classic codes from Wilcom, Pulse Microsystems, or Classic Color Card formats
- Sequins and blings render as filled circles in each stop's color
- Detects Wilcom-wrapped DST files (where the real DST is hidden behind a proprietary container)
- Undo / Redo for color stop changes
- Export the colored preview as a PNG (300 dpi) with dimensions stamped on
- Generate a worksheet PDF for the sew-out

## Important notes for production

- The visualizer can't read sequin/bling info stored in Wilcom's proprietary wrapper metadata — it only renders sequins encoded directly in the standard DST stitch stream. When a file shows the **"Potential issue — sequins / blings detected"** warning, open it in Wilcom to verify the full design before production.
- Rhoback doesn't produce designs with sequins or rhinestones. Any file showing decorative drops should be checked with the customer.

## License / use

Internal Rhoback tool. The HTML is self-contained — no server, no backend, no external dependencies. Open in any modern browser.
