#Logo Authenticity Detection
Logo Authenticity Detection is a Python script that utilizes image processing and deep learning techniques to determine the authenticity of a logo image.
It compares a test logo image with images scraped from the web to identify similarities and assess whether the test image is genuine or potentially altered.

Dependencies
requests
beautifulsoup4
tensorflow
numpy
matplotlib
scipy
easyocr

# Installation
You can install the required dependencies using pip:
pip install requests beautifulsoup4 tensorflow numpy matplotlib scipy easyocr

# Usage
Run the script logo_authenticity_detection.py.
Enter the brand logo name when prompted.
Enter the path to the test image when prompted.
The script will scrape and download images related to the brand logo from the web.
It will then analyze the test image, comparing it with the downloaded images to determine its authenticity.
The script will display the test image with a prediction indicating whether it is real or potentially altered.


# Functionality Overview
Downloading Images: Utilizes Google Image Search to download images related to the specified brand logo.
Feature Extraction: Extracts features from images using the VGG16 convolutional neural network.
Text Extraction: Uses EasyOCR to extract text from images, aiding in determining authenticity.
Image Similarity Calculation: Computes cosine similarity and Pearson correlation coefficient between feature vectors of images to assess similarity.
Prediction: Based on similarity scores, predicts whether the test image is genuine or fake.

