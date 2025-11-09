# NASA-Space-Shuttle-Anomaly-Detection-Sysytem
A machine learning system that automatically detects anomalies in multivariate time series data from the NASA Space Shuttle. These anomalies can correspond to system malfunctions, sensor drifts, or operational faults

# NASA Space Shuttle Anomaly Detection

## Project Overview
This project detects anomalies in NASA Space Shuttle sensor telemetry using machine learning and deep learning. The system:
- Preprocesses and analyzes multivariate time-series data
- Trains anomaly detection models
- Deploys an interactive Streamlit dashboard
- Can be containerized with Docker for cloud deployment

## Folder Structure
- `data/` - raw and processed datasets
- `notebooks/` - EDA, preprocessing, model training, evaluation
- `src/` - modular Python scripts
- `app/` - Streamlit dashboard
- `Dockerfile` - container specification
- `config.yaml` - hyperparameters and paths

## How to Run
1. Create a virtual environment:

   python -m venv venv
   source venv/bin/activate   # Linux/Mac
   venv\Scripts\activate      # Windows

2. Install dependencies:

   pip install -r requirements.txt

3. Run the Streamlit app:

   streamlit run app/streamlit_app.py

4. Build and run Docker container:

   docker build -t nasa-anomaly .
   docker run -p 8501:8501 nasa-anomaly

## Dataset
   
   Dataset

   NASA Space Shuttle telemetry sensor dataset (link in notebooks/data_preprocessing.ipynb)