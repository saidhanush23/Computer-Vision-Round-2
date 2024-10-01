# Computer-Vision-Round-2
# Brain MRI Segmentation using U-Net

This project implements a U-Net architecture for segmenting metastasis in brain MRI images. The model is trained to identify cancerous regions in brain scans, providing valuable assistance in medical imaging.

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Dataset](#dataset)
- [Usage](#usage)
- [Model Training](#model-training)
- [Results Visualization](#results-visualization)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The aim of this project is to develop an efficient and accurate method for segmenting metastasis in brain MRI images using deep learning techniques. The U-Net architecture is particularly well-suited for image segmentation tasks, making it ideal for this application.



## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/brain-mri-segmentation.git
   cd brain-mri-segmentation
   Brain_MRI_Dataset/
    └── Data/
        ├── Patient1/
        │   ├── image1.tif
        │   └── image1_mask.tif
        ├── Patient2/
        │   ├── image2.tif
        │   └── image2_mask.tif
        └── ...
Usage
Update the dataset path: Modify the data_dir variable in the main() function of train.py to point to your dataset path.

Run the training script:

bash
Copy code
python train.py
Check for saved models: The best model will be saved as unet_brain_mri_best.keras during training, and the final model will be saved as unet_brain_mri_final.keras.

Model Training
The model is trained using the following parameters:

Epochs: 50
Batch Size: 8
Optimizer: Adam
Loss Function: Binary Crossentropy
Metrics: Accuracy
Callbacks used during training include:

ModelCheckpoint: Saves the best model based on validation loss.
EarlyStopping: Stops training when the validation loss does not improve for 10 consecutive epochs.
Results Visualization
After training, the script visualizes some predictions along with the true masks to assess the model's performance visually. This will be displayed as a series of images showing the input images, true masks, and predicted masks.

Contributing
Contributions are welcome! If you would like to contribute, please fork the repository and create a pull request. Ensure that you follow the coding style used in the project.

Fork the repository
Create your feature branch (git checkout -b feature/YourFeature)
Commit your changes (git commit -m 'Add some feature')
Push to the branch (git push origin feature/YourFeature)
Open a pull request
