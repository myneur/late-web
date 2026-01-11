# Layout Analysis: Settings Page (settings.html)

## 1. Hierarchy

### Section 1: Header (Navigation)
- Standard "simply late!" header.

### Section 2: Settings Browser (New Style)
- **Heading:** "Weather forecast & Google Calendar Settings: Open Garmin mobile Connect app and browse:"
- **Component:** Single Image Slider (Carousel).
- **Content:** Screenshots of the Garmin Connect app settings.
    - Likely images: `img/settings/Screenshot_*.jpg` series.

### Section 3: Compatibility
- **Text:** "Compatibility: only powerful watches like Garmin Forerunner 245~945, fēnix 5-6, Venu, vívoactive 3-4"
- **Link:** "See all compatible Garmin watches" (to `garmin-compatibility.html` or external).

### Section 4: Google Calendar Info (3-Column Grid)
- **Heading:** "Google Calendar" (Implicit or explicit section header).
- **Cards/Columns:**
    1.  **5-60 min to update:** Internet access limits, update frequency.
    2.  **Battery consumption:** Default settings efficiency, sensor warnings.
    3.  **Strong flavor limitations:** Display limitations for "Strong" flavor.
    4.  **Multiple calendars:** Adding extra calendars via IDs.
    5.  **Calendar colors:** Color coding logic.
    6.  **Reporting problems & Known bug:** Garmin bug info and voting link.

### Section 5: Weather Forecast Info (3-Column Grid)
- **Heading:** "Weather forecast"
- **Cards/Columns:**
    1.  **How the forecast updates:** Temp display, hourly updates.
    2.  **Forecast does not update?:** Troubleshooting connection and calendar blocking.
    3.  **Inaccurate forecast? Check location!:** GPS location, voting for bug fix, provider options (Yr.no vs Clear Outside).

## 2. New Design Components

### Single Image Slider
- Shows one full image at a time.
- Navigation arrows (Previous/Next).
- Dims or hides other images.

### Responsive 3-Column Grid
- Desktop (> 1024px): 3 Columns.
- Tablet (768px - 1023px): 2 Columns.
- Mobile (< 768px): 1 Column.

## 3. Image Mapping
- **Settings Screenshots:**
    - `img/settings/Screenshot_20210402-202929.jpg`
    - `img/settings/Screenshot_20210402-202942.jpg`
    - `img/settings/Screenshot_20210402-202949.jpg`
    - `img/settings/Screenshot_20210402-202958.jpg`
    - `img/settings/Screenshot_20210402-203008.jpg`
    - `img/settings/Screenshot_20210402-203015.jpg`
    - `img/settings/Screenshot_20210402-203038.jpg`
    - `img/settings/Screenshot_20210402-203047.jpg`
- **Other Images:** The text content seems to be text-only cards, but I should check if there are specific images associated with the grid items. The source analysis didn't show obvious images for the grid items, just the top slider.