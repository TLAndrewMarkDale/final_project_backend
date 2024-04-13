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

Installation
Ensure you have Python 3 installed on your system. You can then follow these steps to get the backend up and running:
 
Clone the repository:
 
bash
Copy code
git clone [repository-url]
cd [repository-folder]
Set up a virtual environment (optional but recommended):
 
bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install dependencies:
 
bash
Copy code
pip install flask flask-cors numpy opencv-python-headless pillow keras
Start the server:
 
bash
Copy code
python app.py
API Usage
Endpoint: /classify
Method: POST
Body:
json
Copy code
{
  "image": "base64_encoded_image"
}
Success Response:
json
Copy code
{
  "result": "Type of Lesion"
}
Example:
Using curl to send a POST request:
 
bash
Copy code
curl -X POST http://localhost:5000/classify -H "Content-Type: application/json" -d '{"image":"base64_encoded_image"}'
Model Information
The classification model is built with Keras and trained on a dataset containing various types of skin lesions. The model file model.h5 and label encoder LE.pkl should be placed in the root directory.
 
Troubleshooting

Ensure all Python dependencies are correctly installed.

Verify that the model and label encoder files are correctly placed and accessible by the application.
Check that the base64 encoded image is formatted correctly and compatible with the expected input format of the model.
License

This project is licensed under the MIT License - see the LICENSE.md file for details.
 
Authors
Andrew Mark Dale - 100491442
Team memebers: 
Ali Istanbullu - 100905755
Chinedu Omenkukwu - 100805353
Andre Dallaire – 100337151
