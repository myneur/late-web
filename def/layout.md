# Layout and Style Guide (Simply Late App)

## 1. Page Structure & Components

### Global Layout
- **Containers:** 
    - Default width: 100% with `24px` padding.
    - Max-widths: `1000px` (Desktop), `1160px` (Large), `1280px` (Extra Large).
    - Centered with `margin: 0 auto`.
- **Sections:**
    - Standard Padding: `100px 0` (`var(--spacing-lg)`).
    - Compact Padding: `30px 0` (`.section-compact`).
    - Flush (No Padding): `0` (`.section-flush`).
    - Backgrounds: White (default) or Light Gray (`var(--color-light-bg)`).

### Typography
- **Primary Font:** 'Karla', sans-serif (Body).
- **Secondary Font:** 'Old Standard TT', serif (Headings).
- **Heading Font:** 'Cabin', sans-serif (Alternative).
- **Base Size:** 1.6 line-height.
- **Paragraphs & Lists:** `1.25rem` size, `1.5rem` bottom margin.
- **Headings:**
    - **H2:** Responsive `clamp(2rem, 6vw, 3.5rem)`.
    - **H3:** Responsive `clamp(1.5rem, 4vw, 2.25rem)` (50% larger than base).
- **Links:**
    - Default: Inherit color, no decoration.
    - Inside `.container`: Underlined (`text-decoration: underline`).
    - Navigation/Buttons: No decoration.
    - Hover: `var(--color-primary)`.

### Header (Navigation)
- **Sticky Header:** White background, `20px` padding, `z-index: 1000`.
- **Logo:** 'Old Standard TT', `32px`, Bold.
- **Nav Links:** Flex row, `32px` gap. Hidden on mobile (`< 768px`).

### Hero Section (`.hero`)
- **Structure:** Full-width background image (`.hero-bg`) + Content Container below (`.hero-content-overlay`).
- **Card:** Full-width white background, `48px` padding (desktop) / `24px` (mobile).
- **Content:** Left-aligned H3 headline, bulleted list (styled with custom color bullets), and CTA button.

### Slider Section (`.slider-section`)
- **Layout:** Horizontal scroll container (`.slider-container`).
- **Items (`.slider-item`):**
    - Desktop: Fixed width `430px`, centered snap.
    - Mobile: `49%` width, centered snap.
- **Padding:** `50px 0` (50% of standard).

### Feature Grid (`.grid-2`)
- **Layout:** 2 Columns on desktop (`min-width: 768px`), 1 Column on mobile.
- **Alignment:** Top-aligned (`align-items: start`).
- **Gap:** `48px`.
- **Usage:** "Google Calendars & Weather", "Battery Life".

### Flavors Grid (`.grid-3`)
- **Layout:** 3 Columns on desktop, 1 Column on mobile.
- **Cards:** Centered text, square image container (`aspect-ratio: 1/1`, `object-fit: cover`).

### Explanation Images
- **Layout:** Full-width grid (`.explanation-images`).
- **Columns:** 2 Equal columns on desktop, 1 column on mobile.
- **Gap:** `0` (Seamless).

### Footer
- **Style:** Light gray background, `80px` padding, centered text.
- **Links:** Flex wrap, `24px` gap, `14px` size.
- **Copyright:** `12px` size, gray text.

### Utility Classes
- `.text-primary`: Teal color (`#00A0AA`).
- `.text-center`: Center alignment.
- `.text-right`: Responsive alignment (Center on mobile, Right on desktop > 768px).
- `.mt-1` / `.mt-2` / `.mb-2`: Standardized margins (`16px`, `24px`, `64px`).
- `.img-responsive`: Max-width 100%, height auto.
- `.img-max-400`: Cap width at 400px.

---

## 2. Color Palette & Variables

```css
:root {
    --color-primary: #00A0AA;
    --color-primary-hover: #00828A;
    --color-text: #1b1b1b;
    --color-bg: #FFFFFF;
    --color-light-bg: #f5f5f5;
    --font-primary: 'Karla', sans-serif;
    --font-secondary: 'Old Standard TT', serif;
}
```

## 3. Key Principles for New Pages
1.  **Semantic HTML:** Use `<section>`, `<header>`, `<footer>`, `<main>`.
2.  **No Inline Styles:** Use utility classes (`.mt-1`, `.text-right`, `.section-flush`) instead of `style="..."`.
3.  **Responsive First:** Build for mobile (single column) and expand to grid (`.grid-2`, `.grid-3`) on desktop.
4.  **Lazy Loading:** Always add `loading="lazy"` to images below the fold.
5.  **Inheritance:** Let typography inherit from `body` and container rules; avoid overriding font sizes manually on elements unless using semantic tags (H2, H3).