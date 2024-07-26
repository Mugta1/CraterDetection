

# Lunar Crater Detection with Detection Transformers (DETR)

## Overview

This project focuses on the automatic detection of lunar craters and boulders from Orbiter High Resolution Camera (OHRC) images using advanced AI and ML techniques. Leveraging Detection Transformers (DETR), the solution aims to enhance accuracy and robustness in identifying and classifying geological features on the lunar surface. This tool is intended to support scientific research, mission planning, and lunar exploration by providing detailed and precise information about the lunar terrain.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Model Training](#model-training)
6. [Data Preparation](#data-preparation)
7. [Results](#results)
8. [Future Work](#future-work)
9. [Contributing](#contributing)
10. [License](#license)
11. [Acknowledgements](#acknowledgements)

## Introduction

Detecting craters and boulders on the lunar surface is crucial for various scientific and exploratory missions. This project employs cutting-edge machine learning and deep learning techniques, specifically Detection Transformers (DETR), to automate the detection process. By providing a robust and accurate solution for analyzing lunar imagery, this tool assists researchers and mission planners in understanding the lunar landscape, identifying potential landing sites, and conducting geological studies.

## Features

- **Automated Detection**: Automatically detects craters and boulders in OHRC images with high precision.
- **High Accuracy**: Utilizes DETR, a state-of-the-art object detection model, for improved detection accuracy.
- **Scalable**: Capable of processing large datasets of lunar imagery efficiently.
- **User-Friendly**: Provides an easy-to-use interface for uploading and analyzing images.
- **Customizable**: Allows users to fine-tune the model for specific detection tasks and datasets.
- **Visualization**: Generates visual representations of detected features on the lunar surface.

## Installation

### Prerequisites

- Python 3.7+
- Git
- CUDA (for GPU acceleration, optional but recommended)

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/username/lunar-crater-detection.git
   cd lunar-crater-detection
   ```

2. **Install Dependencies**
   Ensure you have Python 3.7+ installed. Then, install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up Environment**
   Create a `.env` file in the root directory and add necessary environment variables:
   ```
   DATASET_PATH=/path/to/dataset
   MODEL_PATH=/path/to/pretrained/model
   ```

## Usage

### Running the Detection

1. **Prepare Data**
   Ensure your OHRC images are in the specified dataset directory.

2. **Run the Detection Script**
   ```bash
   python detect_craters.py --input /path/to/image.jpg --output /path/to/output.jpg
   ```

3. **View Results**
   The output image with detected craters and boulders will be saved in the specified output directory. You can visualize the detection results using any image viewer.

### Customizing Detection Parameters

You can customize various detection parameters in the `config.yaml` file, such as threshold values, model configurations, and output settings.

## Model Training

### Preparing the Training Environment

1. **Prepare Training Data**
   Organize your dataset into `images` and `annotations` directories. Ensure that the annotations are in the correct format for DETR training.

2. **Train the Model**
   ```bash
   python train.py --config config.yaml
   ```
   Customize the `config.yaml` file to set your training parameters, including learning rate, batch size, and number of epochs.

3. **Evaluate the Model**
   ```bash
   python evaluate.py --model /path/to/trained/model
   ```
   The evaluation script will generate metrics and visualizations to assess the model's performance.

## Data Preparation

Accurate data preparation is crucial for training effective machine learning models. Ensure that your OHRC images are correctly labeled and annotated. Use tools like Labelbox or CVAT for annotation. The annotations should include bounding boxes or segmentation masks for craters and boulders.

## Results

### Sample Results

Include sample results showcasing the detection capabilities of the model. Provide images with detected craters and boulders highlighted, along with metrics such as precision, recall, and F1-score.

### Performance Metrics

- **Precision**: Measure of the accuracy of the detected craters and boulders.
- **Recall**: Measure of the completeness of the detection.
- **F1-Score**: Harmonic mean of precision and recall.

## Future Work

- **Enhancing Model Accuracy**: Explore advanced techniques to further improve detection accuracy.
- **Real-Time Detection**: Optimize the model for real-time detection on edge devices.
- **Integration with Lunar Missions**: Collaborate with space agencies to integrate this tool into lunar missions.
- **Expanding Dataset**: Collect and annotate more OHRC images to improve model robustness.

## Contributing

Contributions are welcome! Follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

This project was developed as part of the ISRO Bharatiya Antariksh Hackathon 2024 by the CyCrawlers team from Delhi Technological University (DTU). Special thanks to all team members, mentors, and organizers for their support and guidance.

---

