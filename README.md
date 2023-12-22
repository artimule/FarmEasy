# FarmEasy - Smart Agriculture Assistance

## Overview
FarmEasy is a Smart Agriculture Assistance system built with Flask, providing features such as crop recommendation, fertilizer suggestion, and plant disease detection. It utilizes machine learning models to make informed suggestions based on user inputs and images.

## Features
- **Crop Recommendation**: Recommends suitable crops based on nutrient levels, pH, rainfall, and weather conditions.
- **Fertilizer Suggestion**: Suggests appropriate fertilizers for a given crop, considering nutrient levels.
- **Disease Detection**: Detects plant diseases from images using a deep learning model.
- **Weather API Integration**: Fetches real-time temperature and humidity data using the OpenWeatherMap API.

## Models Used
1. **Plant Disease Classification Model**: ResNet9 model for classifying plant diseases into various classes.
2. **Crop Recommendation Model**: RandomForest model for crop recommendation.
3. **Fertilizer Recommendation Data**: Utilizes a dataset with nutrient levels for various crops to suggest suitable fertilizers.

## How to Use
1. Run the Flask app (`app.py`).
2. Access the web interface through a browser.
3. Choose from the available options for crop recommendation, fertilizer suggestion, or disease detection.
4. Follow the prompts and receive recommendations or predictions.

## Files
- `models/plant_disease_model.pth`: Trained ResNet9 model for plant disease classification.
- `models/RandomForest.pkl`: Trained RandomForest model for crop recommendation.
- `utils/disease.py`: Dictionary mapping disease classes to human-readable names.
- `utils/fertilizer.py`: Dictionary mapping fertilizer recommendation keys to suggestions.
- `utils/model.py`: Definition of the ResNet9 model.
- `Data/fertilizer.csv`: Dataset with nutrient levels for various crops.

## Requirements
- Flask
- Requests
- Numpy
- Pandas
- Torch
- torchvision
- Pillow

## Running the App
1. Install the required dependencies:
    ```bash
    pip install flask requests numpy pandas torch torchvision pillow
    ```
2. Run the Flask app:
    ```bash
    python app.py
    ```
3. Access the web interface at `http://localhost:5000` in your browser.
