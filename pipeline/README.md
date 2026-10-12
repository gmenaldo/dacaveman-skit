# DaCaveman Video Pipeline

Open-source, self-hosted pipeline for turning the skit into video. No paid APIs required.

## Recommended stack

1. **Toonflow** (https://github.com/HBAI-Ltd/Toonflow-app) — open-source AI short-drama platform. Handles script import, storyboarding, character and scene asset management, image generation, and video generation on an infinite canvas. Best fit for a multi-scene comedy skit.
2. **ComfyUI** (https://github.com/comfyanonymous/ComfyUI) — node-based UI for running local video models.
3. **Wan 2.2** or **LTX-Video** — open-source text-to-video and image-to-video models. Wan 2.2 is the current quality leader for open models; LTX-Video is faster and lighter.
4. **Open-Generative-AI** (https://github.com/Anil-matcha/Open-Generative-AI) — self-hosted studio with 600+ models including Wan, Flux, and Kling alternatives, if you want a browser-based all-in-one.

## Workflow

1. Import the script from `script/dacaveman-skit.md` into Toonflow.
2. Define characters: Dan DaCaveman, Tom DaCaveman, shop workers, owner, female cavewoman.
3. Generate character reference images first (consistent faces across scenes).
4. Break each scene into shots; write prompts per shot.
5. Generate images, then animate with image-to-video.
6. Assemble the timeline and export.

## Hardware note

Wan 2.2 and LTX-Video run locally on a machine with a decent GPU (12GB+ VRAM recommended). CPU-only is possible but very slow.

## DaCaveman Video Producer bot

The Grok Bot named "DaCaveman Video Producer" in George's App Lab is set up to break scripts into shot lists and write optimized prompts for these models. Ask it to process `script/dacaveman-skit.md`.
