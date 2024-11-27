# Soccer Match Outcome Prediction

## Contributors

| **Team Member**   | **Unity ID** |
| ----------------- | ------------ |
| Apurv Choudhari   | apchoudh     |
| Chinmay Singhania | csingha      |
| Parth Kulkarni    | pnkulka2     |
| Madhur Dixit      | mvdixit      |

## Project Overview

This project predicts soccer match outcomes using different datasets and methodologies. Below is an overview of the files in this repository:

### Files

1. **Match_Outcome_Prediction_Manual_Feature_Engineering.ipynb** (Main File)

   - Implements manual feature engineering techniques for predictive modeling.
   - Uses `database.sqlite` dataset.

2. **Match_Outcome_Prediction_Featuretools.ipynb**

   - Employs automated feature engineering using Featuretools.
   - Also uses the `database.sqlite` dataset.

3. **Match_Outcome_Prediction_New_Dataset.ipynb**

   - Works with a simpler dataset derived from 10 CSV files, containing data for seasons 2015-16 to 2024-25.
   - Combines these files into a single dataset for predictions.

4. **README.md**
   - Documentation for the project.

### Datasets

**Our combined data (Contains data from both the sources)**: [Combined Data](https://drive.google.com/drive/folders/1n7oImdv3yXb7axOAgijHk7BZko4nHHJh?usp=sharing)

1. **Kaggle Dataset**: [European Soccer Database](https://www.kaggle.com/datasets/hugomathien/soccer/data)

   - Format: `database.sqlite`
   - Used in: `Match_Outcome_Prediction_Manual_Feature_Engineering.ipynb` and `Match_Outcome_Prediction_Featuretools.ipynb`.

2. **Football Data UK**: [England Matches Dataset](https://www.football-data.co.uk/englandm.php)
   - Format: 10 CSV files (2015-16 to 2024-25 seasons).
   - Used in: `Match_Outcome_Prediction_New_Dataset.ipynb`.
   - Text file explaining the meanings of the columns for the dataset. [Text file with column meanings](https://www.football-data.co.uk/notes.txt)

### Key Differences

- **Manual vs. Automated Feature Engineering**:

  - `Manual_Feature_Engineering.ipynb` applies manual techniques.
  - `Featuretools.ipynb` uses automated feature extraction.

- **Datasets**:
  - `database.sqlite` contains a structured database of European soccer matches.
  - The CSV dataset combines English Premier League match results for 10 seasons.

## Installation and Setup

1. Clone the repository.

   ```bash
   git clone <repository-url>
   cd soccer-match-outcome-predictions
   ```

2. Install dependencies.

   ```bash
   pip install -r requirements.txt
   ```

3. Ensure the datasets are placed in the correct directories:
   - Download the data files from [Combined Data](https://drive.google.com/drive/folders/1n7oImdv3yXb7axOAgijHk7BZko4nHHJh?usp=sharing).
   - Place `database.sqlite` in the root folder.
   - Combine the 10 CSV files into one file (`combined_dataset.csv`) using `Match_Outcome_Prediction_New_Dataset.ipynb`.

## How to Run

1. Launch Jupyter Notebook.

   ```bash
   jupyter notebook
   ```

2. Open the main file: `Match_Outcome_Prediction_Manual_Feature_Engineering.ipynb`.

   - Follow the steps in the notebook to preprocess data, train models, and evaluate predictions.

3. Optionally, explore other notebooks:
   - `Match_Outcome_Prediction_Featuretools.ipynb` for automated feature engineering.
   - `Match_Outcome_Prediction_New_Dataset.ipynb` for working with the simpler dataset.

## Notes

- The notebooks are designed for educational purposes and might require GPU resources for larger datasets.
- Make sure to have Python 3.8 or later installed.

---
