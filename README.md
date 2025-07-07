# Intrusion Detection System (IDS) - UNSW-NB15

This project implements a machine learning-based Intrusion Detection System (IDS) using the UNSW-NB15 dataset. It preprocesses the data, selects key features, trains multiple classification models, and saves the best-performing model for future use.

## Features

- Data preprocessing and label encoding for categorical features
- Feature selection using F-score
- Training and evaluation of Random Forest, Gradient Boosting, and KNN classifiers
- Model comparison with accuracy and cross-validation
- Visualization of model performance
- Saving trained models and encoders for deployment

## Dataset

- **UNSW_NB15_training.csv**: Training data
- **UNSW_NB15_testing.csv**: Testing data

## Requirements

- Python 3.7+
- pandas
- scikit-learn
- seaborn
- matplotlib

Install dependencies with:

```sh
pip install pandas scikit-learn seaborn matplotlib
```

## Usage

1. **Prepare the data**  
   Place `UNSW_NB15_training.csv` and `UNSW_NB15_testing.csv` in the project directory.

2. **Run the notebook**  
   Open `reference_book_backend.ipynb` in VS Code or Jupyter Notebook and run all cells.

3. **Model Training**  
   The notebook will:
   - Preprocess and encode the data
   - Select the top 15 features
   - Train Random Forest, Gradient Boosting, and KNN models
   - Evaluate and compare their performance

4. **Model Saving**  
   The best-performing model (Random Forest) and label encoders are saved as `.pkl` files for later use:
   - `rf_model.pkl`
   - `le_service.pkl`
   - `le_state.pkl`
   - `le_protocol.pkl`
   - `le_attack.pkl`

## Project Structure

```
intrusion detection/
├── reference_book_backend.ipynb
├── UNSW_NB15_training.csv
├── UNSW_NB15_testing.csv
├── rf_model.pkl
├── le_service.pkl
├── le_state.pkl
├── le_protocol.pkl
├── le_attack.pkl
└── README.md
```

## Results

- The Random Forest model achieved the highest accuracy among the tested models.
- Model performance is visualized using a bar plot.

