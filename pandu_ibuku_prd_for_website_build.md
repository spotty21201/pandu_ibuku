# PRD — Pandu Ibuku Website

## 0) Product Snapshot
**Product name:** Pandu Ibuku  
**Tagline:** *Sebuah Landasan untuk Bernalar dan Berinovasi*  
**Positioning:** Editorial-first personal thinking website by Mohamad Sriyanto (engineer; 35+ years in oil & gas, Indonesia). Calm, long-form reading environment. Not a blog/magazine, not a portfolio, not a startup site.

**Primary language:** Bahasa Indonesia (tone: “Spotty style” — clear, grounded, not overly formal, with selective English terms allowed when they improve clarity).  

---

## 1) Goals
### 1.1 Business / Outcome Goals
- Publish and organize Mohamad Sriyanto’s writings in a structured, credible, calm environment.
- Make it easy for the owner to add new posts (short notes or long essays) over time.
- Present five core themes as timeless domains while still showing posts chronologically (latest first).
- Support light, respectful discussion via comments (with moderation).

### 1.2 User Goals
- Readers quickly understand what Pandu Ibuku is within 10–20 seconds.
- Readers can browse by theme or by latest posts.
- Readers can read comfortably for long periods (high legibility, low distraction).

---

## 2) Non-Goals
- No social-media features (likes, reaction counts, “popular posts,” gamification).
- No aggressive CTAs, newsletters, or lead-gen funnels in v1.
- No heavy animations, visual noise, or complex UI patterns.

---

## 3) Target Users
1. **Primary:** Mohamad Sriyanto (site owner) — needs simple publishing workflow.
2. **Secondary:** General readers — friends, professional circles, family, public.
3. **Tertiary:** Commenters — respectful, topic-relevant responses.

---

## 4) Information Architecture (IA)
### 4.1 Primary Navigation (Header)
- Beranda
- Pandu Bangsaku
- Bilangan Prima, Angka, dan Logika
- Akhlak Mulia
- Catatan Kreatif
- Inovasi untuk Mobilitas
- Tentang Penulis

### 4.2 Secondary Navigation (Optional / v1 if easy)
- Arsip (chronological list)
- Pencarian
- Indeks Tema (tags)

---

## 5) Content Model & Taxonomy
### 5.1 Content Types
**A) Post (primary)**
- Title
- Date (published)
- Category (one of the five core themes)
- Optional tags
- Body content (rich text + images)
- Optional hero image (discouraged; use only when meaningful)
- Comments (enabled by default; moderation on)

**B) Page (static)**
- Beranda
- Category landing pages (intro + list)
- Tentang Penulis

### 5.2 Categories (fixed)
1. Pandu Bangsaku
2. Bilangan Prima, Angka, dan Logika
3. Akhlak Mulia
4. Catatan Kreatif
5. Inovasi untuk Mobilitas

### 5.3 Tags (optional)
Use tags for cross-cutting themes (e.g., “pendidikan,” “kebijakan,” “bilangan prima,” “etika,” “mobilitas,” etc.).

---

## 6) Page Requirements
### 6.1 Beranda (Home)
**Purpose:** Provide context quickly; invite calm exploration.

**Must include:**
- Masthead: “Pandu Ibuku”
- Tagline: “Sebuah Landasan untuk Bernalar dan Berinovasi”
- Short intro paragraph about the site’s purpose and the author
- Five theme entry cards/links (simple; no icons required)
- Latest posts list (latest first)

**Must avoid:**
- Slider, carousel, promo banners
- Dense widgets or sidebar blocks

### 6.2 Category Landing Pages (5 pages)
**Purpose:** Intro + chronological list of posts in that category.

**Must include:**
- Category title
- Short category intro (from the “Website Content” document)
- Post list (title, date, short excerpt)
- Pagination or infinite scroll (pagination preferred)

### 6.3 Post Page
**Purpose:** Long-form reading.

**Must include:**
- Title
- Date + category + optional tags
- Body text
- Subtle “Next / Previous” navigation
- Comments section (below content)

**Comments behavior:**
- Enabled by default
- Moderation ON
- Simple anti-spam (basic + honeypot; avoid aggressive captchas if possible)

### 6.4 Arsip (optional but recommended)
Chronological list across all categories, latest first.

### 6.5 Tentang Penulis
Use the content provided in the “Website Content” Canvas. Keep factual, restrained.

---

## 7) Editorial Design System (Hard Requirements)
This site must follow an editorial-first design philosophy.

### 7.1 Layout
- Single-column reading layout
- Generous margins
- Comfortable maximum line length
- No sidebars on post pages

### 7.2 Color Palette
- Background: warm off-white
- Primary text: charcoal (not pure black)
- Secondary text: soft gray for metadata
- Accent: deep navy OR muted dark blue (links + minimal emphasis)

Rules:
- No gradients
- No bright colors
- No heavy shadows

### 7.3 Typography
**Body text (priority):**
- Choose an extremely readable editorial font (serif or humanist serif).
- Slightly larger than typical web body size.
- Generous line-height.

**Headings:**
- Same family as body preferred, or restrained humanist sans if needed.
- Calm hierarchy; avoid display fonts.

**UI text:**
- Clean and small; no decorative styling.

### 7.4 Interaction
- No likes, view counts, “trending,” share widgets.
- Comments are subdued visually.
- Focus: reading, not engagement.

---

## 8) Logo Requirements
### 8.1 Logo Style
- Typographic wordmark only.
- Two-line masthead variant is allowed:
  - Line 1: “Pandu”
  - Line 2: “Ibuku”
- Editorial, restrained, print-like (avoid glossy effects).

### 8.2 Color Use
- Primary version: charcoal
- Secondary variant (optional): navy for “Ibuku” with reduced saturation
- Must work in **single-color** (charcoal) for maximum consistency.

### 8.3 Deliverables (for the build)
- Provide the logo as **SVG** (preferred) + PNG fallback.
- Provide 3 variants:
  1) Single-color (charcoal)
  2) Two-tone (charcoal + muted navy)
  3) Small/header compact version (same wordmark, reduced size)

**Insert logo:** Use the provided logo result as the reference target; recreate faithfully as SVG and apply the palette above.

---

## 9) Content Source (Must Use)
The site copy is already written.

**The developer must use the text from the Canvas document:**
- “Pandu Ibuku — Website Content” (actual website copy)

No placeholders. No lorem ipsum.

---

## 10) Admin / Authoring Requirements
### 10.1 Publishing Workflow
- Easy creation of new posts
- Support short notes and long essays
- Ability to upload images/diagrams (especially for “Inovasi untuk Mobilitas”)
- Simple editor (block editor or markdown) with clean typography

### 10.2 Moderation
- Comment moderation queue
- Basic spam protection

---

## 11) SEO & Sharing
- Clean URLs (slugs in Bahasa Indonesia allowed)
- Proper title tags and meta descriptions
- Open Graph tags for sharing
- RSS feed (recommended)

No “share counters.”

---

## 12) Performance & Accessibility
- Fast loading
- Minimal JS
- Mobile-first responsive
- High contrast and readable font sizes
- Semantic HTML structure

---

## 13) Implementation Options (Choose One)
### Option A — WordPress (recommended if the owner wants simplicity)
- Use posts + categories + tags
- Create pages for Beranda, Tentang Penulis, and category landing pages
- Keep theme minimal; strip unnecessary widgets

### Option B — Static Site + CMS (recommended if you want maximum speed + control)
- Content managed via markdown + lightweight CMS
- Same IA and templates

Regardless of option, the design constraints above must be respected.

---

## 14) Acceptance Criteria (Checklist)
- Navigation matches IA exactly.
- Beranda explains purpose quickly and links to five themes.
- Category pages: intro + chronological post list.
- Post pages: single-column; no sidebar; readable typography; subdued comments.
- Color palette is restrained and consistent.
- Logo appears as typographic masthead and works in one color.
- Content is fully populated from the provided Website Content text.
- New posts can be added without developer help.

---

## 15) Future Enhancements (Post-v1)
- Indeks Tema (tag directory)
- Selected essays / curated list
- Simple search improvements
- Diagram style guide for mobility sketches

---

## 16) Open Questions (for the developer to confirm)
1. Preferred build path: WordPress vs Static+CMS?
2. Do we want a dedicated “Arsip” page in v1?
3. Should comments be enabled by default on every post, or only selected posts?
4. Any domain / hosting constraints?

End of PRD.

