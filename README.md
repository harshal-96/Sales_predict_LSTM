### README: Sales Prediction Using LSTM

---

## Project Title: Sales Prediction Using LSTM

## Project Description

This project focuses on predicting future sales using Long Short-Term Memory (LSTM) neural networks. LSTM is a type of recurrent neural network (RNN) well-suited for time series forecasting due to its ability to capture long-term dependencies. By leveraging historical sales data, the project aims to enhance the accuracy of sales forecasts, aiding businesses in inventory management, demand planning, and overall strategic decision-making.

## Features

- **Time Series Data Preprocessing**: Preparing historical sales data for model training.
- **LSTM Model Development**: Building and training an LSTM neural network for sales prediction.
- **Model Evaluation**: Assessing the model's performance using appropriate metrics.
- **Deployment**: Creating an interactive dashboard to visualize sales predictions.
- **MLOps Integration**: Using MLflow for model tracking and parameter management.

## Technologies Used

- **Programming Languages**: Python
- **Frameworks**: TensorFlow, Keras
- **Data Processing**: Pandas, NumPy
- **Visualization**: Matplotlib, Plotly
- **Model Management**: MLflow
- **Web Framework**: Flask
- **Deployment**: Docker, AWS

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/sales-prediction-lstm.git
   ```
2. Navigate to the project directory:
   ```bash
   cd sales-prediction-lstm
   ```
3. Create a virtual environment:
   ```bash
   python3 -m venv venv
   ```
4. Activate the virtual environment:
   - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```
5. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Data Preprocessing**:
   - Place your historical sales data in the `data/` directory.
   - Run the data preprocessing script to clean and prepare the data:
     ```bash
     python preprocess_data.py
     ```

2. **Model Training**:
   - Train the LSTM model using the preprocessed data:
     ```bash
     python train_model.py
     ```

3. **Model Evaluation**:
   - Evaluate the trained model on a validation dataset:
     ```bash
     python evaluate_model.py
     ```

4. **Model Deployment**:
   - Start the Flask web application to serve the model for real-time predictions:
     ```bash
     python app.py
     ```

5. **Visualization Dashboard**:
   - Access the interactive dashboard by navigating to `http://localhost:5000` in your web browser.

## Project Structure

```
sales-prediction-lstm/
│
├── data/
│   └── sales_data.csv
│
├── models/
│   └── lstm_model.h5
│
├── notebooks/
│   └── exploratory_data_analysis.ipynb
│
├── scripts/
│   ├── preprocess_data.py
│   ├── train_model.py
│   ├── evaluate_model.py
│   └── app.py
│
├── templates/
│   └── index.html
│
├── requirements.txt
├── README.md
└── Dockerfile
```

## Key Scripts

- **preprocess_data.py**: Handles data cleaning, normalization, and preparation for model training.
- **train_model.py**: Contains the LSTM model architecture and training routine.
- **evaluate_model.py**: Evaluates the model's performance on the validation dataset.
- **app.py**: Flask application script for serving the model and displaying the dashboard.

## Model Tracking with MLflow

- Initialize MLflow tracking:
  ```bash
  mlflow ui
  ```
- Log model parameters, metrics, and artifacts during training and evaluation phases.

## Docker Deployment

1. Build the Docker image:
   ```bash
   docker build -t sales-prediction-lstm .
   ```
2. Run the Docker container:
   ```bash
   docker run -p 5000:5000 sales-prediction-lstm
   ```

## Contributors

- Harshal Dhandrut - [GitHub](https://github.com/harshal-96)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
