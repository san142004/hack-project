# Project context

## Overview

This repository is a static, Hack The Box themed cybersecurity training website. It presents learning paths, red/blue/purple team training, pricing, and company information. The current project is a front-end prototype; the calls to action do not connect to an application or backend.

## Stack and layout

- Plain HTML and CSS. There is no JavaScript, package manifest, build step, or test suite in the repository.
- All pages are at the repository root. `style.css` contains the shared design system, layout, components, and responsive rules.
- `image/` contains local logos, illustrations, and the looping `video.webm` background. Main pages also load the Inter font from Google Fonts.
- The visual style uses dark navy backgrounds, lime green accents (`--primary-green: #9FE219`), cards, a sticky header, and responsive grids. Several sections also use inline styles.

## Pages

| File | Current role |
| --- | --- |
| `index.html` | Landing page with hero, learning features, team solutions, social proof, news, and career sections. |
| `red-teams.html` | Offensive security training page. |
| `blue-teams.html` | Defensive security training page. |
| `purple-teams.html` | Combined offensive and defensive training page. |
| `pricing.html` | Individual plans, enterprise section, and FAQ. |
| `company.html` | Mission, values, careers, and contact information. |
| `academy.html`, `products.html`, `solutions.html`, `cybersecurity-resources.html` | Minimal placeholder pages. |

## Running the project

Open `index.html` in a browser, or serve the repository root with any static file server and open its local URL. There are no dependencies to install. Serving the root is preferable when checking links that use `/`.

## Current limitations and maintenance notes

- Many buttons and footer links use `href="#"`; navigation items such as `#platform`, `#resources`, `#business`, `#signin`, and `#get-started` have no matching section IDs. Treat these as unfinished navigation.
- The Individual/Teams controls on `pricing.html` are visual buttons only. There are no scripts, forms, authentication, or checkout flows.
- The four placeholder pages reference `../style.css` even though they sit beside `style.css`; their shared styling will not load from the repository root.
- The main pages repeat the header and footer markup. If shared navigation changes, update each page consistently.
- Preserve existing local asset paths when editing pages, and use the CSS variables in `style.css` for shared colors and spacing.
