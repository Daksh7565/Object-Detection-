
# README

## Project Overview

This repository contains the implementation for the AI Internship assessment task provided by LPU. The objective is to develop a robust computer vision system capable of detecting objects and their associated sub-objects in a hierarchical structure, meeting the requirements outlined in the assessment.

## Assessment Details

### Task Requirements:

1. **Object and Sub-Object Detection**:

   - The system must identify main objects, such as vehicles or people, and detect smaller, related components like tires, helmets, or doors.
   - It must establish a parent-child relationship between the detected main objects and their components, assigning unique identifiers to each item.
   - The system needs to function reliably with standard video streams and common object-sub-object associations.

2. **JSON Output**:

   - The detection results should be presented in a structured JSON format, clearly capturing the hierarchical relationships and details such as bounding boxes and unique IDs for both main objects and their components.

3. **Sub-Object Image Retrieval**:

   - The system should allow users to extract and save cropped images of specific sub-objects based on the detected hierarchy, such as retrieving a helmet image from a person or a door image from a car.

4. **Inference Speed Optimization**:

   - The solution should be optimized for real-time performance, capable of processing video at 10–30 frames per second (FPS) using only a CPU.

5. **Modularity and Extensibility**:

   - The system should be designed to easily accommodate new object-sub-object pairs without significant rework, ensuring future flexibility and scalability.

## System Features

- **Object Detection**: Detects objects and their associated sub-objects in a hierarchical manner.
- **JSON Output**: Provides detection results in a structured JSON format.
- **Sub-Object Image Retrieval**: Allows users to retrieve and save specific sub-object images.
- **Optimized Performance**: Real-time processing at 10–30 FPS on CPU.
- **Modular Design**: Easily extensible for additional object-detection scenarios.

## Requirements

1. **Python**: Ensure Python 3.x is installed.
2. **Dependencies**: Install required packages using:
   ```bash
   pip install -r requirements.txt
   ```
3. **Frameworks and Libraries**:
   - OpenCV
   - YOLO (PyTorch-based)

## How to Run

1. Clone this repository:
   ```bash
   git clone [repository_url]
   ```
2. Navigate to the directory:
   ```bash
   cd [repository_folder]
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the main script:
   ```bash
   python Implementation.ipynb
   ```
5. View JSON outputs and cropped sub-object images in the output folder.

## Benchmarking and Results

Visual Results
![download](https://github.com/user-attachments/assets/c1e41b36-d82c-43ca-bb60-f0b32370a561)
![download (2)](https://github.com/user-attachments/assets/316270fc-d439-4a80-bd9f-ff08f511c316)
The system successfully detected multiple objects (e.g., persons, cars) and associated sub-objects (e.g., components) in a forest scene, as shown in the image above. Bounding boxes and labels clearly indicate the confidence scores and hierarchical associations.
- **Inference Speed**: Achieved [7-14] FPS .
- **Sample JSON Outputs**: Included in the `outputs/` folder.
Cropped Sub-Objects**: Saved in the `subobjects/` folder.

## Deliverables

1. Complete source code with detailed comments.
2. JSON outputs for test cases.
3. Benchmarking report documenting inference speeds and optimization strategies.

## Notes

- Ensure that the system handles edge cases like occlusion and overlapping objects.
- Focus on clean, modular, and well-documented code.

## License

Specify the license under which your project is distributed (e.g., MIT License).

## Authors

Provide the names or contact details of the contributors.

---

Feel free to update this README as needed to reflect changes in the project or additional instructions.
