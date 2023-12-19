# Drone Detection Project - SkyGuard Y5
<img src="https://github.com/muqeet-here/SkyGuard-Y5/blob/main/images/Image.png" alt="Drone">
## Overview

SkyGuard Y5 is a drone detection system based on the YOLOv5 object detection model. It is trained using annotated data from Roboflow, a platform for managing and annotating computer vision datasets.

## Roboflow Dataset

The annotated dataset for this project is available on Roboflow. You can access it [here](https://app.roboflow.com/nano-industries-sjw3s/quadcopter-mzzrt/1).

## Custom Training with YOLOv5

To perform custom training with YOLOv5, you can use the following Colab notebook:

[YOLOv5 Custom Training Tutorial](https://colab.research.google.com/github/roboflow-ai/yolov5-custom-training-tutorial/blob/main/yolov5-custom-training.ipynb)

## Requirements

- Python 3.x
- PyTorch
- YOLOv5
- Roboflow account for annotation

## Getting Started

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/drone-detection-yolov5.git
    cd drone-detection-yolov5
    ```

2. **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

3. **Download the YOLOv5 weights:**

    ```bash
    ./download_weights.sh
    ```

4. **Obtain annotated data from Roboflow:**

   - Log in to your Roboflow account.
   - Upload and annotate drone images using the Roboflow platform.
   - Export the dataset in YOLOv5 format.

5. **Organize the dataset:**

    ```bash
    unzip path/to/roboflow_export.zip -d data/
    ```

6. **Train the model:**

    ```bash
    python train.py --data data.yaml --cfg yolov5s.yaml --weights yolov5s.pt --batch-size 16
    ```

7. **Evaluate the model:**

    ```bash
    python val.py --data data.yaml --weights runs/train/exp/weights/best.pt
    ```

## Customization

- Adjust YOLOv5 configuration in `yolov5s.yaml`.
- Fine-tune training parameters in `train.py`.

## Results

After training, you can find the model weights in the `runs/train/exp/weights/` directory.

## Acknowledgments

- YOLOv5: [GitHub Repo](https://github.com/ultralytics/yolov5)
- Roboflow: [Official Website](https://roboflow.com/)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
