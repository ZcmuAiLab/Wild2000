# Wild2000: Wild Virtual try-on Dataset

[![GitHub license](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Dataset Size](https://img.shields.io/badge/dataset_size-2000_samples-blue)](dataset)
[![Open Source](https://img.shields.io/badge/open_source-yes-brightgreen)](LICENSE)

## Introduction

The Wild2000 dataset is introduced in the paper "Mamba-Vton: Mamba SLLA Cross-Attention Fusion for Robust Virtual Try-On in Complex Wild Scenes" to provide high-quality data support for virtual try-on tasks in complex wild scenes. Focusing on virtual dressing in wild scenarios, this dataset covers a variety of clothing styles, human poses, and background environments, effectively promoting the application and development of virtual try-on technologies in real-world complex scenes.

## Dataset Features

- **Sample Size**: Contains 2000 carefully annotated pairs of model images and corresponding cloth images.
- **Diverse Clothing Styles**: Includes a wide range of clothing categories, such as tops, bottoms, dresses, and accessories, to meet different research needs.
- **Real-World Scenarios**: All samples are captured in real wild scenes with complex backgrounds and natural lighting conditions, closely resembling actual application environments.
- **High-Resolution Images**: Both model and cloth images are presented in high resolution to ensure clear details, facilitating in-depth analysis and research.
- **Paired Images**: Model images are paired one-to-one with corresponding cloth images, making it convenient for researchers to develop and test virtual dressing algorithms.


## Summary of Existing Test Datasets for Wild Scenes

| Dataset Name   | Reference | Number of Pairs | Open Source |
|----------------|-----------|-----------------|-------------|
| StreetVTON     | Cui et al. (2023)       | 2089            | ✓           |
| WildVTON       | Choi et al. (2024)      | 200            | x          |
| Wild2000       | Ours      | 2000        | ✓              |

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


## Data Visualization

### Wild2000_distribution


### Wild200 dataset



## Getting Started

### Downloading the Dataset
You can download the dataset from the [Wild2000 Release Page]( google link!!!)


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

For any questions or inquiries about the Wild2000 dataset, please contact us at [your.email@example.com](jinwei@zcmu.edu.cn).

Thank you for your interest in the Wild2000 dataset! We hope it helps advance your research and development in the exciting field of virtual dressing and fashion AI.



## References

- **Cui et al. (2023)**: Aiyu Cui, Jash Mahajan, Viraj Shah, Pranav Gomathinayagam, and Svetlana Lazebnik. Street TryOn: Learning In-the-Wild Virtual Try-On from Unpaired Person Images. CoRR abs/2311.16094 (2023). [https://doi.org/10.48550/arXiv.2311.16094](https://doi.org/10.48550/arXiv.2311.16094)
- **Choi et al. (2024)**: Improving Diffusion Models for Authentic Virtual Try-On in the Wild. _Computer Vision - ECCV 2024 - 18th European Conference, Milan, Italy, September 29-October 4, 2024, Proceedings, Part LXXXVI_, pages 206–235. Springer, 2024.

