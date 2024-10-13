# GAN Image Processing Project

This project uses a Generative Adversarial Network (GAN) to perform image processing tasks, such as style transfer or image generation, on a set of input images. The workflow includes loading images from a source folder, applying a GAN model, and saving the processed images to an output folder.

## Project Overview

This repository contains a Jupyter Notebook (`gan3.ipynb`) that demonstrates how to apply a pre-trained GAN model on a collection of images. The notebook covers:
- Loading images from a specified directory.
- Preprocessing and normalizing images for input into the GAN.
- Applying the GAN model for image transformation.
- Saving the transformed images to an output directory.

## Getting Started

### Prerequisites

To run this project, you'll need the following libraries installed:
- Python 3.x
- TensorFlow
- Pillow (PIL)
- shutil (part of Python’s standard library)

### Data

Please download data from [here](https://www.kaggle.com/competitions/gan-getting-started/data) and modify SOURCE_DIR, and TARGET_DIR

You can install the required libraries using pip:
```zsh
pip install -r requirements.txt
```

### Directory Structure

Before running the notebook, make sure to unzip the gan-getting-started zip file from kaggle into kaggle/input/gan-getting-started

### How to Run

1. **Prepare Input Images**: Place the `.jpg` images you want to process inside the `kaggle/input/gan-getting-started/monet_jpg` directory.
   
2. **Execute the Notebook**:
   - Open `gan3.ipynb` in Jupyter Notebook or Jupyter Lab.
   - Follow the instructions within the notebook to load and preprocess images.
   - Run the cell that applies the GAN model to process each image in the input folder.
   - The processed images will be saved to the `output` directory.

3. **Generate Archive (Optional)**:
   - The notebook also includes a step to create a ZIP archive of all processed images, saved in the `output` directory. This step can be useful for easily downloading or sharing the results.

### Example Usage

To start processing images, run all cells in the notebook. You can adjust the parameters or specify additional settings (e.g., start processing after a certain image) within the notebook as needed.

## Notes

- **Input Image Format**: Ensure all input images are in `.jpg` format.
- **Image Size**: Depending on the GAN model, large images may require significant memory. You may need to resize images before processing if you encounter memory issues.
- **Model Customization**: If you wish to modify the GAN model, you can do so in the notebook. Be sure to adjust the relevant parameters or paths accordingly.

## Troubleshooting

If you encounter any errors, ensure that all directories exist as specified and that the necessary Python libraries are installed. For issues related to TensorFlow or the GAN model, consult the respective library documentation for further guidance.