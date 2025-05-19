# Plant Disease Recognition Dashboard

## Overview
This project is a machine learning-based dashboard for recognizing plant diseases from images. It uses a Convolutional Neural Network (CNN) trained on a large dataset of plant leaf images, and provides a user-friendly web interface for disease prediction using Streamlit.

## Features
- **Image-based Disease Recognition**: Upload a plant leaf image and get instant disease prediction.
- **Deep Learning Model**: Utilizes a TensorFlow/Keras CNN trained on 38 classes of plant diseases and healthy leaves.
- **Interactive Dashboard**: Built with Streamlit for easy use and visualization.
- **Jupyter Notebooks**: Includes notebooks for model training (`Train.ipynb`) and evaluation (`Test.ipynb`).

## File Structure
- `main.py`: Streamlit app for disease recognition.
- `Train.ipynb`: Notebook for data preprocessing, model building, and training.
- `Test.ipynb`: Notebook for model evaluation and testing.
- `trained_plant_disease_model.keras`: Saved Keras model (generated after training).

## Setup Instructions
1. **Clone the repository**
   ```bash
   git clone <repo-url>
   cd Plant
   ```
2. **Install dependencies**
   Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
   Install required packages:
   ```bash
   pip install streamlit tensorflow numpy matplotlib pandas seaborn opencv-python
   ```
3. **Prepare the dataset**
   - Place your training images in a `train/` directory and validation images in a `valid/` directory, structured by class (see `Train.ipynb` for details).

4. **Train the model (optional)**
   - Run `Train.ipynb` to preprocess data and train the model. This will generate `trained_plant_disease_model.keras`.

5. **Run the dashboard**
   ```bash
   streamlit run main.py
   ```
   - Open the provided local URL in your browser to use the dashboard.

## Usage
- Go to the "Disease Recognition" page in the sidebar.
- Upload a plant leaf image.
- Click "Show Image" to preview.
- Click "Predict" to get the disease prediction.

## Dependencies
- streamlit
- tensorflow
- numpy
- matplotlib
- pandas
- seaborn
- opencv-python

## Credits
- Model and dashboard by [Your Name or Team].
- Dataset: [Specify source if public, e.g., PlantVillage].

## License
[Specify your license here] 
