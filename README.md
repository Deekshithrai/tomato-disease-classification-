# Tomato Disease Classification

This project is a web application built with FastAPI and TensorFlow for classifying tomato diseases based on uploaded images. Users can upload an image of a tomato plant leaf, and the application will provide a prediction of the disease class along with a confidence score.

![Screenshot (6)](https://github.com/Deekshithrai/tomato-disease-classification-/assets/144473857/186e9a1e-c03d-495d-8900-eb43b60b2da4)

## Prerequisites

Before running the application, ensure that you have the following dependencies installed:

- Python 3.x
- FastAPI
- TensorFlow (for the pre-trained model)
- Pillow (PIL)
- uvicorn (for serving the FastAPI application)
- A modern web browser (for accessing the web interface)

You can install these dependencies using `pip`:

```bash
pip install fastapi tensorflow pillow uvicorn
```
## Usage
1. Clone this repository to your local system.

2.Navigate to the project directory.

3. Place your pre-trained TensorFlow model in the "saved_models/1" directory. Make sure the model is ready for inference and can classify tomato diseases.

4. Ensure that the HTML file is available at the specified path ("api/image.html") for serving the upload form.

5. Run the FastAPI application using uvicorn:
```bash
uvicorn main:app --host localhost --port 8080
```

1. Access the web application in your browser by visiting "http://localhost:8080/upload".

2. You will see a web page with a form that allows you to upload an image file.

3. Click the "Choose File" button to select an image file. The label will update to display the selected file name.

4. Click the "Predict" button to submit the image for classification.

5. The application will make predictions using the pre-trained model and display the predicted class and confidence score on the web page.

## Customization
1. You can customize the model's class names and structure by modifying the code in the FastAPI application as needed. Update the CLASS_NAMES list and model loading code in "main.py" to match your specific use case.

2. You can modify the HTML interface ("api/image.html") to change the appearance or layout of the web page as desired.

## Deployment
For deployment in production, you may want to use a production-ready web server, such as Gunicorn, instead of uvicorn. Additional configuration may be required to ensure security and performance.

## Acknowledgments
1. This project uses FastAPI for building the web application.
2. The TensorFlow model for tomato disease classification is provided by the user.
## License
This project is open-source and available under the MIT License.
