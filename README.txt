# Intrusion Detection System (IDS) Using Machine Learning

## Overview

The **Intrusion Detection System (IDS)** is a machine learning-based cybersecurity project designed to analyze network traffic and identify potentially malicious activities. The system uses machine learning classification algorithms to distinguish between normal network traffic and suspicious or malicious traffic.

The project aims to demonstrate how machine learning can support network security by automating traffic classification and helping identify potential cyber threats.

## Features

- Machine learning-based network intrusion detection.
- Network traffic analysis using the UNSW-NB15 dataset.
- Data preprocessing and feature preparation.
- Training and evaluation of multiple machine learning models.
- Performance comparison using classification metrics.
- Interactive web interface using Streamlit, if included in the project.
- Visualization of model performance, if implemented.

## Technologies Used

- **Programming Language:** Python
- **Data Processing:** Pandas, NumPy
- **Machine Learning:** Scikit-learn
- **Web Interface:** Streamlit
- **Dataset:** UNSW-NB15
- **Development Tools:** Jupyter Notebook, VS Code

## Dataset

This project uses the **UNSW-NB15 dataset**, a network intrusion detection dataset containing normal and malicious network traffic records.

The dataset includes network traffic features that can be used to train machine learning models for intrusion detection.

Dataset source: [UNSW-NB15 Dataset — Official UNSW Research](https://research.unsw.edu.au/projects/unsw-nb15-dataset)

Place the required dataset files in the appropriate project directory before running the application.

## Project Structure

The project may have the following structure. Adjust the filenames to match your actual repository.

```text
Intrusion-Detection-System/
│
├── streamlit_app.py
├── requirements.txt
├── README.md
├── UNSW_NB15_features.csv
│
├── notebooks/
│   └── model_training.ipynb
│
├── models/
│   └── trained_model.pkl
│
└── venv/
```

**Note:** The `notebooks/`, `models/`, and `venv/` directories shown above are examples. Keep only the files and directories that actually exist in your project. Do not commit your virtual environment.

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/aravindparepally/Intrustion-Detection-system.git
```

### 2. Navigate to the Project Directory

```bash
cd Intrustion-Detection-system
```

### 3. Create a Virtual Environment

For Windows:

```powershell
python -m venv venv
```

Activate it:

```powershell
.\venv\Scripts\Activate.ps1
```

For Linux or macOS:

```bash
python3 -m venv venv
source venv/bin/activate
```

### 4. Install Dependencies

If `requirements.txt` is available:

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

If the project does not contain `requirements.txt`, install the dependencies specified by the source code before proceeding.

## Running the Application

If the project includes `streamlit_app.py`, launch the web application with:

```bash
streamlit run streamlit_app.py
```

Open the local URL displayed in the terminal, usually:

```text
http://localhost:8501
```

If your project uses a Jupyter Notebook for training, open the notebook and execute its cells in the required order before launching the application, if applicable.

## Machine Learning Workflow

The intended workflow for a machine learning-based IDS is:

1. **Data Collection:** Load the network traffic dataset.
2. **Data Preprocessing:** Handle missing values, encode categorical features, and prepare the input features.
3. **Model Training:** Train the selected machine learning classifiers.
4. **Model Evaluation:** Evaluate the models using appropriate classification metrics.
5. **Intrusion Detection:** Classify network traffic based on the trained model.
6. **Visualization:** Present predictions and evaluation results through the notebook or web interface, if implemented.

## Evaluation Metrics

The models can be evaluated using the following metrics:

- **Accuracy:** Proportion of correctly classified records.
- **Precision:** Proportion of predicted attacks that are actual attacks.
- **Recall:** Proportion of actual attacks detected by the model.
- **F1-Score:** Harmonic mean of precision and recall.
- **Confusion Matrix:** Breakdown of correct and incorrect predictions.

For intrusion detection, precision and recall are especially important because false alarms and missed attacks have different security implications.

## Troubleshooting

**Module not found**

```bash
pip install -r requirements.txt
```

**Dataset not found**

Verify the dataset filename and path referenced in the code.

**Streamlit command not found**

```bash
python -m pip install streamlit
```

**Trained model not found**

Run the model-training notebook or script if the application depends on a model that has not yet been saved.

## Security Considerations

- Use the system for educational, research, and authorized defensive security purposes.
- Validate input data before processing.
- Do not use predictions as the sole basis for critical security decisions.
- Evaluate false positives and false negatives before considering real-world deployment.

## Future Enhancements

- Support real-time network traffic monitoring.
- Improve detection of previously unseen attacks.
- Add detailed visualizations and an alert dashboard.
- Compare additional machine learning and deep learning models.
- Optimize prediction latency and resource usage.
- Integrate logging and alerting mechanisms.

## Author

**Aravind Parepally**

GitHub: [@aravindparepally](https://github.com/aravindparepally)

## Disclaimer

This project is intended for educational and research purposes. Its detection capabilities depend on the dataset, preprocessing pipeline, trained models, and evaluation methodology. It should not be considered a replacement for a comprehensive production security system.
