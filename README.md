# final_project_backend
Backend for LesionCheckr, Group 7's final project for AI in Enterprise Systems

LesionCheckr Backend
Description
LesionCheckr is a backend service designed to support a mobile application for classifying skin lesions. It uses a trained machine learning model to analyze images of skin lesions and return their classification based on the most likely lesion type.
 
Features

Image Classification: Classify skin lesions from images using a pre-trained deep learning model.

REST API: Provides a simple REST API for receiving images and sending back classification results.

Cross-Origin Resource Sharing (CORS): Configured to accept requests from various frontends.

Technologies Used
- Flask
- Python 3
- Keras
- OpenCV
- NumPy
- Pillow
 
Troubleshooting

Ensure all Python dependencies are correctly installed.

Verify that the model and label encoder files are correctly placed and accessible by the application.
Check that the base64 encoded image is formatted correctly and compatible with the expected input format of the model.
License

This project is licensed under the MIT License - see the LICENSE.md file for details.
 
Authors
Andrew Mark Dale - 100491442
Ali Istanbullu - 100905755
Chinedu Omenkukwu - 100805353
Andre Dallaire – 100337151
