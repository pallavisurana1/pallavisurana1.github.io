# Pallavi Surana — academic website

Personal academic website, live at [pallavisurana1.github.io](https://pallavisurana1.github.io).
Plain HTML and CSS; no installation or build step required.

## Where to edit

| File or folder | What it contains |
| --- | --- |
| `index.html` | All page text, project order, links, news, and contact details |
| `style.css` | Colors, fonts, spacing, and mobile layouts |
| `images/` | Headshot and research figures |
| `docs/` | PDFs linked from the website |

## Research projects

Search for `EDIT RESEARCH` in `index.html`.

Projects appear in this order: OnKoLoop, PGViS, Isoform Tumor Expression in Solid Tumor, TSProm, TransTEx.

- **Change order:** move an entire project's `<article> ... </article>` block.
- **Change card text:** edit `project-title` and `project-summary`.
- **Change destination:** edit the card's `href`. Each shaded PhD card opens its matching section in `phd-research.html`.
- **Add a PhD card:** copy a `phd-project-card` block and update its unique `id`, title, summary, accessible label, and destination.
- **Edit project descriptions, figures, or paper links:** update the corresponding section in `phd-research.html`.

### OnKoLoop poster

Upload the poster as **`docs/CAFCW_OnKoLoop.pdf`**, matching capitalization exactly. Poster links open the GitHub PDF viewer in a new tab. Commit and push the PDF to `main` to update that viewer.

## Other edits

- **News:** search for `To add news`; copy one `<li>` and place the newest item first.
- **About, Bio, Contact:** find the matching section in `index.html`.
- **Colors:** edit the named values under `:root` at the top of `style.css`.
- **Research layout:** find `expandable research projects` near the end of `style.css`.

## Preview and publish

Open `index.html` in a browser to preview. Try each research row, the paper links, and a narrow window to check the mobile layout.

Commit and push the changed files to the branch used by GitHub Pages to publish them. Upload the OnKoLoop PDF before publishing if you want its link available immediately.

## OnKoLoop project page

Clicking the OnKoLoop title opens `onkoloop.html`. The separate **CAFCW SC26 Poster ↗** link still opens the GitHub PDF viewer in a new tab.

Edit `onkoloop.html` to grow the project page:

- `EDIT PROJECT INTRO`: update the introductory text.
- `EDIT POSTER`: the page displays `images/onkoloop-poster.jpg` and links to the GitHub viewer for `docs/CAFCW_OnKoLoop.pdf`. Replace both when updating the poster. The image preview works without browser PDF support.
- `EDIT FUTURE CONTENT`: replace the overview placeholder and copy the section to add methods, findings, or resources.

The page shares `style.css` with the homepage, so site-wide design updates apply to both.

## PhD Research page

`phd-research.html` contains the expanded PhD story, organized into TransTEx, tumor isoforms, evolution, TSProm, and PGViS. Each shaded homepage project card links to its matching section on this page.

- Edit the clearly marked `EDIT` sections to update the scientific text.
- Replace `images/phd-theme.png` and `docs/PhD_theme.pdf` together to update the theme diagram.
- Each project reuses its existing figure in `images/` and paper links.
- Keep the section IDs (`transtex`, `isoform-tumor`, `evolution`, `tsprom`, `pgvis`) stable so homepage links continue working.

OnKoLoop also uses a full clickable card, opening `onkoloop.html`. Its deeper sage color is set under `.onkoloop-card` in `style.css`; poster links are on the project page.
