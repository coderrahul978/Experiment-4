# Experiment 4 - SEO and accessibility optimization
`before.html` is the given unoptimized page; `index.html` is the optimized version. (Add any image named coffee.jpg to see the image.)

| Problem in before.html | Fix in index.html |
|---|---|
| No doctype, no lang, no charset/viewport | Added `<!DOCTYPE html>`, `lang="en"`, charset and viewport meta |
| Title "page", no description | Descriptive `<title>` and meta description, keywords, robots, canonical, Open Graph tags |
| Everything in `<div>` with inline font sizes | Semantic `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`, `<address>` |
| No `<h1>`, headings jump to `<h4>` | One `<h1>`, then `<h2>` sections in order |
| `<img>` has no alt text or size | Meaningful `alt`, width/height, `loading="lazy"`, `<figure>` and `<figcaption>` |
| "click here" links | Descriptive link text, `aria-label` on nav, phone as `tel:` link |
| Light grey text on white (low contrast) | Dark text on light background (WCAG AA contrast) |
| No keyboard support | "Skip to main content" link and visible focus outlines |

Check with Chrome Lighthouse (DevTools -> Lighthouse -> SEO and Accessibility) on both files and note the score improvement in the report.


**Bootstrap (minimal):** Bootstrap 5 via CDN; uses `container`, `list-group` and `img-fluid`. Semantic HTML and SEO/accessibility fixes are unchanged.
