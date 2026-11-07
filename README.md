# Portfolio

An intentionally small personal portfolio inspired by [nqd.vn](https://nqd.vn/):
a narrow reading column, simple project links, and generous spacing.

Plain HTML and CSS. No dependencies, JavaScript, or build step. The layout adapts
to mobile screens and follows the visitor’s light or dark appearance preference.

## Preview

Serve the repository locally so the homepage, `/cv/`, and `/uses/` routes work:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Visit <http://127.0.0.1:8000>, the CV at <http://127.0.0.1:8000/cv/>,
or Uses at <http://127.0.0.1:8000/uses/>.
Stop the server with `Ctrl+C`.

## Update content

Edit `index.html` for the homepage, `cv/index.html` for the CV, and
`uses/index.html` for the hardware and tools list:

- The page title, description, and introduction.
- Project links, descriptions, and category labels.
- Contact and profile links.
- The footer year.

The introduction, projects, and contact links are based on the supplied CV and
personal details. The CV page presents the PDF content as HTML, including
experience, projects, publications, education, skills, achievements, and
certificates. Update it when the source CV changes. The original PDF remains
reference material and is not linked for download.

The homepage’s More section links to CV and Uses, between Projects and Elsewhere.
Uses groups the supplied setup into hardware, system, editor and terminal, and
AI tools. Update the setup and skill links in `uses/index.html` as they change.

Use the browser’s Print command on the CV page to print or save a PDF. Print
styles use a light appearance and hide navigation and the footer.

Adjust the colors, spacing, and font in `styles.css`. No external fonts, images,
analytics, or services are loaded.

## Verification

There is no build or test framework. Before publishing, preview the page at a
narrow mobile width and a desktop width, check light and dark appearances, use
Tab to check keyboard focus, and verify your project and contact links.

The preview command above is for local development, not public hosting.

## Publish with GitHub Pages

This site uses the free GitHub Pages address:
<https://huatansang.github.io/>. No custom domain or paid hosting is required.

After the source is pushed to `HuaTanSang/huatansang.github.io`:

1. Open the repository’s **Settings → Pages**.
2. Under **Build and deployment**, select **Deploy from a branch**.
3. Select **main**, choose **/(root)**, and click **Save**.
4. Wait for the Pages deployment to finish before sharing the URL.

The empty `.nojekyll` file lets Pages serve the HTML and CSS directly.
After Pages is enabled, pushes to `main` update the live site. Check the
homepage, `/cv/`, and `/uses/` after deployment.

The original CV PDF and its download metadata are ignored. The initial upload
includes only the website files, this README, `.gitignore`, and `.nojekyll`;
local agent instructions and workflow notes remain in the workspace.

## Repository structure

```text
.gitignore                   Files excluded from version control
.nojekyll                    Serve static files without Jekyll
README.md                    Preview, content, and publishing instructions
index.html                   Portfolio content and metadata
cv/index.html                CV in HTML
uses/index.html              Hardware and tools
styles.css                   Responsive layout and color themes
```
