# CSVTU Study Portal

CSVTU Study Portal site source with PYQs, syllabus, notes, question banks, videos, books, and course resources for CSVTU programs (B.Tech, M.Tech, Diploma).

**Repository Contents**
- `/Users/anurag/Desktop/CSVTU/csvtu.xml` — Canonical Blogger XML source (layout, widgets, CSS, and scripts).
- `/Users/anurag/Desktop/CSVTU/index.html` — HTML export for local preview (still contains Blogger tags/expressions).
- `/Users/anurag/Desktop/CSVTU/styles.css` — Extracted stylesheet (from `csvtu.xml`).
- `/Users/anurag/Desktop/CSVTU/scripts.js` — Extracted scripts (from `csvtu.xml`).

**Tech Stack (Detailed)**
- HTML5 (Blogger-compatible XHTML markup).
- CSS3 with custom properties, media queries, flexbox, and keyframe animations.
- JavaScript (ES5+ DOM APIs, event handling, lazy loading, scroll logic).
- Blogger XML templating (GML) with `b:` tags and `data:`/`expr:` bindings.
- JSON-LD and microdata for SEO (Schema.org).
- Open Graph + Twitter Card metadata.
- Inline SVG icons and SVG sprites.
- Base64 data URIs for placeholders.

**Blogger XML Tags Used**
- `b:attr`, `b:class`, `b:defaultmarkup`, `b:defaultmarkups`, `b:eval`, `b:if`, `b:elseif`, `b:else`, `b:loop`, `b:include`, `b:includable`, `b:message`, `b:param`, `b:section`, `b:tag`, `b:template-skin`, `b:widget`, `b:widget-setting`, `b:widget-settings`, `b:with`.

**Blogger Data Bindings (Examples)**
- `data:blog.*` (title, description, URLs, IDs, settings).
- `data:view.*` (page context, homepage, post, error view, mobile, search).
- `data:post.*` (title, snippet, author, images, timestamps).
- `data:messages.*` (localized UI strings).

**Fonts**
- Google Sans Text (400/700) loaded via `@font-face` from `fonts.gstatic.com`.
- Google Sans Mono (400) loaded via `@font-face` from `fonts.gstatic.com`.

**SEO + Structured Data**
- JSON-LD types used: `EducationalOrganization`, `Course`, `WebSite`, `SearchAction`, `BlogPosting`, `ImageObject`, `Organization` (publisher).
- Microdata types used: `SiteNavigationElement`, `BreadcrumbList`, `ListItem`, `Comment`, `Person`.

**Core Features (Implemented in CSS/JS)**
- Responsive layout with desktop and mobile variants.
- Dark mode toggle with localStorage persistence.
- Sticky header and mobile menu transitions.
- Lazy image loading with IntersectionObserver.
- Lazy YouTube embeds with thumbnail placeholders.
- Lightbox-style image viewer.
- Infinite scroll (AJAX) + numbered pagination.
- Related posts (in-article and bottom widgets).
- Reading time estimate.
- Time-ago timestamps.
- Copy-to-clipboard helpers.
- Preloader animation.
- Maintenance mode countdown.
- Bookmarking (saved list).
- Offline/online notifications.

**Third-Party Libraries / Services (Hooked, Configurable)**
- Disqus comments (lazy-loaded on scroll).
- Simple AJAX Infinite Scroll by Taufik Nurrohman (dte.web.id).
- `@shinsenter/defer.js` for deferred/lazy loading of scripts, styles, and media.
- Google Analytics / Tag Manager hooks.
- Google AdSense hooks (`adsbygoogle`).
- Google Translate widget.
- Firebase Realtime Database hooks for “real views”.
- Facebook SDK for widgets/share features.
- Google Fonts via `fonts.gstatic.com` (`Google Sans Text`, `Google Sans Mono`).
- Polyfill.io for `IntersectionObserver` support.
- Highlight.js hooks for code highlighting (if enabled).

**External Link Targets Used for Sharing**
- Facebook, WhatsApp, Twitter/X, Telegram, Pinterest, LinkedIn, Line.

**How to Use**
1. Blogger deployment: upload `/Users/anurag/Desktop/CSVTU/csvtu.xml` as the theme in Blogger.
2. Local preview: open `/Users/anurag/Desktop/CSVTU/index.html` in a browser.
3. Styling changes: edit `/Users/anurag/Desktop/CSVTU/styles.css` (then sync into `csvtu.xml` if deploying on Blogger).
4. Script changes: edit `/Users/anurag/Desktop/CSVTU/scripts.js` (then sync into `csvtu.xml` if deploying on Blogger).

**Configuration Points (Typical)**
- Disqus shortname: `disqus_shortname` in `/Users/anurag/Desktop/CSVTU/scripts.js`.
- Analytics ID: `analyticsID` in `/Users/anurag/Desktop/CSVTU/scripts.js`.
- AdSense publisher ID: `adsenseAds.publisherId` in `/Users/anurag/Desktop/CSVTU/scripts.js`.
- Firebase database URL: `realViews.databaseUrl` in `/Users/anurag/Desktop/CSVTU/scripts.js`.
- Google Translate languages: `gTranslate.includedLangs` in `/Users/anurag/Desktop/CSVTU/scripts.js`.

**Notes**
- `index.html` is an extracted preview; it still contains Blogger tags and escaped entities that only resolve on Blogger.
- `styles.css` and `scripts.js` are derived artifacts; `csvtu.xml` is the source of truth for Blogger.

**License**
- No license file is present. Add one if you want explicit usage terms.
