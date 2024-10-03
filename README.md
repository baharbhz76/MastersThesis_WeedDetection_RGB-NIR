# MastersThesis_WeedDetection_RGB-NIR
Enhancing Weed Detection and Segmentation with Advanced Deep Learning Methods Leveraging RGB-NIR Imaging
# Overview
This repository contains the Jupyter notebooks and code for my master's thesis project titled "Enhancing Weed Detection and Segmentation with Advanced Deep Learning Methods Leveraging RGB-NIR Imaging". The goal of this research is to enhance weed detection in agriculture using deep learning models that leverage both RGB and near-infrared (NIR) imaging data. This work contributes to the field of precision agriculture by automating weed management through more accurate and eco-friendly methods.

# Thesis Summary
The project addresses improving weed detection and segmentation by integrating NIR data with classical RGB channels. By optimizing CNN architectures, particularly U-Net for segmentation and YOLO models for detection, the thesis demonstrates how combining multispectral data enhances model performance, supporting precision agriculture.

# Notebooks
The repository includes the following notebooks that demonstrate different parts of the research:

** 1. G+NIR.ipynb
Description: This notebook focuses on the use of Green (G) and NIR spectral data to perform segmentation tasks. Various image processing techniques and a U-Net-based model are applied.
Key Methods: Image pre-processing, U-Net segmentation on G+NIR data.

** 2. G+NIR+NDVI.ipynb
Description: This notebook expands the previous one by adding the NDVI (Normalized Difference Vegetation Index) feature for segmentation. It explores how NDVI data can be used to enhance weed detection.
Key Methods: U-Net model with G+NIR+NDVI channels for improved weed segmentation.

# 3. RGB+NIR.ipynb
Description: This notebook explores the combination of traditional RGB imaging with NIR data, leveraging a modified U-Net model to accept the four input channels.
Key Methods: RGB+NIR image processing, U-Net with a custom convolutional layer for four-channel input.

# 4. Yolov5.ipynb
Description: This notebook implements the YOLOv5 model for object detection, focused on detecting weeds and crops using RGB data.
Key Methods: YOLOv5 for weed detection, training with different image resolutions and model sizes.

# 5. Yolov8.ipynb
Description: This notebook extends the object detection work using the YOLOv8 model, improving the detection accuracy and speed.
Key Methods: YOLOv8 model, real-time weed detection with RGB images.

# Dataset
ACRE Dataset: The primary dataset used for object detection tasks, split into training, validation, and testing sets. Images were pre-processed using Roboflow and augmented to enhance training.
Sunflower Dataset: Used for segmentation tasks, with images representing different growth stages. NDVI and NIR data were applied for better segmentation.
Installation
To run the notebooks, you will need Python 3.6 or higher and the following dependencies:

1. Clone the Repository
bash
Copy code
git clone https://github.com/yourusername/yourrepository.git
cd yourrepository
2. Install the Required Dependencies
bash
Copy code
pip install flask transformers datasets tensorflow yolov5 yolov8 scikit-image
pip install opencv-python
Running the Notebooks
To run the notebooks, use the following steps:

Launch Jupyter Notebook

bash
Copy code
jupyter notebook
Open the Desired Notebook:

Navigate to the cloned repository and open one of the provided .ipynb files (e.g., RGB+NIR.ipynb).
Run the cells to reproduce the results of the thesis.
Results
The key findings of the thesis are as follows:

RGB+NIR Models: By integrating NIR data with RGB, the U-Net model achieved superior segmentation accuracy, particularly for distinguishing weeds from crops.
YOLOv8 Object Detection: YOLOv8 outperformed YOLOv5 for real-time object detection tasks, providing higher precision in detecting weeds using RGB data alone.
NDVI Impact: Adding NDVI data marginally improved segmentation performance, particularly in more challenging scenarios where weeds and crops had similar visual characteristics.
Contributors
Candidate: Bahareh Behrouzi
Supervisors: Prof. Renato Ferrero, Dr. Nicola Dilillo
Institution: Politecnico di Torino
License
This project is licensed under the MIT License.
