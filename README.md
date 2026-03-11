# Anime Image Generator

This repository provides a Google Colab notebook that launches a Gradio-based web interface for generating anime images with a diffusion model. The notebook is designed to run directly in Colab without local setup and includes the full workflow for checking GPU support, installing required packages, loading the model, and launching the interface.

<p align="center">
  <a href="https://huggingface.co/cagliostrolab">
    <img src="https://img.shields.io/badge/Model%20Author-Cagliostro%20Lab-blue?style=for-the-badge&logo=huggingface" alt="Model Author">
  </a>
  <a href="https://www.gradio.app/">
    <img src="https://img.shields.io/badge/Built%20With-Gradio-orange?style=for-the-badge&logo=gradio" alt="Built with Gradio">
  </a>
</p>

## Features

- Gradio-based image generation interface
- Runs entirely in Google Colab
- No local installation required
- Prompt-based anime image generation
- Multiple resolution options
- Seed control for reproducible results
- Optional save to Google Drive
- Public Gradio share link when launched in Colab

## Installation

### 1. Download the notebook

Download the `.ipynb` file from this repository.

### 2. Upload it to Google Colab

- Open Google Colab
- Click **Upload Notebook**
- Select the downloaded notebook file

### 3. Run the cells in order

Run the notebook cells from top to bottom.

The notebook workflow is:

1. **GPU Check**  
   Confirms that a compatible GPU is attached.

2. **Install**  
   Installs the required Python packages used by the notebook.

3. **Verify**  
   Checks that the required imports work correctly after installation.

4. **Load Model**  
   Downloads and loads the model into GPU memory.

5. **Launch UI**  
   Starts the Gradio interface for image generation.

## Important Notes

- Run the cells in the exact order shown in the notebook.
- After the install cell, Colab may restart the session. This is expected.
- Once the final cell runs, the Gradio interface will appear in the notebook.
- A public share link is also created when the interface launches.

## Recommended Colab Runtime

Use this runtime setting in Google Colab:

`Runtime -> Change runtime type -> GPU`

A T4 GPU is recommended for the notebook.

## How to Use

After the interface launches:

1. Enter a positive prompt
2. Enter a negative prompt
3. Choose a resolution
4. Adjust steps, CFG scale, and seed if needed
5. Click the generate button

The generated image will appear in the Gradio interface.

## Prompting

The interface is built for tag-based prompting. It works best with comma-separated tags instead of long natural-language sentences.

You can also use:

- positive prompts for what you want
- negative prompts for what you want to avoid
- seed values for repeatable outputs

## Saving Images

Generated images are saved inside the Colab environment.

The notebook also includes an option to save images to Google Drive if Drive is mounted.

## Disclaimer

This repository only provides a Colab notebook and Gradio interface for running the model.

All credit for the model goes to the original model authors. Please follow the model authors' licensing and usage terms.

## License

Refer to the model authors' pages for license and usage information.
