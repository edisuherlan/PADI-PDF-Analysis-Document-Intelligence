# PADI — PDF Analysis & Document Intelligence

**English** | [Bahasa Indonesia](#bahasa-indonesia)

Offline-first desktop app for PDF tools, conversion, OCR, and optional AI (chat, analysis, research).

**Author:** [Edi Suherlan](https://audhighasu.com) · [GitHub @edisuherlan](https://github.com/edisuherlan)  
**License:** MIT  
**Platform:** Windows 10/11 (64-bit) · Linux x86_64 (AppImage)

---

## Download

| Platform | Version | File |
|----------|--------:|------|
| **Windows** | **v1.1.0 (latest)** | [**PADI-Setup-1.1.0.exe**](https://github.com/edisuherlan/PADI-PDF-Analysis-Document-Intelligence/releases/download/v1.1.0/PADI-Setup-1.1.0.exe) |
| **Linux** | **v1.1.0 (latest)** | [**PADI-1.1.0-x86_64.AppImage**](https://github.com/edisuherlan/PADI-PDF-Analysis-Document-Intelligence/releases/download/v1.1.0/PADI-1.1.0-x86_64.AppImage) |
| Windows | v1.0.2 | [PADI-Setup-1.0.2.exe](https://github.com/edisuherlan/PADI-PDF-Analysis-Document-Intelligence/releases/download/v1.0.2/PADI-Setup-1.0.2.exe) |

All releases: [Releases](https://github.com/edisuherlan/PADI-PDF-Analysis-Document-Intelligence/releases)

> Installers are large (~180+ MB) because they include the Python runtime, Qt/PySide6, and PDF libraries.

---

## What's new in v1.1.0

- **PDF → Word:** convert PDFs to editable `.docx`, preserving layout where possible (with a text-only fallback).
- **Convert preview:** see the selected PDF/image right inside the Convert page before running.
- **Responsive UI:** layouts now adapt to different screen sizes and DPI — compact sidebar on narrow windows, scrollable pages, and consistent scaling across machines.
- **New settings:** choose a custom output folder, open results automatically after a task, plus clearer, more informative update options.
- **Optional AI toggle:** enable/disable AI features from Settings — PADI works fully for PDF tools & OCR offline, with AI menus hidden when turned off.

---

## Install — Windows

1. Download **PADI-Setup-1.1.0.exe**
2. Run the installer (admin may be required for Program Files)
3. Open **PADI** from the Start Menu or Desktop

### SmartScreen

If Windows shows *“Windows protected your PC”*: **More info** → **Run anyway**.

### Uninstall

**Settings → Apps → PADI → Uninstall**

---

## Install — Linux (AppImage)

1. Download **PADI-1.1.0-x86_64.AppImage**
2. Make it executable and run:
   ```bash
   chmod +x PADI-1.1.0-x86_64.AppImage
   ./PADI-1.1.0-x86_64.AppImage
   ```
3. Optional: move it to `~/Applications` or `/usr/local/bin`

**Notes**
- Works on most modern x86_64 distros (Ubuntu, Fedora, etc.) without a system Python install
- OCR uses system `tesseract` if installed (`sudo apt install tesseract-ocr tesseract-ocr-ind`), or PADI’s portable download when available
- For Office → PDF, install [LibreOffice](https://www.libreoffice.org/)

---

## System requirements

| | **Minimum** (runs) | **Recommended** (best performance) |
|--|--------------------|------------------------------------|
| **OS** | Windows 10/11 (64-bit) or Linux x86_64 | Same |
| **CPU** | Dual-core x86_64, 2.0 GHz | Quad-core x86_64, 2.5 GHz or faster |
| **RAM** | 4 GB | **8 GB** (PDF tools, OCR, convert, preview) |
| **Storage** | ~500 MB free (install + working space) | 1 GB+ free; **SSD** preferred |
| **Display** | 1280 × 720 | 1366 × 768 or higher |

**Optional AI (local Ollama):** add **8–16 GB RAM** depending on model size (e.g. ~8 GB for a 7B model). Cloud AI only needs a normal internet connection and an API key.

**Optional helpers:** [Tesseract](https://github.com/tesseract-ocr/tesseract) for OCR language packs · [LibreOffice](https://www.libreoffice.org/) for Office → PDF.

---

## Automatic updates

PADI can check [GitHub Releases](https://github.com/edisuherlan/PADI-PDF-Analysis-Document-Intelligence/releases) on startup and offer to download:

- **Windows:** Setup.exe installer  
- **Linux:** new AppImage  

Manual check: **About → Check for updates**. Toggle in **Settings**.

---

## What’s included

| Feature | Notes |
|---------|--------|
| **PDF Tools** | Join, merge, split, compress, rotate, watermark, password, metadata, and more |
| **PDF Editor** | Edit text, annotations, stamps, signatures, pages (offline) |
| **Convert** | PDF → Word (.docx), PDF ↔ images, text, Markdown, CSV, Excel, table extraction — with live file preview |
| **OCR** | Scan/image text; searchable PDF |
| **AI Analysis** | Summary, keywords, entities *(optional AI)* |
| **Chat PDF** | Ask questions about documents *(optional AI)* |
| **Research Assistant** | Gaps, methods, citations *(optional AI)* |
| **Knowledge Base** | Personal library + search |
| **UI languages** | English (default) and Indonesian |

App data: `%USERPROFILE%\.pdfmaster_ai\` (Windows) or `~/.pdfmaster_ai/` (Linux)

---

## Optional AI

Core PDF / Convert / OCR work **without** AI.

- **Ollama (local):** [ollama.com](https://ollama.com) — e.g. `ollama pull qwen2.5:7b`
- **Cloud:** set provider + API key in **Settings** (keys stay on your device)

---

## Bahasa Indonesia

**PADI** adalah aplikasi desktop untuk alat PDF, konversi, OCR, dan AI opsional. Platform: **Windows** dan **Linux (AppImage)**.

### Unduh

| Platform | Versi | File |
|----------|------:|------|
| **Windows** | **v1.1.0 (terbaru)** | [**PADI-Setup-1.1.0.exe**](https://github.com/edisuherlan/PADI-PDF-Analysis-Document-Intelligence/releases/download/v1.1.0/PADI-Setup-1.1.0.exe) |
| **Linux** | **v1.1.0 (terbaru)** | [**PADI-1.1.0-x86_64.AppImage**](https://github.com/edisuherlan/PADI-PDF-Analysis-Document-Intelligence/releases/download/v1.1.0/PADI-1.1.0-x86_64.AppImage) |

Semua rilis: [Releases](https://github.com/edisuherlan/PADI-PDF-Analysis-Document-Intelligence/releases)

### Install Windows

1. Unduh **PADI-Setup-1.1.0.exe**
2. Jalankan installer
3. Buka PADI dari Start Menu / Desktop

### Install Linux (AppImage)

```bash
chmod +x PADI-1.1.0-x86_64.AppImage
./PADI-1.1.0-x86_64.AppImage
```

Opsional OCR: `sudo apt install tesseract-ocr tesseract-ocr-ind`  
Opsional Office→PDF: LibreOffice.

### Persyaratan sistem

| | **Minimum** | **Direkomendasikan** (performa maksimal) |
|--|-------------|------------------------------------------|
| **OS** | Windows 10/11 (64-bit) atau Linux x86_64 | Sama |
| **CPU** | Dual-core x86_64, 2.0 GHz | Quad-core x86_64, 2.5 GHz ke atas |
| **RAM** | 4 GB | **8 GB** (PDF tools, OCR, konversi, preview) |
| **Penyimpanan** | ~500 MB bebas | 1 GB+ bebas; **SSD** lebih baik |
| **Layar** | 1280 × 720 | 1366 × 768 atau lebih tinggi |

**AI lokal (Ollama):** tambahkan **8–16 GB RAM** sesuai ukuran model. AI cloud hanya butuh internet + API key.

### Pembaruan otomatis

PADI dapat mengecek Release baru dan menawarkan unduhan Setup.exe (Windows) atau AppImage (Linux). Cek manual: **Tentang → Periksa pembaruan**.

---

## Support

- Website: [audhighasu.com](https://audhighasu.com)
- Issues: [GitHub Issues](https://github.com/edisuherlan/PADI-PDF-Analysis-Document-Intelligence/issues)
