# sebi.tools

[Open the website](https://sebidc.github.io/sebi.tools/)

A collection of 16 browser tools in Everforest Dark Soft and light themes, with Agrandir headings and Gramatika body text.

## Tools

- Direct-file downloader (sources must allow browser access)
- QR generator: links, text, Wi-Fi, email, custom colors, dots, and logo
- PNG / JPEG / WebP conversion, compression, resizing, social crops, watermarking, transparency trimming
- Palette extraction and WCAG contrast checks
- PDF merging, page extraction/reordering, and images to PDF
- DOCX / TXT / Markdown / HTML to plain text or text-based PDF
- Audio/video conversion, audio extraction, and short video to GIF
- SRT / WebVTT subtitle conversion

## On your device

Selected files are processed in your browser and are not uploaded. Libraries, fonts, and the media engine are served from this repository. No third-party conversion service or API key is used. Download links contact the source you enter. GitHub Pages still receives ordinary requests for the site assets.

Use short clips on iPhone. Media conversion loads a 31 MB single-thread WebAssembly engine and has an 80 MB input limit; actual device memory can impose a smaller limit. Document conversion preserves text, not the original layout. This is not a complete CloudConvert replacement. YouTube/Instagram page downloading requires a separate backend and is not part of this browser-only release.

## Run on your own host

Serve the `web/` directory with any static HTTPS server. For local development:

```sh
python3 -m http.server 8767 --directory web
```

Open http://localhost:8767/. There is no build step or backend. GitHub Pages deploys `web/` using the included workflow whenever main changes. Tool URLs use hash routes so they work on static hosts.

## Edit

Tool definitions and behavior are in `web/app.js`; colors and responsive layouts are in `web/style.css`. Main page markup is in `web/index.html`. Theme choice uses the same `sebi-theme` preference as sebi.dc and sebi.emojis.

See [THIRD_PARTY.md](THIRD_PARTY.md) for bundled libraries and their source/license information. Brand fonts and character artwork belong to their respective owners; no new license for those assets is granted here.
