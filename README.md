# Megadetector

## Wild Animal Detection with Mega Detector

### Overview

This project aims to detect and classify wild animals in wild terrains using the Mega Detector, an advanced object detection and classification model. The model leverages transfer learning on a deep neural network and is implemented on an AWS EC2 instance with the Deep Learning AMI.

### Features

- **Mega Detector Model:** Utilizes a pre-trained model for object detection and classification of wild animals.
  
- **Data Pipeline Script:** Downloads data from a remote server, processes it using the Mega Detector model and stores the results on the EC2 instance.

- **Video Processing Script:** Provides functionality to process videos for wild animal detection, with the flexibility to adapt for image processing.

### Workflow

1. **EC2 Instance Setup:**
    - Use the Deep Learning AMI on an AWS EC2 instance.
  
2. **Data Retrieval and Storage:**
    - Employ the data pipeline script to download data from a remote server, storing it on the EC2 instance.
  
3. **Model Implementation:**
    - Utilize the Mega Detector model for object detection and classification.
    - Apply transfer learning on the large training dataset to fine-tune the model for wild animal detection.

4. **Data Processing:**
    - Implement the data pipeline script to process the downloaded data, feeding it through the Mega Detector model, and storing the results on the EC2 instance. For this project, we had our own data residing on the the server for MSDA program at Clarkson University.

5. **Video/Image Processing:**
    - Leverage the provided script for processing videos, with the option to modify it for image processing.

### Getting Started

1. **Prerequisites:**
    - AWS account with EC2 instance access.
    - Deep Learning AMI installed on the EC2 instance.

2. **Installation:**
    - Clone the repository to your local machine.
    - Run the setup.py script to install all the dependencies.

3. **Usage:**
    - This repository has two main folders: "PytorchWildlife" and "Demo".
    - The PytorchWildlife folder contains scripts for building the model and scripts for modified models for different datasets and tasks.
    - The models can be used for detection as well as classification.
    - The demo folder has a few scripts to demonstrate the working of the models for images and videos.
    - I have worked on the 'modified_video_detection.ipynb' notebook. This notebook has a script that downloads the data file on the local machine, feeds data to the model one by one and then saves these files to a separate folder.
    - The script can be modified and used for image data as well.
    - For fine-tuning the models and changing the models, the modifications need to be made in respective files for the respective model in the PytorchWildlife directory.
      

### Modification and Customization

- The project is highly customizable:
    - Adjust the Mega Detector model parameters.
    - Modify the data pipeline script for specific data processing requirements.
    - Adapt the video processing script for image processing if needed.

### Contribution

Contributions are welcome! Feel free to open issues, submit pull requests, or provide feedback.

### Reference

[https://github.com/microsoft/CameraTraps/blob/main/megadetector.md](https://github.com/microsoft/CameraTraps/blob/main/megadetector.md)
