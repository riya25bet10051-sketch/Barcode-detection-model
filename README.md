# Barcode-detection-model
Excited to share my newest project: an automated barcode verification system!  It uses deep learning (TensorFlow) to sort codes by how they look and checks the accuracy of the data in real time. 99% correct on fake datasets. #Python #DeepLearning #ComputerVision
# Deep Learning Barcode Verification System

# Overview  
This project is an automated Visual Verification System. It detects, classifies, and validates QR Codes and EAN-13 Barcodes.  

Unlike traditional laser scanners, this system uses a Convolutional Neural Network (CNN) to recognize code types visually. This makes it strong against noise, rotation, and blurring. It achieves over 98% accuracy using a custom-generated synthetic dataset. The system also has a decoding pipeline to ensure data is readable.  

## Key Features  
* *Synthetic Data Engine:* Automatically creates thousands of labeled QR/Barcode images for training.  
* *Deep Learning Classifier:* Custom CNN architecture (MobileNetV2 and Simple CNN variants) optimized for feature extraction.  
* *Dual-Stage Verification:*  
    1. *Visual Check:* AI confirms if the image is a valid code type.  
    2. *Data Check:* Decodes the content (URL/Product ID) to ensure integrity.  
* *High Precision:* The trained model achieves nearly perfect accuracy on validation sets.  

## Tech Stack  
* *Core:* Python 3  
* *Deep Learning:* TensorFlow, Keras  
* *Computer Vision:* OpenCV, Pillow  
* *Decoding:* Pyzbar  
* *Data Viz:* Matplotlib, Seaborn  

## Project Structure  
bash  
├── dataset_generator.py    # Script to create synthetic training data  
├── train_model.py          # CNN training script (with Transfer Learning)  
├── verify_system.py        # Main application: AI Classification + Decoding  
├── requirements.txt        # List of dependencies  
└── README.md               # Project documentation  
