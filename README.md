Bird Data Digitization Project 🐦
This repository contains the code and resources for a project that automates the extraction of ornithological data from scanned paper records. By combining Optical Character Recognition (OCR) with a Convolutional Neural Network (CNN), the system can digitize handwritten and printed bird survey data, a process that is traditionally time-consuming and prone to human error.

📜 Project Overview
The goal of this project is to create an efficient pipeline for digitizing historical bird survey sheets. These sheets often contain both standardized, typed fields (e.g., location, date) and handwritten observations (e.g., species counts, notes). The project addresses two main challenges:

Extracting structured data from the forms using OCR.

Handling variations in handwriting and form layout using a custom-trained CNN.

The output is a clean, structured dataset ready for analysis by ornithologists and researchers.

✨ Features
Image Preprocessing: Scripts to clean and enhance scanned images for better OCR accuracy.

Tesseract OCR Integration: Uses the Tesseract engine to recognize and extract text from defined regions of interest (ROIs) on the paper forms.