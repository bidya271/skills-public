---
name: luxury-book-cover-designer
description: Generate publication-ready luxury front and back book covers with custom fine-art Chiaroscuro illustration, 3D gold-leaf typography, and compliant KDP barcode zones.
---

# Luxury Book Cover Designer

Produce publication-grade front and back book covers engineered for Amazon KDP, IngramSpark, and digital storefronts. Combines generative fine-art architectural matte painting with precision browser-rendered typography and dark barcode clearance zones.

## Overview & Architecture

Standard AI image generators struggle to render clean typography, consistent series branding, or barcode-safe layout zones.

This skill executes a decoupled two-stage publishing pipeline:
1. **Fine-Art Focal Stage:** Generates a high-resolution, prompt-engineered fine-art centerpiece (Chiaroscuro, classical architecture, atmospheric god-rays, or symbolic iconography) with dedicated negative space reserved at the top and bottom.
2. **Precision Typographic Composition Stage:** Uses headless Chromium with modern CSS (multi-stop gold foil gradient text clipping, Cinzel/Cormorant typography, and layered depth vignettes) to render exact print-dimension covers (848 × 1264 px trade ratio).

## Capabilities

- **Front Cover Master:** Generates framed or unframed fine-art covers with dual-stop vignettes and 3D metallic gold-leaf text effects.
- **Back Cover Engine:** Generates compelling narrative sales blurbs, 5 key thesis bullet points, author brand mark, and a subtle dark clearance zone reserved for Amazon KDP barcodes (no jarring white blocks).
- **Exact Ratio Adherence:** Defaults to standard 5.5" × 8.5" trade paperback / hardcover trim ratios (848 × 1264 px).

## Step-by-Step Implementation

### Step 1: Generate Chiaroscuro Artwork
Prompt your image generation tool or subagent:
```text
A monumental classical Greco-Roman architectural staircase rising out of dark mist and stormy clouds toward a luminous, unreachable golden apex. A solitary dark-cloaked traveler ascends in deep chiaroscuro. Leave the top 35% and bottom 20% dark and uncluttered for typography. Aspect ratio 5.5:8.5.
```

### Step 2: Render Front Cover HTML
```html
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<style>
@import url('https://fonts.googleapis.com/css2?family=Cinzel:wght@700;900&family=Cormorant+Garamond:ital,wght@1,500;1,600&family=Montserrat:wght@600;700&display=swap');
body { width: 848px; height: 1264px; overflow: hidden; background: #000; position: relative; font-family: 'Cinzel', serif; }
.bg-image { width: 100%; height: 100%; object-fit: cover; }
.vignette-top { position: absolute; top: 0; left: 0; width: 100%; height: 480px; background: linear-gradient(180deg, rgba(3,4,7,0.98) 0%, rgba(3,4,7,0.90) 40%, transparent 100%); pointer-events: none; }
.title-primary { font-size: 74px; font-weight: 900; letter-spacing: 0.16em; background: linear-gradient(180deg, #FFFFFF 0%, #F5E6BA 25%, #D4AF37 55%, #B38318 85%, #6E4B06 100%); -webkit-background-clip: text; -webkit-text-fill-color: transparent; filter: drop-shadow(0 6px 20px rgba(0,0,0,0.98)); text-transform: uppercase; }
</style>
</head>
<body>
  <img class="bg-image" src="cover_art_clean.jpg" />
  <div class="vignette-top"></div>
  <!-- Typography layers -->
</body>
</html>
```

### Step 3: Render Back Cover with Dark Barcode Zone
```html
<div class="amazon-barcode-clearance" style="width: 250px; height: 140px; border: 1px dashed rgba(212, 175, 55, 0.25); border-radius: 4px; background: rgba(8, 11, 16, 0.65); box-shadow: inset 0 0 15px rgba(0,0,0,0.6); pointer-events: none;"></div>
```

### Step 4: Headless Chrome Compilation
```bash
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" \
  --headless --disable-gpu --window-size=848,1264 \
  --screenshot="cover.jpg" "file://$(pwd)/cover.html"
```

## License
MIT License
