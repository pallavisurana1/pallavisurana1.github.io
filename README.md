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

- **Change order:** move the entire project's `<article class="project"> ... </article>` block.
- **Change text:** edit `project-title`, `project-summary`, and the paragraph in `project-content`.
- **Change a figure:** replace its image in `images/`, or update both the figure's `href` and image `src`. Update `alt` to describe the figure.
- **Change paper or dataset links:** edit the links in `<p class="links">`. They stay visible when details are closed.
- **Add an expandable project:** copy a complete expandable project block, give its `<details>` a unique `id`, and keep `name="research-project"`. This lets one project open at a time in current browsers. Content remains usable without JavaScript.
- **Rename a project:** its title is independent of its figure filename, so existing image files can keep their names.

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
