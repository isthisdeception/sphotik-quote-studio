# Sphotik Quote Studio

**Sphotik Quote Studio** is a lightweight, zero-dependency, browser-based social media quote card generator built for **Sphotik Library (স্ফটিক — সদস্যভিত্তিক লাইব্রেরি · বাংলাদেশ)**. It enables instant creation of high-resolution literary quote graphics (`1080×1080` and `1080×1350` JPG) featuring author portraits, custom typography, and official Sphotik branding.

---

## ✨ Key Features

- **Real-Time Canvas Rendering:** Instant live preview powered by the HTML5 Canvas 2D API with zero server roundtrips.
- **Author Portrait Controls:**
  - Drag-and-drop or file-picker image upload (`JPG`, `PNG`, `WebP`).
  - **Classic B&W Literary Filter** (high-contrast grayscale) or **Full Color** mode.
  - Smooth **Zoom (`1.0x – 2.5x`)** and **X/Y Pan** sliders for precise framing.
  - Automatic fallback to author initials when no portrait is uploaded.
- **4 Signature Brand Themes:**
  - **Sphotik Forest (`#154131`):** Deep forest green canvas with warm gold accents and crisp white typography.
  - **Vintage Paper (`#f6f3eb`):** Warm editorial paper surface with deep green accents.
  - **Deep Ink (`#0c1612`):** High-contrast dark literary theme with amber highlights.
  - **Crisp White (`#ffffff`):** Minimalist clean gallery card aesthetic.
- **3 Editorial Layouts:**
  - **Editorial:** Oversized quotation mark, left-aligned quote, author badge, and branded footer.
  - **Center Portrait:** Circular author portrait centerpiece with centered quote and wordmark.
  - **Split Frame:** Magazine-style top header with large rectangular portrait frame.
- **Social-Ready Aspect Ratios:**
  - **1:1 Square (`1080 × 1080 px`)** — Ideal for Facebook & Instagram feeds.
  - **4:5 Portrait (`1080 × 1350 px`)** — Optimized for mobile feed engagement.
- **Offline & CORS-Safe Export:** Sphotik logos and self-hosted `Fraunces` & `Noto Serif Bengali` `.woff2` fonts are bundled locally so high-quality (`0.98` quality) `.jpg` exports work both offline (`file://`) and on any static host.

---

## 📁 Project Structure

```text
sphotik-quote-studio/
├── fonts/
│   ├── fraunces-latin-italic.woff2
│   ├── fraunces-latin-normal.woff2
│   └── noto-serif-bengali-400-normal.woff2
├── index.html       # Main application UI & Canvas rendering engine
├── logos.js         # Base64-encoded Sphotik brand marks for CORS-free Canvas export
├── logo.png         # Sphotik primary icon
├── logo-light.png   # Sphotik light/transparent icon
└── README.md        # Project documentation
```

---

## 🚀 Quick Start (Local Usage)

No build tools, `npm install`, or local server required:

1. Clone the repository:
   ```bash
   git clone https://github.com/isthisdeception/sphotik-quote-studio.git
   cd sphotik-quote-studio
   ```
2. Open `index.html` directly in any modern browser (Chrome, Edge, Firefox, Safari).
3. Enter the quote, author name, optional book title, upload the author's photo, and click **High-Quality JPG ডাউনলোড করুন**.

---

## ☁️ Deploying to Cloudflare Pages

Because this project is 100% static HTML/CSS/JS, deploying to **Cloudflare Pages** takes less than a minute:

1. Log in to the **Cloudflare Dashboard** and navigate to **Workers & Pages** → **Create** → **Pages** → **Connect to Git**.
2. Select the `isthisdeception/sphotik-quote-studio` repository.
3. Configure the build settings:
   - **Framework preset:** `None`
   - **Build command:** *(Leave empty)*
   - **Build output directory:** `/` *(or leave default)*
4. Click **Save and Deploy**.

---

## 🎨 Brand Guidelines

- **Primary Brand Color:** Sphotik Forest (`#154131`)
- **Accent Colors:** Warm Gold (`#f5c451`) & Literary Amber (`#e07a16`)
- **Typography:** `Fraunces` (Display / Latin) & `Noto Serif Bengali` (Bengali Literary Serif)

---

© **Sphotik Library (স্ফটিক)** · Dhaka, Bangladesh · [sphotik.com](https://sphotik.com)
