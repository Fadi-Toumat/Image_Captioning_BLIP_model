# Image Captioning with BLIP Model

## Overview

This project provides a simple web application for Image Captioning using the BLIP (Bootstrapping Language-Image Pre-training) model from the Hugging Face Transformers library. The application allows you to upload an image, and then the model automatically generates a textual description for that image.

**This application has been primarily designed and tested on [Google Colab](https://colab.research.google.com/), and it is highly recommended to run it there to leverage its free resources (especially GPUs) and ease of setup.**

## Features

* Generates descriptive captions for images.
* Intuitive user interface built with Gradio.
* Supports running the model on GPUs for improved performance.

## How to Run (in Google Colab)

**For optimal performance, it is recommended to enable T4 GPU in Google Colab:**
* In the top menu bar, click on `Runtime` -> `Change runtime type`.
* Select `T4 GPU` as the `Hardware accelerator`.

**Steps to run the application:**

1.  **Open a new Google Colab notebook.**
2.  **In the first cell, install the required libraries:**
    ```bash
    !pip install gradio transformers torch numpy Pillow
    ```
3.  **In a separate cell, paste the code from the `app.py` file** (found in this repository).
4.  **Run this cell.** Gradio will generate a Public URL in the cell output (e.g., `https://xxxxxxxx.gradio.live`).
5.  **Click the link** to open the application in your web browser.

## Key Components

* **`app.py`**: The main Python file containing the Gradio application code.
* **`requirements.txt`**: A list of required Python libraries and dependencies.
* **BLIP Model**: `Salesforce/blip-image-captioning-base` used for caption generation.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
