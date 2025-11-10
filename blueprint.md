
# Step-by-Step Astro Blog

## Overview

A personal blog website built with Astro.js. It features a clean, modern design, a blog section with posts written in Markdown, and an RSS feed. The site is designed to be fast, accessible, and SEO-friendly.

## Project Outline

*   **Framework:** Astro.js
*   **Styling:** Tailwind CSS, global CSS file for base styles.
*   **Pages:**
    *   Home (`/`): Displays a welcome message and a list of recent blog posts.
    *   About (`/about`): A page with information about the author.
    *   Blog (`/blog`): A list of all blog posts.
    *   Blog Post (`/blog/[slug]`): Individual blog post pages.
*   **Content:**
    *   Blog posts are written in Markdown and stored in `src/content/blog/`.
    *   Images are stored in `src/assets/`.
*   **Features:**
    *   RSS feed (`/rss.xml`).
    *   Sitemap (`/sitemap-index.xml`).
    *   Responsive design.
    *   Dark mode.
*   **Design:**
    *   **Fonts:** Atkinson Hyperlegible for readability.
    *   **Color Palette:** A custom color palette with shades of gray, and accent colors for links and other elements.
    *   **Layout:** A centered, single-column layout for content.

## Current Plan: Fix "Page Not Found" Error

1.  **Update Astro Configuration:** Set the `trailingSlash` option to `'always'` and `build.format` to `'file'` in `astro.config.mjs`. This will change the output of the build to be a single HTML file per page (e.g., `/blog/first-post.html`), which is a more robust way to handle routing on static hosting platforms.
2.  **Rebuild Project:** Run `npm run build` to apply the changes.
3.  **Deploy to Firebase Hosting:** Deploy the `dist` directory to Firebase Hosting.
4.  **Final Verification:** Verify that the deployed site is working correctly.
