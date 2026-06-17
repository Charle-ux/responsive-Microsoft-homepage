# Rponsive-Microsoft-homepage

A pixel-accurate, fully responsive replica of the Microsoft Landing Page, CSS3, Flexbox, and CSS Grid. No frameworks. No JavaScript libraries. No dependencies.

LIVE DEMO
[View Project]( )

## Technologies Used

| Technology | Purpose |

| **HTML5** | Semantic structure (`header`, `nav`, `section`, `article`, `footer`) 
| **CSS3** | Styling, transitions, hover effects, gradients.
| **CSS Flexbox** | Navigation bar, card body layout, social strip, footer bottom bar.
| **CSS Grid** | 4-column product cards, 2-column feature banner, 6-column footer.
| **CSS Custom Properties** | Design token system (`--ms-blue`, `--ink`, `--shadow-hover`, etc.).
| **Media Queries** | 3-breakpoint responsive system (1100px / 768px / 480px).
| **SVG** | Microsoft 4-colour logo and icon buttons — no image requests.
| **Microsoft CDN** | Live product images served directly from Microsoft's own image CDN.

## Sections Built

- **Sticky Navigation** — Logo, 7 nav links, search button, "All Microsoft" toggle
- **Hero Banner** — Full-width image, white gradient overlay, headline, CTA, carousel dots
- **Consumer Products Grid** — Microsoft 365, Bing Wallpaper, Edge, OneDrive
- **Feature Highlight** — OneNote two-column layout (image + copy)
- **For Business Grid** — Microsoft 365 Copilot, Teams, Visual Studio 2026, Windows 365
- **Social Strip** — Follow Microsoft (X, LinkedIn)
- **Footer** — 6-column link grid + legal/locale bottom bar


## Responsive Behaviour

| Breakpoint | Layout Change |

| `≤ 1100px` | Cards → 2 columns · Footer → 3 columns · Nav spacing tightened.
| `≤ 768px` | Nav hidden · Feature section stacks vertically · Footer → 2 columns.
| `≤ 480px` | Cards → 1 column · Hero text simplified · All padding reduced .


## What I Learnt

- **CSS Grid vs Flexbox** — when to use each: Grid for page-level 2D layouts, Flexbox for 1D component rows/columns
- **CSS Custom Properties** — building a real design token system that mirrors how design systems work in production
- **Hero overlay technique** — layering `position: absolute` elements with a `linear-gradient` to keep text readable over a photograph without touching the image
- **`object-fit: cover`** — maintaining consistent image aspect ratios across all cards regardless of the source image dimensions
- **`clamp()`** — fluid typography that scales smoothly between viewport sizes without multiple media query overrides
- **Semantic HTML** — using `article`, `section`, `nav`, `header`, `footer` correctly for accessibility and SEO
- **File separation** — splitting CSS into base styles and media queries as a professional workflow habit
- **Sticky positioning** — `position: sticky` on the header without JavaScript



## Key UI Patterns Practised

- Card component with hover shadow lift and image scale transition
- Gradient overlay on hero images
- Sticky header with border-bottom divider
- CTA link with `::after` chevron content
- Dark footer with muted link colours and white hover states
- Locale/legal bottom bar layout