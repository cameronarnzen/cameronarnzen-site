# cameronarnzen.com

Quarto source for www.cameronarnzen.com, published with GitHub Pages from the `docs/` folder.

## Updating the site (R console)

```r
quarto::quarto_preview()            # live preview while editing; quarto::quarto_preview_stop() to end
quarto::quarto_render()             # rebuild docs/
gert::git_add(".")
gert::git_commit("Update site")
gert::git_push()                    # live within a couple of minutes
```

## Where things are

- `index.qmd`, `research.qmd`, `teaching.qmd`, `media.qmd`: one file per page
- `_quarto.yml`: menu, footer links, site settings
- `styles.scss`: colors and fonts (palette at the top)
- `images/headshot.jpg`: your photo
- `files/arnzen-cv.pdf`: your CV (the CV menu link points here)
- `docs/`: the built site. Don't edit by hand; `quarto_render()` overwrites it.
