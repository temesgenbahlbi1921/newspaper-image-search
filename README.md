# newspaper-image-search
A Python computer vision and OCR project developed as part of the **Python 3 Programming Specialization on Coursera**.

The project processes a collection of newspaper images stored in a ZIP archive and allows users to search for a keyword within the images. When the keyword is found, the program uses OpenCV to detect faces on the corresponding newspaper page and generates a contact sheet containing the detected faces.

## Project Overview

This project combines several Python libraries and computer vision techniques:

- **Python** — core programming language
- **Pillow (PIL)** — image processing and contact-sheet generation
- **Pytesseract** — Optical Character Recognition (OCR)
- **OpenCV** — face detection
- **NumPy** — numerical and image-processing support
- **zipfile** — processing images stored inside ZIP archives

## How It Works

The application follows these main steps:

1. Open the ZIP archive containing newspaper images.
2. Extract and process each image.
3. Use Pytesseract to perform OCR on the newspaper image.
4. Search the extracted text for a specified keyword.
5. When the keyword is found, use OpenCV's Haar Cascade classifier to detect faces.
6. Crop the detected faces from the original image.
7. Generate a contact sheet containing the detected faces.
8. Display the results.

## Example Search

The project can search for keywords such as:

```python
search("Christopher", "readonly/small_img.zip")
```

The program reports the newspaper files containing the requested keyword and displays the detected faces when available.

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/newspaper-image-search.git
cd newspaper-image-search
```

Install the required Python packages:

```bash
pip install -r requirements.txt
```

Tesseract OCR must also be installed on the system for Pytesseract to work.

## Running the Project

The main implementation is available in:

```text
notebook/newspaper_image_search.ipynb
```

Open the notebook using Jupyter Notebook or JupyterLab:

```bash
jupyter notebook
```

Then run the notebook cells and provide the appropriate ZIP image dataset.

## Technologies Used

| Technology       | Purpose                         |
| ---------------- | ------------------------------- |
| Python 3         | Programming language            |
| Pillow           | Image manipulation              |
| Pytesseract      | Optical Character Recognition   |
| OpenCV           | Face detection                  |
| NumPy            | Numerical processing            |
| Jupyter Notebook | Development and experimentation |

## Learning Outcomes

Through this project, I practiced:

- Working with ZIP archives in Python
- Image processing with Pillow
- Optical Character Recognition
- Face detection with OpenCV
- Image cropping and composition
- Creating contact sheets
- Combining multiple Python libraries in a single application

## Course

**Python 3 Programming Specialization — Coursera**

This project was completed as a specialization project to apply Python programming, image processing, OCR, and computer vision concepts.

## Author

**Temesgen Bahlbi**
