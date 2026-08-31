# News Community Online Demo - Design QA

## Scope

- One standalone static site combines the former home and article-entry demos.
- The site excludes the requirements panel, solution tabs, and the other five prototype screens.
- All image assets are local to `assets/`; no external image request is required.

## Verified Viewports

- Desktop browser viewport with a centered 390px device surface.
- Mobile viewport: 390 x 844 CSS px.

## Verified Interactions

- Lead story opens the article at the top.
- Article back button restores the home screen.
- Home inline comment opens the article at `News comments`.
- Home inline-comment likes float across the card's bottom-right border without reducing the two-line text width.
- The news-comment carousel exposes the next card and moves from `1 / 3` to `2 / 3` after a horizontal drag.
- Article reaction buttons retain a selected state.

## Verification Results

- Inline JavaScript syntax: passed with `node --check`.
- HTML structure: no parser errors reported by `tidy` with HTML5 block tags configured.
- Browser console: 0 errors, 0 warnings.
- Mobile document overflow: 0px at 390 x 844.
- Inline-comment text width: 314px; the floating like badge has 2.66px clearance from text and 3px clearance from the next news row.
- Inline-comment text/like overlap: false; like/next-row overlap: false.
- Broken images: 0.
- Active product screen count: 1.
