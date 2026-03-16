# Image Generation Colab FAST

Fast Google Colab notebooks for anime and realistic image generation with a Gradio interface.

[![Gradio](https://img.shields.io/badge/Gradio-Website-orange?style=for-the-badge)](https://www.gradio.app/)
[![Google Colab](https://img.shields.io/badge/Platform-Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=black)](https://colab.research.google.com/)
[![Repository](https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github)](https://github.com/CookieFilled/Image-Generation-Colab-FAST)

This repository contains Google Colab notebooks for launching image generation workflows with a simple Gradio UI. The notebooks are designed for an easy upload-and-run flow in Colab, with GPU checks, package setup, model loading, and a ready-to-use interface.

---

## Models and Tools

[![Animagine XL 3.1](https://img.shields.io/badge/Model-Animagine%20XL%203.1-blue?style=for-the-badge)](https://huggingface.co/cagliostrolab/animagine-xl-3.1)
[![LUSTIFY v2.0](https://img.shields.io/badge/Model-LUSTIFY%20v2.0-purple?style=for-the-badge)](https://huggingface.co/TheImposterImposters/LUSTIFY-v2.0)
[![RealVisXL V5.0](https://img.shields.io/badge/Model-RealVisXL%20V5.0-green?style=for-the-badge)](https://huggingface.co/SG161222/RealVisXL_V5.0)

---

## Notebooks

### Anime Generator
**File:** `anime_nsfw_generator_v4.ipynb`  
Anime-focused image generation using Animagine XL 3.1.

[![Open in Colab](https://img.shields.io/badge/Open%20in-Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=black)](https://colab.research.google.com/github/CookieFilled/Image-Generation-Colab-FAST/blob/main/anime_nsfw_generator_v4.ipynb)

### Realistic Generator
**File:** `realistic_nsfw_generator_v1.ipynb`  
Photorealistic image generation powered by LUSTIFY v2.0.

[![Open in Colab](https://img.shields.io/badge/Open%20in-Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=black)](https://colab.research.google.com/github/CookieFilled/Image-Generation-Colab-FAST/blob/main/realistic_nsfw_generator_v1.ipynb)

### RealVisXL Generator
**File:** `realvisxl_nsfw_generator.ipynb`  
Realism-focused image generation using RealVisXL V5.0.

[![Open in Colab](https://img.shields.io/badge/Open%20in-Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=black)](https://colab.research.google.com/github/CookieFilled/Image-Generation-Colab-FAST/blob/main/realvisxl_nsfw_generator.ipynb)

### Additional Notebooks
- `roleplay_companion_final (1).ipynb`
- `roleplay_companion_v3 (1).ipynb`

---

## Features

- Runs entirely in Google Colab
- Gradio-based web UI
- No local installation required
- T4 GPU-friendly setup
- Guided notebook flow with clearly separated steps
- Cached model loading after first download
- Prompt, negative prompt, steps, CFG, resolution, and seed controls
- Optional Google Drive saving in supported notebooks
- Public Gradio share link when launched from Colab

---

## Quick Start

### 1. Pick a notebook
Choose the notebook that matches the style you want:
- `anime_nsfw_generator_v4.ipynb` for anime-style outputs
- `realistic_nsfw_generator_v1.ipynb` for realistic outputs
- `realvisxl_nsfw_generator.ipynb` for another realism-focused workflow

### 2. Open it in Google Colab
Use the **Open in Colab** button above, or download the notebook and upload it manually to Colab.

### 3. Enable GPU
In Colab, use:

`Runtime -> Change runtime type -> T4 GPU`

### 4. Run cells in order
Run the cells from top to bottom exactly as shown in the notebook.

The main notebooks follow this flow:

1. **GPU Check**
2. **Install**
3. **Verify**
4. **Load Model**
5. **Launch UI**

---

## Important Notes

- Run the cells in the exact order shown
- After the install cell, Colab may restart the kernel or show a session crashed popup
- This behavior is expected in these notebooks
- After restart, continue from the verify cell
- Do not re-run the install cell unnecessarily

---

## How to Use

After the UI launches:

1. Enter your prompt
2. Add a negative prompt if needed
3. Choose a resolution
4. Adjust steps, CFG, and seed
5. Click generate

The generated image will appear directly in the Gradio interface.

---

## Recommended Runtime

Use a **T4 GPU** in Google Colab for the intended workflow.

---

## Troubleshooting

### No GPU found
Make sure your Colab runtime is set to **T4 GPU**.

### Session restarted after install
This is expected. Click **OK** and continue from the next verification step.

### Gradio UI not showing
Make sure the model loaded correctly, then re-run only the final UI cell.

### Slow first launch
The first run downloads model files. Later runs are faster because cached files are reused.

---

## Repository Structure

```text
README.md
anime_nsfw_generator_v4.ipynb
realistic_nsfw_generator_v1.ipynb
realvisxl_nsfw_generator.ipynb
roleplay_companion_final (1).ipynb
roleplay_companion_v3 (1).ipynb
