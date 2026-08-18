# Siril Scripts for Windows

A collection of astrophotography scripts and Python tools for **Siril**, prepared for **Windows** and created by **ag_astrophotography**.

The goal of this repository is to provide practical tools for common astrophotography workflows such as **2× drizzle**, **channel processing**, **OSC channel extraction**, and **professional astronomical annotation**.

> Designed for Siril 1.4.x / Siril 1.4.4 Stable on Windows.

---

## Included tools

| Tool | Version | Description |
|---|---:|---|
| **2× Drizzle Mono** | v1.0 | 2× drizzle workflow for mono data, including Full and From Masters variants. |
| **2× Drizzle OSC** | v1.0 | 2× drizzle workflow for OSC / CFA data while preserving the Bayer pattern until drizzle. |
| **Astro Channel Processor** | v1.5 | Python GUI for processing and combining LRGB, SHO and HOO channels inside Siril. |
| **OSC Channel Extractor** | v1.0 | Extracts and processes individual channels from OSC image data. |
| **AG Astro Annotator** | v2.8 | Creates professional RA/Dec grids, catalog labels, object markers, compass overlays and exportable annotations. |

---

## AG Astro Annotator

**AG Astro Annotator** is a Siril-based annotation tool for plate-solved astrophotography images.

### Features

- RA / Dec coordinate grid
- Siril-like automatic grid spacing
- Adaptive coordinate-label placement based on image orientation
- Separate horizontal and vertical grid colors
- Messier, NGC, IC, Sharpless / Sh2 and LDN catalog support
- Automatic catalog object size markers when diameter data is available
- Custom objects using X/Y or RA/Dec coordinates
- Custom circles, boxes, crosshairs and text annotations
- Adjustable North / East compass
- Siril plate-solving support
- Zoomable and pannable preview
- Siril AutoStretch preview
- Transparent overlay export as PNG or TIFF
- Complete annotated image export
- Presentation FITS export

The bundled annotation catalogs work offline.

---

## Installation on Windows

### Siril `.ssf` scripts

Download the ZIP for the script you want, extract it, and copy the included `.ssf` files to:

```text
C:\Program Files\Siril\scripts
```

Administrator permission may be required.

Restart Siril or refresh the script list afterwards.

---

### Python tools

The Python-based tools include a Windows installer:

```text
INSTALL_TO_SIRIL.bat
```

### Recommended installation

1. Download the ZIP for the tool you want.
2. Extract the ZIP.
3. Double-click `INSTALL_TO_SIRIL.bat`.
4. Approve the Windows administrator prompt if requested.
5. The installer copies the required files to:

```text
C:\Program Files\Siril\scripts
```

6. Restart Siril.
7. Open **Scripts → Python Scripts**.

The tool should now appear in Siril.

---

## Windows security note

Windows may display a SmartScreen warning for downloaded `.bat`, `.py`, or ZIP files.

If you trust the files downloaded from this repository:

1. Choose **More info** if SmartScreen appears.
2. Select **Run anyway**.
3. Approve the administrator prompt if required.

No separate Python installation is normally required for Siril Python scripts when using a supported Siril installation.

---

## Downloads

The latest Windows packages are available from the **Releases** section of this repository.

Recommended release assets:

```text
2xDrizzle_Mono_by_ag_astrophotography_v1.0.zip
2xDrizzle_OSC_by_ag_astrophotography_v1.0.zip
Astro_Channel_Processor_Siril_v1.5.zip
OSC_Channel_Extractor_by_ag_astrophotography_v1.0.zip
AG_Astro_Annotator_Siril_v2.8.zip
```

---

## 2× Drizzle workflows

### 2× Drizzle Mono

Designed for monochrome data and available in two workflow variants:

- **Full** – complete processing workflow
- **From Masters** – starts from existing master calibration frames

### 2× Drizzle OSC

Designed for one-shot-color / CFA data.

The Bayer / CFA structure is preserved until the drizzle stage so the data is handled correctly before debayering.

---

## Astro Channel Processor

A native Siril Python GUI designed for multi-channel astrophotography workflows.

Supported combinations include:

- **LRGB**
- **SHO**
- **HOO**

It provides a simple interface for selecting channel files and performing common channel-processing steps directly from Siril.

---

## OSC Channel Extractor

A Siril Python tool for extracting individual channels from OSC image data.

Useful for workflows where separate channel data is required for further processing, recombination, or experimentation inside Siril.

---

## Compatibility

These scripts were prepared for:

- **Siril 1.4.x**
- **Siril 1.4.4 Stable**
- **Windows**
- Siril Python scripts using `sirilpy`

The Windows packages are separate from the macOS releases to keep installation simple and platform-specific.

> If you discover a Windows-specific issue, please open a GitHub Issue and include your Windows version, Siril version and the affected script.

---

## Repository structure

```text
siril-scripts/
├── 2x Drizzle Mono
├── 2x Drizzle OSC
├── Astro Channel Processor
├── OSC Channel Extractor
└── AG Astro Annotator
```

Release ZIP files can be kept in **GitHub Releases**, while the repository itself can contain documentation, screenshots and source files.

---

## About

Created for astrophotographers who want a straightforward workflow inside Siril without having to move every processing step to separate software.

Developed by **ag_astrophotography**.

Instagram: **@ag_astrophotography**

---

## License

This project is released under the **MIT License**.

You are free to use, modify and redistribute the code under the terms of the license.

---

## Support & feedback

Found a bug, have a workflow idea, or want to suggest a new feature?

Please open an **Issue** in this repository.

Clear screenshots, Siril console output and a short description of the workflow are especially helpful when reporting problems.

---

### Clear skies ✨
