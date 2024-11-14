# Traffic Object Detection with Gradio Interface
This repository contains a project for detecting traffic-related objects using a custom-trained model. The project includes a Gradio-based user interface, allowing users to upload images or video frames and view real-time object detection results.

## Overview
The goal of this project is to accurately detect traffic objects such as cars, buses, crosswalks, and traffic lights in images or video frames. The model is built with Detectron2, a high-performance object detection library. An interactive Gradio interface simplifies usage by providing an accessible way to test the model’s performance on new images or videos.

## Features
Model Training and Evaluation: Train and evaluate the model using Detectron2 with COCO metrics, including mean Average Precision (mAP).

Traffic Object Detection: Identify objects like vehicles,  buses, crosswalk, and traffic signs in real-time.

Gradio Interface: Easy-to-use web interface for uploading and analyzing images.


## Installation
Clone the repository and install the necessary dependencies.

Note: The project requires Python 3.8+ and Detectron2, which can be installed following the Detectron2 installation guide.

## Usage
Model Training: To train the model on a custom traffic dataset, refer to Traffic Object Detection-Main.ipynb. Configure the dataset and model settings, then run the training cells. Ensure you download the trained model and the config. file(faster_rcnn_X_101_32x8d_FPN_3x.yaml) from the detectron2 output directory.

Run the Gradio Interface: Launch the Gradio interface by running the Traffic Object Detection-Gradio Interface.ipynb notebook. Ensure you have the trained model file and config. file stored in your google drive.

## Model Evaluation
The model is evaluated using COCO metrics:

mAP: Assesses precision across different IoU thresholds.

AR: Measures recall for detecting various object sizes.

Details on the model evaluation are available in Traffic Object Detection-Main.ipynb.

## Results
Example results, including detection accuracy and sample output images, are shown in the notebooks.

## Contributing
Contributions are welcome! Feel free to open issues or submit pull requests to enhance the project.
