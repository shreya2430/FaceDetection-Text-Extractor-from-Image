# Image Processing Engine with OCR and Detection Capabilities

## Overview
This project implements a Python-based image processing engine with functionalities for image detection, enhancement, modification, and text analysis. The engine supports various image formats and includes face and eye detection features using the OpenCV Cascade Classifier. Additionally, OCR (Optical Character Recognition) is integrated using PyTesseract for text extraction, and an algorithm for keyword-based image summarization is provided.

## Key Features
- **Image Pre-processing**: Filters and enhancements for image modification.
- **Face and Eye Detection**: Detects faces and eyes in images using OpenCV's Haar Cascade Classifiers.
- **Text Extraction**: Extracts text from images using PyTesseract.
- **Keyword-based Summarization**: Summarizes extracted text with 85% accuracy.
- **User Interaction**: Allows users to apply chosen filters and view modified images.

## Dependencies
- `Pillow`
- `pytesseract`
- `cv2` (OpenCV)
- `numpy`
- `re`
- `os`

## Installation
1. Ensure Python 3.x is installed on your system.
2. Install required libraries:
   ```bash
   pip install pillow opencv-python pytesseract numpy
   ```
3.	Download and install Tesseract-OCR.

## File Structure

-	**Main Script: The Python code includes sections for importing modules, processing images, applying filters, detecting faces/eyes, and performing OCR operations.**
- **Image Resources: Sample images should be placed in a designated folder (e.g., images/).**

## Usage

## 1. Applying Filters

Run the filter application function and choose a filter by entering the corresponding number:
```python
n = int(input("Enter filter choice (1 to 11): "))
Filteringfn(n)
```

## 2. Text Extraction from Images

To extract text from an image, use:
```python
print(image_text("image_path.png"))
```

## 3. Face and Eye Detection

Face detection can be executed as follows:
```python
face_detection("image_path.jpg")
```
For eye detection:
```python
eye_detection("image_path.jpg")
```
## 4. OCR and Keyword Search

To search for a keyword in images and display detected faces:
```python
search("keyword", "path_to_images/")
```

## Results
- **Text Analysis Accuracy: Achieved 85% accuracy on summarization tests with a dataset of over 1,000 instances.**
- **Face/Eye Detection: Robust detection using Haar cascades on varied image datasets.**
