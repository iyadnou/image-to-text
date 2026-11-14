# Image to Text (Image Captioning)

Generates a text description (caption) of a photo using the **BLIP** image-captioning model from Hugging Face.

This is a project I made while learning about generative AI with Python.

## What it does

- Loads a photo (from Google Drive in Colab)
- Uses the pretrained model [`Salesforce/blip-image-captioning-base`](https://huggingface.co/Salesforce/blip-image-captioning-base) with `BlipProcessor` and `BlipForConditionalGeneration`
- Runs on GPU if available, otherwise CPU
- Prints the generated caption

## Example

Input: a photo of a boat at sea
Output: **"a boat traveling on the water near a small island"**

## Run it

The notebook is written for **Google Colab**:

1. Open `Image_to_Text.ipynb` in [Google Colab](https://colab.research.google.com/).
2. Upload a photo to your Google Drive and change `image_path` to point to it.
3. Run all cells.

To run it locally instead, remove the Google Drive cell, set `image_path` to a local file and install:

```
pip install transformers torch pillow
```
