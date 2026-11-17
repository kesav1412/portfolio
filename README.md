# Kesavapandi V — Portfolio

Personal portfolio for a backend developer: a single-page bento grid built with plain HTML, CSS and vanilla JavaScript. No framework and no build step.

**Live site:** https://kesav1412.github.io/portfolio/

## Features

- Fixed 1440×960 stage that scales to any desktop window, and a stacked layout on screens 820px wide or narrower, with extra styles for very small (smartwatch-size) screens.
- Cards for work experience, education and certification, tech stack, current focus, projects, and "How I work".
- Light and dark theme toggle that follows the system setting and remembers your choice.
- Motion driven by one clock: the `currentTime` of a Web Animation, read in a single `requestAnimationFrame` loop. Reduced-motion users get a static page.

## Files

| File | Purpose |
|---|---|
| `content.json` | **All the text and links on the page. Edit this to change content.** |
| `index.html` | Layout, styles and script. Reads `content.json` and fills the page |
| `kesav.jpg` | Profile photo |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

## Run locally

The page loads `content.json` with `fetch`, so opening `index.html` by double-click will not work. Serve the folder instead:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000.

## Deploy

The site is hosted on GitHub Pages from the `main` branch, root folder. Push to `main` and it redeploys within about a minute.

## Customise

- **Text and links:** edit `content.json`: headline, bio, contact links, status, location, work experience, tech stack, current projects, education, projects, and the four "How I work" steps. To add a job, a tag or a project, add another entry to the matching list. The number of "How I work" steps can change too.
- **Layout and look:** `index.html`.
- Colours are CSS variables at the top of the `<style>` block, with a separate set for dark mode.
- Fonts: the page uses Inter if it is installed or placed at `fonts/InterVariable.woff2`, and falls back to the system sans-serif.

## Contact

- Email: kesavapandi2000@gmail.com
- LinkedIn: https://www.linkedin.com/in/kesavapandi-v
- GitHub: https://github.com/kesav1412
