# Drone Detection Project - SkyGuard Y5
<img src="https://github.com/muqeet-here/SkyGuard-Y5/blob/main/images/Image.png" alt="Drone">

## Overview

This project focuses on detecting drones in images using the YOLOv5 object detection model. We utilize Roboflow for efficient dataset management and YOLOv5 for custom training. The implementation is done using PyCharm as the integrated development environment (IDE) and PyTorch for deep learning.

## Prerequisites

Make sure you have the following software installed:

- [PyCharm](https://www.jetbrains.com/pycharm/download/)
- [Python 3.x](https://www.python.org/downloads/)
- [PyTorch](https://pytorch.org/get-started/locally/)

## Setup

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/dronedetection.git
    cd dronedetection
    ```

2. **Create a virtual environment (recommended):**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

## Dataset Preparation with Roboflow

1. Collect and annotate drone images.
2. Upload the dataset to Roboflow.
3. Generate YOLOv5-compatible annotations using Roboflow.

## YOLOv5 Custom Training

1. Open the YOLOv5 custom training notebook in PyCharm.

2. Configure the training parameters, such as dataset paths, batch size, and model hyperparameters.

3. Execute the notebook to start training.

## PyCharm Project Structure

- `data/`: Directory for storing dataset and model-related files.
- `notebooks/`: Contains the YOLOv5 custom training notebook.
- `src/`: Source code for the project.
- `utils/`: Utility functions and scripts.

## Usage

1. Ensure the virtual environment is activated:

    ```bash
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

2. Run the YOLOv5 custom training notebook.

3. Monitor training progress and evaluate the model.

## Results

Evaluate the trained model on test data to assess its performance. Adjust hyperparameters or augmentations as needed for better results.

## Acknowledgments

- [Roboflow](https://roboflow.com/) for dataset management and annotation.
- [YOLOv5](https://github.com/ultralytics/yolov5) for the object detection model.
- [PyCharm](https://www.jetbrains.com/pycharm/) for the IDE.
- [PyTorch](https://pytorch.org/) for deep learning.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

Feel free to customize this README to suit your project and provide more specific details about your implementation.
