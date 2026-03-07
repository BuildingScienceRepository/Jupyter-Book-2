## 2024-03-06 - Enhancing MyST Accessibility and Polish
**Learning:** This is a MyST markdown (Jupyter Book 2) project. Direct HTML/JSX edits aren't possible as the site is statically generated from Markdown and predefined themes. However, MyST allows injecting a custom CSS file via `site.options.style` in `myst.yml`.
**Action:** Created `custom.css` to add a highly visible, keyboard-accessible focus ring (`:focus-visible`) and smooth hover transitions. Added this CSS to `myst.yml`. This improves keyboard navigation accessibility and provides a subtle layer of UX polish on interactions without changing the core theme or adding dependencies.

## 2026-03-07 - Accessible Smooth Scrolling in Static Sites
**Learning:** Adding `scroll-behavior: smooth` directly to the `html` element is a quick way to add spatial context to anchor link navigation (e.g., Table of Contents clicks) in statically generated sites like MyST. However, this global smooth scrolling can trigger motion sickness for users with vestibular disorders.
**Action:** Implemented the smooth scroll CSS pattern wrapped in a `@media (prefers-reduced-motion: no-preference)` query. This provides the UX enhancement for most users while seamlessly falling back to instant jumps for users who have requested reduced motion at the OS level. This is a crucial accessibility pattern for any global CSS animation or transition.
