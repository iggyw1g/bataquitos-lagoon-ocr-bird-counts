# Bird Data Digitization Project 🐦

This repository contains the code and resources for a project that automates the extraction of ornithological data from scanned paper records. By combining **Optical Character Recognition (OCR)** with a **Convolutional Neural Network (CNN)**, the system can digitize handwritten and printed bird survey data, a process that is traditionally time-consuming and prone to human error.

## 📜 Project Overview

The goal of this project is to create an efficient pipeline for digitizing historical bird survey sheets. These sheets often contain both standardized, typed fields (e.g., location, date) and handwritten observations (e.g., species counts, notes). The project addresses two main challenges:

1.  **Extracting structured data** from the forms using OCR.
2.  **Handling variations** in handwriting and form layout using a custom-trained CNN.

The output is a clean, structured dataset ready for analysis by ornithologists and researchers.

---

## ✨ Features

* **Image Preprocessing**: Scripts to clean and enhance scanned images for better OCR accuracy.
* **Tesseract OCR Integration**: Uses the Tesseract engine to recognize and extract text from defined regions of interest (ROIs) on the paper forms.
* **Custom CNN for Handwriting**: A trained CNN model specifically designed to interpret difficult-to-read handwritten fields, improving on Tesseract's general-purpose capabilities.
<!-- * **Data Validation**: A post-processing step to validate and clean the extracted data, checking for inconsistencies and formatting errors.
* **Automated Pipeline**: A complete workflow that takes a raw scan as input and outputs a structured CSV or JSON file.

---

## 🛠️ Technologies & Dependencies

* **Python**: The core programming language for the project.
* **Tesseract OCR**: An open-source OCR engine.
* **OpenCV**: Used for image preprocessing, including noise reduction, deskewing, and region-of-interest (ROI) detection.
* **TensorFlow / Keras**: The framework used to build and train the CNN model.
* **NumPy**: For numerical operations on data.
* **pandas**: For handling and manipulating the output data.

---

## 🚀 Getting Started

### Prerequisites

* Python 3.8 or higher.
* A C++ compiler (e.g., Visual C++ Build Tools on Windows, `build-essential` on Linux).
* Tesseract-OCR installed on your system.
    * **Windows**: [Tesseract Installer](https://github.com/UB-Mannheim/tesseract/wiki).
    * **Linux**: `sudo apt-get install tesseract-ocr`.
    * **macOS**: `brew install tesseract`.

### Installation

1.  Clone the repository:
    ```bash
    git clone [https://github.com/your-username/bird-data-digitizer.git](https://github.com/your-username/bird-data-digitizer.git)
    cd bird-data-digitizer
    ```
2.  Create and activate a virtual environment:
    ```bash
    python -m venv venv
    # On Windows
    .\venv\Scripts\activate
    # On macOS/Linux
    source venv/bin/activate
    ```
3.  Install the required Python packages:
    ```bash
    pip install -r requirements.txt
    ```

### Usage

To run the full data extraction pipeline on a single image:

```bash
python run_pipeline.py --image_path "path/to/your/scanned_bird_sheet.png" -->