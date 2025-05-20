# Forecasting Infrastructure Needs and Environmental Effects Using Satellite Imagery

This project focuses on analyzing urban growth in Phoenix, Arizona from 1984 to 2024 using satellite imagery and deep learning. The idea is to identify key urban features like buildings, roads, vegetation, and construction zones, and use those to understand how the city has grown over time. Based on this, we try to forecast future infrastructure needs and assess potential environmental impacts.


Author: Hetavi Mehta

---

## About the Project

We worked with quarterly satellite images (.tif format) spanning 40 years—about 1,476 images in total. All images are from the Phoenix region and were extracted using Google Earth Engine. The main goal was to build a deep learning pipeline that could process these images and generate meaningful insights for urban planning.

### Key Tasks:
- Extracted and organized temporal satellite imagery using GEE.
- Preprocessed the images (resize, augment, tile) to make them model-ready.
- Used YOLOv8 for object detection and DeepGlobe U-Net for semantic segmentation.
- Labeled each image with counts of detected features and assigned them to one of four zone types:
  - Urban Growth Zone
  - Stable Zone
  - Construction Zone
  - Green Recovery Zone
- Created a final labeled dataset in CSV format for further analysis and visualization.

---

## Tools and Libraries Used

- Google Earth Engine
- PyTorch & TensorFlow
- YOLOv8 (Ultralytics)
- DeepGlobe U-Net
- OpenCV, NumPy, Matplotlib
- Google Colab (for training on GPU)
