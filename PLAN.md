# The Balanced Tank — Minimal Aquarium Blog Plan

A minimal, sleek site to share your aquarium hobby with family: tank inhabitants, how they interact, and care notes—with videos, images, and clear info sections.

---

## 1. Design direction (minimal & sleek)

- **Palette**: Keep your current deep blue (`rgb(26, 22, 50)`) as base. Add:
  - Soft neutrals for text (off-white / light gray).
  - One accent (e.g. teal or soft green) for links, highlights, and “tank” feel.
- **Typography**: One clean sans-serif (e.g. system stack or a single Google Font like **DM Sans** or **Outfit**) for headings and body; consistent sizes and line-height.
- **Layout**: Plenty of whitespace, clear hierarchy, no clutter. Optional subtle gradients or very light texture for depth.
- **Media**: Large, crisp images and embedded videos; consistent aspect ratios and spacing.

---

## 2. Site structure (minimal pages)

| Page        | Purpose |
|------------|--------|
| **Home**   | Short intro, hero image/video, links to Tank Overview and Latest updates. |
| **Tank overview** | One place that explains what’s in the tank and how things interact (fish, plants, invertebrates, equipment). |
| **Inhabitants** | Sections or cards per species/group: name, photo, short description, role in the tank. |
| **Updates / journal** (optional) | Chronological posts: new additions, changes, water params, short videos. |
| **About / care** (optional) | Brief “how I care for this tank” for family who might be curious. |

Start with **Home + Tank overview + Inhabitants**; add Updates and About later if you want.

---

## 3. Content types to support

- **Videos**: Short clips (feeding, behavior, tank tour). Use `<video>` (self-hosted) or embed (e.g. YouTube/Vimeo unlisted) with a simple wrapper for consistent width and aspect ratio.
- **Images**: Full-width or grid for inhabitants, plants, and full-tank shots. Use `<picture>` or `srcset` later if you want responsive images.
- **Info sections**: Clear headings and short paragraphs; optional expandable “read more” for longer notes.
- **“How they interact”**: Dedicated section (on Tank overview or Inhabitants) explaining relationships: who eats what, who cleans what, plant/cycle role, etc. Use short bullets or a simple diagram (e.g. arrows or a list).

---

## 4. Technical approach (minimal stack)

- **HTML/CSS only** to start: semantic HTML5, one main stylesheet, no build step.
- **Structure**:
  - `index.html` — Home.
  - `tank-overview.html` — What’s in the tank and how it all interacts.
  - `inhabitants.html` — Species/group pages or one long page with sections.
  - Optional: `updates.html`, `about.html`.
- **Assets**:
  - `images/` — Photos (optimize size before adding).
  - `videos/` — Short clips, or use embed links only.
  - `style.css` — Global styles; optional `pages/` or section-specific CSS later if needed.
- **Responsiveness**: Mobile-first; breakpoints for tablet/desktop so layout and typography stay minimal and readable.

---

## 5. Implementation phases

### Phase 1 — Foundation (1–2 sessions)
- [ ] Set up folder structure: `images/`, `videos/` (if self-hosting).
- [ ] Define CSS variables: colors, font family, spacing, max-width for content.
- [ ] Build a simple header (site name + nav) and footer (e.g. “The Balanced Tank” + year).
- [ ] Style the home page: hero area, title, 1–2 sentences, link to Tank overview.

### Phase 2 — Tank overview & “how it interacts”
- [ ] Create `tank-overview.html` with sections: Equipment, Plants, Fish, Invertebrates (or your real categories).
- [ ] Add one “How they interact” section: short bullets or numbered steps (e.g. plants → oxygen/cleanup; snails → algae; fish → waste → cycle).
- [ ] Reuse header/footer; apply same minimal styling.

### Phase 3 — Inhabitants
- [ ] Create `inhabitants.html` (or one section per species if you prefer separate pages).
- [ ] For each inhabitant: image, name, 1–2 sentence description, “role in tank” line.
- [ ] Optional: simple card layout (image + text) that stacks on mobile and grids on desktop.

### Phase 4 — Media (videos & images)
- [ ] Add 1–2 hero or full-tank images on Home and Tank overview.
- [ ] Add one short video (embed or `<video>`) on Home or Tank overview.
- [ ] Add inhabitant photos to each card/section.
- [ ] Standardize image sizes and video aspect ratio in CSS.

### Phase 5 — Polish
- [ ] Responsive check: nav, typography, images, and video on phone/tablet.
- [ ] Optional: light animations (e.g. fade-in on scroll, or hover on cards).
- [ ] Favicon and meta description for sharing.
- [ ] Optional: Updates page and About/Care page when you’re ready.

---

## 6. Content checklist (for you to fill in)

- [ ] 1–2 sentences for “What is The Balanced Tank” (home).
- [ ] List: fish, plants, inverts, key equipment.
- [ ] Short “how they interact” notes (who does what, cycle, feeding).
- [ ] 3–5 photos: full tank, key inhabitants.
- [ ] 1–2 short videos (e.g. 30–60 seconds): tank tour or feeding.

---

## 7. File structure (target)

```
thebalancedtank/
├── index.html
├── tank-overview.html
├── inhabitants.html
├── style.css
├── images/
│   ├── hero-tank.jpg
│   └── ...
├── videos/          (optional, if self-hosting)
│   └── ...
└── PLAN.md          (this file)
```

---

You can start with **Phase 1** (foundation + home) and then add Tank overview and Inhabitants. If you tell me which phase you want to do first, I can turn this into concrete HTML/CSS changes step by step.
