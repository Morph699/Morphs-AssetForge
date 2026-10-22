<img width="1328" height="1888" alt="AssetForge" src="https://github.com/user-attachments/assets/428679d3-c86b-4d00-b5af-2a12b35d10e6" />

Morphs Asset Forge & Icon Master (v2.26)

Lightweight Asset Transformation, Multi-Resolution Icon Packing & Chroma Studio

Overview

Morphs Asset Forge & Icon Master is an air-gapped, zero-latency graphics utility built for developers, designers, and creators who need clean assets, app icons, and favicons without the bloat of heavyweight editing suites.

Available as a native Windows desktop executable and a standalone, touch-optimized Android/Web workstation, Asset Forge handles background knockout, precision scaling, color palette quantization, vector path tracing,
and multi-resolution binary .ico bundling—entirely offline on your local hardware.

Core Capabilities & Features

  - 🛡️ Memory Shield Ingestion Engine: Automatically downscales oversized master inputs (>1024\text{px}) using bicubic interpolation, protecting device RAM and eliminating container out-of-memory crashes while preserving pixel fidelity.
  - ✨ Euclidean Chroma Knockout Studio: Rapidly key out backgrounds using true Euclidean RGB color distance with real-time chroma tolerance sliders (5–160) and smooth alpha edge feathering (0–15\text{px}). Revert to master frames non-destructively at any time.
  - 📐 Precision Canvas Resizer: Freely scale canvases from 16\text{px} up to 4096\text{px} with a 2.2\times pixel distortion radar and quick presets for 256^2, 512^2, and 1024^2 square standards.
  - 🎨 Extracted Dominant Palette Studio: Automatically clusters and quantizes the top 6 dominant colors from your image into interactive swatches with one-click CSS variable block generation (:root { --color-1: ... }).
  - 📦 Multi-Resolution Asset Export Matrix: 
      - Master Clean PNG: Full-fidelity transparent output.
      - App Icon Kit: Standardized 512 \times 512\text{px} production asset.
      - Web Favicon: Clean 32 \times 32\text{px} browser icon.
      - Windows .ICO (7 Sizes in 1 File): Bundles 16, 24, 32, 48, 64, 128, and 256\text{px} frames into a single binary-packed Windows icon file.
      - Vector .SVG Trace: Quantized boundary scanning that traces opaque alpha blocks (A > 128) directly into scalable <path> vectors.
  - 🗄️ Local Saved Asset Vault: High-speed local repository (IndexedDB on Web/Android, local app directory on Windows) with instant thumbnail previews, timestamps, direct downloads, and asset inspection.
  - 💾 100% Air-Gapped Universal Export: Direct Base64 data anchor downloads and touch-and-hold save hubs that bypass native container crashes with zero third-party cloud relays.
  - 🎨 10 High-Contrast Themes (WCAG AAA): Calibrated for maximum legibility across Light Slate, Dark Stealth, Matrix Green, Cyber Yellow, Cyberpunk Pink, Dracula Purple, Blood Matrix, Nordic Frost, Solarized Ocean, and
    Sunset Amber.
  - 🔤 4-Tier Responsive Font Scaler: Instant scaling across Small, Medium, Large, and Extra Large display tiers.
  - ⚡ Gothic Fade & Pulse Startup (Windows): Distinctive, pixel-locked startup screen with auto-discovery for AmericanText.ttf / Old English Text MT and a 7-color palette pulse.

Platform Availability

1.  Windows Native Desktop (AssetForge_Paid.ps1 / .exe):
      - Pure WinForms executable compiled via PS2EXE.
      - Multi-monitor bounds restoration and dual-persistence configuration engine (settings_paid.json).
      - Embedded dragon application icon and sub-second telemetry log buffer.
2.  Android & Web SPA (Morphs_AssetForge_Paid.html):
      - Mobile-first, responsive standalone PWA container.
      - Zero external npm or CDN dependencies—runs 100% offline in any modern browser or hybrid container.
