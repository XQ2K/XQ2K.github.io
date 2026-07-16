# Yuqing Luo GitHub Pages Portfolio

A responsive, bilingual, dependency-free academic portfolio for GitHub Pages.

## Files

- `index.html` - complete website (HTML, CSS, and JavaScript in one file)
- `assets/` - research figures, CV, favicon, and local paper PDFs

## Deploy to GitHub Pages

1. Back up the current repository.
2. Copy `index.html` and the entire `assets/` folder to the repository root.
3. Commit and push:

```bash
git add index.html assets/
git commit -m "Redesign academic portfolio"
git push
```

4. In the GitHub repository, open **Settings -> Pages**.
5. Set the source to the branch containing these files, using the repository root (`/`).
6. Wait a few minutes, then refresh the `github.io` site.

## Customisation

The content is data-driven in the `projectData` object near the bottom of `index.html`.

- Change the contact email by searching for `xqtheone@gmail.com`.
- Update publications in the `#publications` section.
- Replace the CV at `assets/Yuqing_Luo_CV.pdf` without changing any code.
- Replace local paper PDFs in `assets/papers/` while keeping their filenames.
- Change the default language by changing:

```js
let currentLanguage = localStorage.getItem("portfolio-language") || "en";
```

from `"en"` to `"zh"`.

## Notes

- No npm, build command, or framework is required.
- The site supports dark/light mode, English/Chinese switching, mobile navigation, animated project diagrams, scroll reveal, and research-figure lightboxes.
- Research images were cropped from the author-provided papers for use on the author's own academic website.
