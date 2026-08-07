# Lighthouse Summary

Local Lighthouse run for `http://localhost:8000/` on 2026-08-07.

## Scores

- Performance: 76
- Accessibility: 98
- Best Practices: 96
- SEO: 100

## Core Metrics

- First Contentful Paint: 1.6 s
- Largest Contentful Paint: 5.6 s
- Total Blocking Time: 110 ms
- Cumulative Layout Shift: 0.084
- Speed Index: 2.4 s

## Main Opportunities

- Improve image delivery, especially images contributing to Largest Contentful Paint.
- Add explicit `width` and `height` attributes to image elements.
- Consider CSS minification in the future if the site grows.
- Review cache lifetimes after deployment, because static hosting/cache settings can affect this.

## Interpretation

The site is strong for SEO, accessibility, and best practices. The main technical opportunity is performance, especially image delivery and LCP on the home page.
