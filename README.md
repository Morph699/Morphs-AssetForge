<img width="1024" height="1536" alt="AssetForge" src="https://github.com/user-attachments/assets/b2dd416c-5f75-4ef8-9f07-2ea59ad67bf4" />

# Morphs AssetForge & Icon Master (v3.1)
**Product ID:** 4 | **Ecosystem Symbol:** `&` | **Platform:** Windows Desktop Native & Hybrid Web/PWA

---

### Overview
**Morphs AssetForge & Icon Master** is a high-performance, air-gapped asset processing and icon generation workstation engineered to run seamlessly across Windows desktop environments and mobile hybrid web containers. Designed for independent developers, UI/UX designers, and technical creators, it transforms raw imagery into production-ready digital assets, multi-resolution application icons, and vector paths without external cloud dependencies or server-side data routing.

---

### Core Processing Engines & Capabilities

#### 1. Resilient Memory Shield Ingestion Pipeline
* **High-DPI & DSLR Safety Net:** Automatically inspects incoming bitmap payloads and downsamples inputs exceeding 1024×1024 px to prevent mobile GPU out-of-memory stalls, canvas crashes, or desktop GDI+ memory leaks.
* **Format Agnostic:** Natively ingests PNG, JPEG, WEBP, and BMP formats with instant viewport mapping and aspect ratio preservation.

#### 2. 3D Euclidean Chroma Knockout Engine
* **Precision Transparency Removal:** Strips solid, studio, or keyed backgrounds directly in RAM using 3D Euclidean color distance calculations:
  $$\text{Distance} = \sqrt{(R - R_{\text{target}})^2 + (G - G_{\text{target}})^2 + (B - B_{\text{target}})^2}$$
* **Fine-Tuned Edge Blending:** Features continuous real-time chroma tolerance controls (5–160) paired with an 8× linear falloff feathering slider (0–15 px) for anti-aliased edge smoothing.
* **Non-Destructive Buffer Revert:** Preserves master bitmap streams in volatile memory, enabling instant, one-click stage rollbacks without re-importing the source file.

#### 3. Precision Canvas Resizer & Preset Matrix
* **Arbitrary Dimension Scaling:** Scale dimensions smoothly between 16×16 px and 4096×4096 px using high-quality bicubic interpolation and smoothing filters.
* **Instant Target Presets:** One-touch sizing triggers for standard production targets, including **256²**, **512²**, and **1024²**.
* **Distortion & Upscale Radar:** Automatic threshold warning system that alerts users when scaling factors exceed 2.2× to prevent unwanted rasterization blur or artifacting.

#### 4. Dominant Palette Quantization Studio
* **Discrete Color Grouping:** Scans active raster bitplanes, quantizes non-transparent pixels into 32-step color clusters, and isolates the top 6 dominant color values.
* **Interactive Hex Swatches:** One-tap copying of any quantized color swatch directly to the system clipboard.
* **One-Click CSS Variable Generator:** Formats the entire active color scheme into copy-ready `:root { --color-1: #HEX; ... }` stylesheets for web and UI workflows.

---

### Multi-Format Export Pipelines

* **Master Clean PNG:** Full-fidelity 32-bit ARGB raster export preserving all transparency knockout and dimension adjustments.
* **App Icon Standard (512×512 PNG):** Production-standard store listing icon processed through bicubic scaling filters.
* **Web Favicon (32×32 PNG):** Downscaled, pixel-aligned browser favicon for immediate web deployment.
* **Windows Multi-Resolution Icon (`.ico`):** Packs 7 discrete mipmap frames into a single compound binary file:
  `16×16`, `24×24`, `32×32`, `48×48`, `64×64`, `128×128`, and `256×256`  
  Constructs genuine `ICONDIR` and `ICONDIRENTRY` headers with zero command-line conversion tools required.
* **Vector Path Tracer (`.svg`):** Raster-to-vector tracing module that analyzes canvas alpha thresholds and emits compact, scalable SVG compound paths.

---

### Local Asset Vault & Operational Tooling

* **Integrated Storage Vault:** Stores processed files locally (via desktop filesystem or in-browser IndexedDB) with detailed metadata, dimensions, timestamps, and live visual thumbnails.
* **Direct File System Bridges:** Open assets directly in default system editors, reveal items highlighted in Windows File Explorer, or copy file paths in a single click.
* **Comprehensive Telemetry Buffer:** Dedicated real-time diagnostic log documenting ingestion dimensions, knockout parameters, resize steps, and export activities with quick-copy and `.txt` log export tools.
* **Universal Dual-Persistence Engine:** Saves configuration states, window bounds, splitter positions, active themes, and typography preferences across local directories and user roaming profiles.
