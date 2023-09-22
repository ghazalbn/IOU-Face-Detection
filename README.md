# IOU-Face-Detection

![GitHub](https://img.shields.io/github/license/ghazalbn/iou-face-detection)

This repository contains Python code for two main tasks:

1. **IOU-based Object Detection**: In the `IOU_object_detection.py` file, I demonstrate how to perform object detection using the Intersection over Union (IOU) method. The input image is labeled with bounding boxes using the LabelImg labeling tool. The code calculates IOU scores for candidate windows and labels them as "Face," "Background," or "None" based on predefined IOU thresholds.

2. **Geometric Image Augmentation**: In the `geometric_augmentation.py` file, I showcase various geometric image augmentations using the [imgaug](https://github.com/aleju/imgaug) library. The input image have bounding box annotations obtained from the LabelImg labeling tool. We apply a range of geometric transformations to the image and visualize the augmented results.

## Getting Started

### Prerequisites

Before running the code, ensure you have the following prerequisites installed:

- Python (3.6 or higher)
- OpenCV (`opencv-python`)
- NumPy (`numpy`)
- Matplotlib (`matplotlib`)
- XML ElementTree (`xml.etree.ElementTree`)
- imgaug (`imgaug`)

## Files

- `Melli.jpg`: Input image for both object detection and augmentation.
- `Melli.xml`: XML file containing bounding box information for objects in the image. Generated using the LabelImg labeling tool.

## IOU-based Object Detection

### Code

The `IOU_object_detection.py` file performs IOU-based object detection on the input image. It follows these steps:

1. Loads the input image and converts it to RGB format.
2. Reads the XML file to extract ground truth bounding box annotations.
3. Applies sliding windows of varying sizes and positions.
4. Calculates IOU scores for candidate windows and assigns labels ("Face," "Background," or "None") based on predefined thresholds.
5. Visualizes the input image with labeled bounding boxes.
6. Randomly displays detected faces and backgrounds.

## Geometric Image Augmentation

### Code

The `geometric_augmentation.py` file showcases various geometric image augmentations using the imgaug library. It performs the following steps:

1. Loads the input image and converts it to RGB format.
2. Reads the XML file to obtain bounding box annotations.
3. Defines a function for applying geometric augmentations and visualizing the results.
4. Applies a series of geometric augmentations, including scaling, translation, rotation, shear, and more.
5. Displays the augmented images with bounding boxes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- The code in this project serves as a basic starting point for object detection using IOU and geometric image augmentation tasks. Feel free to customize and extend this project for your specific needs!

