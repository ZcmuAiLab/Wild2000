# Wild2000: Dataset

[![GitHub license](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Dataset Size](https://img.shields.io/badge/dataset_size-2000_samples-blue)](dataset)
[![Open Source](https://img.shields.io/badge/open_source-yes-brightgreen)](LICENSE)

## Introduction

Welcome to the **Wild2000** dataset repository! This dataset is designed to support research and development in the field of virtual try-on and fashion AI. It contains 2000 high-quality samples of virtual try-on scenarios, capturing diverse clothing styles, body shapes, and poses. Whether you're working on virtual try-on systems, fashion recommendation algorithms, or computer vision tasks related to clothing, this dataset is a valuable resource for you.

## Dataset Overview

### Key Features
- **Sample Size**: 2000 pairs samples, include models and cloth in the wild.
- **Diverse Clothing Styles**: Includes a wide range of clothing categories such as tops, lowers, dresses, and accessories.
- **Realistic Body Shapes and Poses**: Features various body shapes and natural poses to simulate real-world dressing scenarios.
- **High-Resolution Images**: All samples are captured in high resolution to ensure detailed analysis.
- **Annotations**: Each sample is annotated with detailed information, including clothing labels, body keypoints, and pose data.

### Sample Structure
Each sample in the dataset is organized as follows:

Wild2000/
├── model_images/
│   ├── model_0001.jpg
│   ├── model_0002.jpg
│   └── ...
├── cloth_images/
│   ├── cloth_0001.jpg
│   ├── cloth_0002.jpg
│   └── ...
└── README.md

- **images/**: Contains high-resolution images of virtual try-on scenarios.
- **annotations/**: Contains JSON files with detailed annotations for each image.
  

## Data Visualization

### Clothing Distribution
The dataset includes a wide variety of clothing items, with a focus on different categories such as tops, bottoms, dresses, and accessories. The distribution of clothing categories is shown in the following visualization:

![Clothing Distribution](visualizations/clothing_distribution.png)

### Body Shape Distribution
The dataset captures diverse body shapes to ensure that the virtual dressing scenarios are representative of real-world variations. The distribution of body shapes is shown below:

![Body Shape Distribution](visualizations/body_shape_distribution.png)

### Pose Distribution
To simulate natural dressing scenarios, the dataset includes a variety of poses. The distribution of poses is shown in the following visualization:

![Pose Distribution](visualizations/pose_distribution.png)

## Getting Started

### Downloading the Dataset
You can download the dataset from the [Wild2000 Release Page](https://github.com/yourusername/Wild2000/releases). The dataset is available in a compressed `.zip` format for easy download.

### Usage
To use the dataset in your project, follow these steps:
1. **Extract the Dataset**: Unzip the downloaded file to a local directory.
2. **Load the Data**: Use your preferred programming language to load the images and annotations. For example, in Python, you can use the following code snippet:
     ```python
    import cv2
    import os

    dataset_path = "path/to/Wild2000"
    model_folder = os.path.join(dataset_path, "model_images")
    cloth_folder = os.path.join(dataset_path, "cloth_images")

    # Load an example model image and its corresponding cloth image
    model_path = os.path.join(model_folder, "model_0001.jpg")
    cloth_path = os.path.join(cloth_folder, "cloth_0001.jpg")

    model_image = cv2.imread(model_path)
    cloth_image = cv2.imread(cloth_path)

    cv2.imshow("Model Image", model_image)
    cv2.imshow("Cloth Image", cloth_image)
    cv2.waitKey(0)
    cv2.destroyAllWindows()

## Contributing

We welcome contributions to improve the Wild2000 dataset! If you find any issues or have suggestions for enhancements, please feel free to open an issue or submit a pull request.

### How to Contribute
1. **Report Issues**: If you encounter any problems with the dataset, please open an issue to let us know.
2. **Enhance Data**: If you have additional data or improvements to the existing data, please submit a pull request.
3. **Share Use Cases**: If you have used the dataset in your research or projects, we would love to hear about it! Share your work with us by opening an issue or sending us an email.

## License

The Wild2000 dataset is released under the [MIT License](LICENSE). You are free to use, modify, and distribute the dataset for both academic and commercial purposes, as long as you comply with the terms of the license.

## Contact

For any questions or inquiries about the Wild2000 dataset, please contact us at [your.email@example.com](mailto:your.email@example.com).

Thank you for your interest in the Wild2000 dataset! We hope it helps advance your research and development in the exciting field of virtual dressing and fashion AI.
