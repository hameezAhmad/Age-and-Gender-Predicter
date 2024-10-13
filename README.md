# Gender and Age Prediction System

This project is a web application designed to predict the gender and age group of a person using facial images. The system consists of a React-based frontend and a Flask API backend, utilizing computer vision and machine learning techniques to provide accurate predictions.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Technologies Used](#technologies-used)
3. [System Architecture](#system-architecture)
4. [Prerequisites](#prerequisites)
5. [Getting Started](#getting-started)
    - [Setting up the Backend (Flask API)](#setting-up-the-backend-flask-api)
    - [Running the Frontend (React App)](#running-the-frontend-react-app)
6. [Using the Application](#using-the-application)
7. [Folder Structure](#folder-structure)
8. [Troubleshooting](#troubleshooting)
9. [License](#license)

## Project Overview

The Gender and Age Prediction System is an AI-powered application that uses a webcam or image upload to determine a person's gender and approximate age group. The backend processes the images using a pre-trained machine learning model, while the frontend provides an interactive interface for users to upload images or capture photos using their device's camera.

## Technologies Used

- **Frontend:** React, JavaScript, HTML, CSS
- **Backend:** Flask, OpenCV, NumPy
- **Machine Learning Frameworks:** TensorFlow / PyTorch (for pre-trained model integration)
- **Libraries:** Flask-CORS for enabling cross-origin requests, OpenCV for image processing

## System Architecture

The system is composed of two main components:
1. **Backend (Flask API)**: Handles image processing and prediction logic. It uses a machine learning model to predict the gender and age group based on the provided image.
2. **Frontend (React App)**: A web application that allows users to interact with the system by either uploading an image or using the camera to capture a photo.

## Prerequisites

Before running the project, ensure you have the following software installed on your machine:

- **Python** (3.x) and **virtualenv**
- **Node.js** and **npm**
- A virtual environment is set up for the Flask API (details below).

## Getting Started

### Setting up the Backend (Flask API)

1. **Navigate to the backend folder in your project directory.**
2. **Activate the virtual environment:**
   - On Windows:
     ```bash
     .\venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```
3. **Install dependencies (if needed):**
   If any required library is missing, install it using:
   ```bash
   pip install -r requirements.txt
   ```
   The key dependencies include `flask`, `flask_cors`, `opencv-python`, and `numpy`.

4. **Run the Flask API:**
   Execute the following command in the terminal:
   ```bash
   python app_predict.py
   ```
   The server should now be running, usually on `http://127.0.0.1:5000/` by default.

### Running the Frontend (React App)

1. **Navigate to the root directory of the React app.**
2. **Install the dependencies:**
   ```bash
   npm install
   ```
3. **Run the React app:**
   ```bash
   npm start
   ```
   This will start the development server, usually accessible at `http://localhost:3000/`.

### Note
Make sure that the Flask API is running before making predictions from the web application.

## Using the Application

1. **Launch the React web application** by navigating to `http://localhost:3000/` in your browser.
2. **Click "Get Started"** on the homepage.
3. **Choose an option:**
   - **Upload:** Select an image from your device, then click "Predict" to get the gender and age prediction.
   - **Camera:** Position your face in front of the camera, click "Capture" to take a photo, then click "Predict" to obtain the results.

## Folder Structure

```
project-root/
│
├── backend/                  # Flask API code
│   ├── venv/                 # Virtual environment folder
│   ├── app_predict.py        # Main Flask app file
│   ├── requirements.txt      # List of dependencies
│   └── ...                   # Other files for prediction logic
│
└── frontend/                 # React App code
    ├── public/               # Public files
    ├── src/                  # Source code (components, pages, etc.)
    ├── package.json          # Node dependencies
    └── ...                   # Other configuration files
```

## Troubleshooting

- **Flask API issues:**
  - Ensure the virtual environment is activated before running the `app_predict.py` file.
  - If a module is missing, use `pip install <module_name>` to install it.

- **React App issues:**
  - Make sure Node.js is installed. If not, download and install it from [Node.js official website](https://nodejs.org/).
  - If `npm start` fails, try deleting the `node_modules` folder and running `npm install` again.

## License

This project is licensed under the **Sufa International College** under the Supervision of **Mr. Arfan Shahzad**.
