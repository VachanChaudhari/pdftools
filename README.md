# iLovePDF Clone

A faithful, fully front-end clone of the **iLovePDF** website — the colorful PDF-tools
marketplace with a header, hero, category-organized tool grid, feature strip, CTA and footer.

## ✨ What's included

- **Pixel-style recreation** of the iLovePDF landing layout (header nav, hero, tool cards
  grouped by category: Organize · Optimize · Convert to PDF · Convert from PDF · Edit · Security).
- **Responsive design** with a mobile hamburger menu.
- **Working tool modals** — click any tool to open a drag-and-drop uploader with per-tool options.
- **Real, in-browser PDF processing** (no server needed) via `pdf-lib` + `pdf.js` (loaded from CDN).

## 🛠 Tools that actually work

| Tool | What it does |
|------|--------------|
| Merge PDF | Combine multiple PDFs into one |
| Split PDF | Extract a page |
| Organize PDF | Reverse/reorder pages |
| Rotate PDF | Rotate every page 90/180/270° |
| Compress PDF | Re-save with object streams + size report |
| Repair / Unlock | Re-save ignoring encryption |
| OCR / PDF→Word / PDF→Excel | Extract text (PDF→Word `.doc`, PDF→Excel `.csv`) |
| PDF→JPG | Render a page to an image |
| JPG→PDF | Wrap images into a PDF |
| Page Numbers | Stamp page numbers (position options) |
| Watermark | Diagonal text watermark |
| Protect PDF | Owner-password encryption |
| Sign PDF | Typed signature on the last page |

Word/PPT/Excel/HTML → PDF are wired as demo passthroughs (real conversion is server-side).

## ▶️ Run it

Just open `index.html` in a browser. For full processing, run a local server so the CDN libs load:

```bash
cd ilovepdf-clone
python3 -m http.server 8080
# visit http://localhost:8080
```

> Note: the CDN scripts (`pdf-lib`, `pdf.js`) require an internet connection. Without them,
> file selection and the UI still work; processing shows an offline notice.

## 📁 Structure

```
ilovepdf-clone/
├── index.html       # layout + tool cards + modal markup
├── css/style.css    # full styling (iLovePDF-inspired theme)
└── js/main.js       # modal logic + per-tool PDF processors
```

---

Demo/educational project. Not affiliated with iLovePDF.
