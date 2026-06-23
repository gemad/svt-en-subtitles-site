---
title: SVT Play – English Subtitles
description: A privacy-first Chrome extension that uses on-device AI to translate Swedish subtitles to English in real time on SVT Play. No cloud APIs, no data collection — 100% local.
tags:
  - browser-extension
  - translation
  - privacy
link: https://chromewebstore.google.com/detail/svt-play-%E2%80%93-english-subtit/gmlibincdalncglkkneojolmpbbaehnf
featured: true
---

## What it does

SVT Play – English Subtitles is a Chrome extension that intercepts the Swedish subtitle stream on [svtplay.se](https://svtplay.se) and translates it to English in real time using a local neural machine translation model.

The translation runs entirely inside your browser via **WebAssembly (WASM)** — no text is ever sent to a cloud API. Your viewing habits and subtitle content stay completely on your device.

## Key Features

- **On-device translation** — powered by the Helsinki-NLP Opus-MT model via Transformers.js and ONNX Runtime
- **Zero cloud dependencies** — works offline after the initial model download
- **Real-time** — subtitles appear with under 2 seconds of latency
- **Customizable overlay** — adjust font size, layout (stacked/side-by-side), and position
- **Free** — completely free to use, open-source

## Privacy

No subtitle text, no URLs, no viewing habits, no personal data of any kind ever leaves your machine. The extension has no analytics, no crash reporters, and no third-party services.

## Installation

Install directly from the [Chrome Web Store](https://chromewebstore.google.com/detail/svt-play-%E2%80%93-english-subtit/gmlibincdalncglkkneojolmpbbaehnf). On first launch, the model (~150 MB) is downloaded once from Hugging Face's CDN and cached locally.

## Tech Stack

- [Transformers.js](https://huggingface.co/docs/transformers.js) — ML inference in the browser
- [ONNX Runtime Web](https://onnxruntime.ai/) — WASM execution backend
- Helsinki-NLP [Opus-MT](https://opus.nlpl.eu/) — Swedish→English translation model
