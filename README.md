# Sphotik Quote Studio

Internal tool for generating branded literary quote cards for Sphotik Library social media channels.

**Live App:** [https://sphotik-quote-studio.pages.dev](https://sphotik-quote-studio.pages.dev/)

## Overview

Sphotik Quote Studio renders social media quote graphics (`1080x1080` and `1080x1350` JPEG) directly in the browser using the HTML5 Canvas API. It bundles Sphotik's brand assets and self-hosted fonts (`Fraunces` and `Noto Serif Bengali`) so exports remain consistent across devices without requiring a backend.

## Features

- **Quote & Attribution:** Supports Bengali and English text with adjustable font size, author name, and book title/subtitle.
- **Author Portrait Framing:** Image upload with zoom, pan (X/Y), and grayscale/color toggle.
- **Themes:** Sphotik Forest (`#154131`), Vintage Paper (`#f6f3eb`), Deep Ink (`#0c1612`), and Crisp White (`#ffffff`).
- **Layouts:** Editorial, Center Portrait, and Split Frame.
- **Export:** High-resolution JPEG (`0.98` quality) in `1:1` square or `4:5` portrait aspect ratios.

## Local Usage

This is a static application with no build step or dependencies.

```bash
git clone https://github.com/isthisdeception/sphotik-quote-studio.git
cd sphotik-quote-studio
```

Open `index.html` in any browser.

## Deployment

Hosted on Cloudflare Pages (`sphotik-quote-studio.pages.dev`) directly from the `main` branch with no build command and root (`/`) as the output directory.
