# andrewcmiller.org

Personal academic website of Andrew Cesare Miller, served by GitHub Pages.

The site is plain HTML and CSS. It has no build step, no framework, and no external dependencies. The fonts are self-hosted free stand-ins for the original Typekit fonts: Oswald (same as the original), Jost for Futura PT and Europa, and Figtree for Proxima Nova.

| File | URL |
|---|---|
| `index.html` | `/` |
| `research.html` | `/research` |
| `biography.html` | `/biography` |
| `contact.html` | `/contact` |
| `home.html` | `/home` (redirects to `/`; kept for old Squarespace links) |
| `404.html` | shown for any missing page |
| `assets/site.css` | all styles; the design follows the original Squarespace site |
| `assets/img/` | cover photo (`cover-photo.jpg`), research banner (`baltimore.jpg`), book cover, social-share image, favicon |
| `Miller_CV.pdf` | CV, linked from the Bio page |
| `llms.txt` | plain-text summary and full publication list for AI assistants and crawlers |
| `robots.txt`, `sitemap.xml` | crawler instructions and page list for search engines |
| `CNAME` | tells GitHub Pages to serve the site at andrewcmiller.org |

GitHub Pages serves `research.html` at `/research`, so the old Squarespace URLs keep working.

## Updating content

- **Add an article:** in `research.html`, copy one `<article class="pub">…</article>` block under "Journal Articles," paste it at the top of that list, and edit the title, link, citation and abstract.
- **Edit the bio:** edit the paragraphs in `biography.html`.
- **Update the CV:** replace `Miller_CV.pdf` with the new PDF, keeping the same file name; the Bio page's download button points to it.

Commit to `main` and the site updates within a minute or two.

## Previewing locally

All links and asset paths are relative, so the site works from any folder. From the repository folder, run:

```
python3 -m http.server 8000
```

Then open http://localhost:8000.
