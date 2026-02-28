![Image Dataset Cleaner](images/img.png)

# Image Dataset Cleaner & Corruption Detector

A lightweight and fast Python utility designed to clean image datasets for Machine Learning and AI projects. This script recursively scans a given directory, filters out unsupported file types, and detects/deletes corrupted images to ensure your dataset is ready for training.

## Features

* **Recursive Scanning:** Automatically walks through all folders and subfolders in your target directory.
* **Format Filtering:** Instantly identifies and removes non-image files (e.g., SVG, GIF, etc.) while keeping supported formats (`.jpg`, `.jpeg`, `.png`, `.bmp`, `.webp`).
* **Corruption Detection:** Uses the `Pillow` library to verify image integrity and safely discard broken or unreadable files.
* **Progress Tracking:** Includes a sleek terminal progress bar powered by `tqdm` to monitor the cleaning process in real time.

## ⚠️ Important Warning
**This script permanently deletes files.** It does not move them to a recycle bin. Please make sure you have a **full backup** of your dataset before running this script!

## Prerequisites

Before running the script, ensure you have Python installed on your system. You will also need to install the required external libraries.

Install the dependencies using `pip`:

## Prerequisites

Before running the script, ensure you have Python installed on your system. You will also need to install the required external libraries.

Install the dependencies using `pip`:

```bash
pip install Pillow tqdm
```
Usage
Clone or download this repository to your local machine.

Open the corruption_ditection.py file in your preferred code editor.

Locate the dataset_path variable on line 5 and update it with the absolute path to your dataset folder:

```bash
dataset_path = r"C:\Path\To\Your\Dataset" # Enter your directory path here
```

Run the script from your terminal:
```bash
python corruption_ditection.py
```

