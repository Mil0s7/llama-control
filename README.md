🇵🇱 [Wersja polska](./README.pl.md)

# Llama Control

**Llama Control** is a free desktop app that helps you run and manage AI language models (like a local "ChatGPT") on your own hardware. No internet required after setup, no subscription, nothing sent anywhere else.

## How it works

AI models live locally on your disk as files. To make a model actually "come alive" and let you talk to it, you need an engine to run it. Llama Control uses **[llama.cpp](https://github.com/ggml-org/llama.cpp)**, one of the most popular open-source engines for running AI models locally.

Llama Control is a friendly **wrapper** around that engine:

- **Keeps track of your models.** Shows a list, their size, when they were downloaded, and lets you tag them as favorites or add notes.
- **Installs the llama.cpp engine for you** if you don't already have it, picking the right build for your graphics card.
- **Starts and stops a model with one click.** No typing anything into a console.
- **Lets you download new models** straight from HuggingFace (think of it as a "store" for AI models) and tells you right away whether a given model will fit in your GPU's memory.
- **Updates itself** whenever a new version comes out.

In short: you install it, the app figures out the rest, you just click.

### Why llama.cpp instead of Ollama or LM Studio?

This isn't meant to be another standalone AI engine competing with those. It's deliberately a **lightweight wrapper**, not a full application. Ollama and LM Studio are their own complete environments. They run in the background and use up memory and resources all the time, even when you're not doing anything. Llama Control doesn't have its own heavy engine running in the background. It simply turns `llama.cpp` on and off exactly when you want to use it, and doesn't eat your RAM or CPU/GPU power when you don't.

## What devices this works on

- **Windows only for now** (10 or 11): desktop or laptop. Doesn't work on phones or tablets.
- **An NVIDIA graphics card (GeForce/RTX) is recommended.** Models run fast with one. It still works without one, just slower (on the CPU alone).
- AI models can weigh from a few gigabytes to tens of gigabytes each, so it's worth having some free disk space.

### Planned

- Support for **AMD and Intel graphics cards** (currently works best with NVIDIA).
- Optimization and support for **macOS and Linux** (currently Windows only).

## Getting started

1. Download the latest installer from the **[Releases](../../releases)** tab on the right side of this page.
2. Run the downloaded `.exe` file.
3. Windows may show a blue warning screen ("Windows protected your PC"). That's normal for smaller independent apps without a paid signing certificate. Click **"More info" → "Run anyway"**.
4. Done. The app will guide you from there.
