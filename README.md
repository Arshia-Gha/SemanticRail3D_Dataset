# 📌 SemanticRail3D_Dataset
This repository contains the SemanticRail3D dataset, a high-quality 3D point cloud dataset for railway infrastructure segmentation and classification. It consists of 438 point clouds, each covering 200 meters of track, totaling 2.8 billion points labeled into 11 semantic classes. The dataset is structured for machine learning applications, with train, validation, and test splits.

# 🔹 Key Features:
✔ High-resolution LiDAR data (980 points/m², 5mm precision)

✔ Semantic segmentation (11 classes) & instance segmentation

✔ Preprocessed with normal vectors, intensity, and additional features

✔ Structured in NumPy format for easy loading

🚀 Use this dataset for developing AI models in railway point cloud analysis! 🚀



## Introduction

The segmentation and classification of 3D point clouds in railway infrastructures present significant challenges in both scientific research and technological applications. One major difficulty is the limited availability of large, high-quality datasets that enable the training of AI models for point cloud segmentation and classification. Furthermore, the field lacks benchmarks that allow for objective comparison of different approaches, making it difficult to track progress and develop improved solutions.

The SemanticRail3D dataset aims to bridge this gap by offering a comprehensive benchmark for the scientific community. This dataset provides detailed 3D point cloud labels of railway environments, facilitating the development and evaluation of segmentation and classification models. With this dataset, researchers now have a common reference for comparing results, improving methodologies, and advancing state-of-the-art machine learning techniques for railway infrastructure analysis.

## Dataset Overview
The SemanticRail3D dataset consists of 438 point clouds, each covering approximately 200 meters of railway track. The dataset contains a total of 2.8 billion points, with 11 different classes labeled for semantic segmentation. Additionally, track position for each railway line is provided, along with instance segmentation to distinguish between different objects in the scene.

 ## Data Acquisition
The dataset was collected using a LYNX Mobile Mapper by Optech, which employs two LiDAR sensors mounted on a Mobile Mapping System (MMS). The average point cloud density is 980 points/m², with a range precision of 5 mm, ensuring high-quality spatial representation.

## Data Attributes
Each point cloud includes the following attributes:

XYZ Coordinates: Provided in a local coordinate system, ensuring positive values (minimum coordinate value is 0).

Intensity: Encoded in 12-bit format (0-4096), indicating surface reflectivity.

Time Stamp: Time at which each point was captured.

Return Number: Identifies whether the point corresponds to the first, second, third, etc., return of a LiDAR pulse.

Number of Returns: Specifies the total number of returns detected from a single laser pulse.

Scan Angle: The inclination angle of the LiDAR sensor when capturing the point.

## 📂 Dataset Splits

- 📝 **[Train Cloud Segments](Data_Info/train_clouds.txt)** → Clouds and their respective segment numbers.
  
- 📝 **[Validation Cloud Segments](Data_Info/val_clouds.txt)** → Clouds and their respective segment numbers.
  
- 📝 **[Test Cloud Segments](Data_Info/test_clouds.txt)** → Clouds and their respective segment numbers.
  
- 🗑 **[Removed Cloud Segments](Data_Info/removed_clouds.txt)** → List of removed clouds with missing segments.
  
📊 Dataset Distribution
The dataset consists of 437 point clouds, each divided into 5 segments, totaling 2,185 segments.
Some segments were removed due to issues such as mislabeling, errors in labels, or incorrect class assignments.
The remaining data was split into Train, Validation, and Test sets to be used for machine learning approaches.

📌 Static Chart
Below is the dataset distribution after preprocessing and splitting:

![Dataset Distribution](Data_Info/dataset_distribution.png)

📈 Interactive Chart
For a detailed interactive version, click the link below:

📈 **[View Interactive Chart](Data_Info/dataset_distribution.svg)**

📊 View Interactive Chart
