# Animal Adoption Analysis

This project, created for UT Austin's I310D (Intro to Human-Centered Data Science) by Isa Melendez, Anoushka Kancherla, and Anzhelika Lomakina, analyzes animal adoption data from the Austin Animal Center in order to understand factors influencing adoption outcomes. The analysis includes data preprocessing, exploratory data analysis, visualizations, and machine learning models (Logistic Regression and MLP Classifier) to predict adoption likelihood. Additionally, LIME is used to interpret model predictions on individual examples.

## Prerequisites

- Python 3.7 or higher
- Jupyter Notebook or JupyterLab (for running the notebook)
- Required Python packages (see Installation section)

## Installation

1. Clone or download this repository to your local machine.

2. Install the required Python packages (pandas, numpy, matplotlib, scikit-learn, and lime) using pip

## Data

The analysis uses the dataset `Austin_Animal_Center_Outcomes_20260415.csv`, which contains records of animal outcomes from the Austin Animal Center. Ensure this file is in the same directory as the notebook.

- **Source**: [Austin Animal Center](https://data.austintexas.gov/Health-and-Community-Services/Austin-Animal-Center-Outcomes/gsvs-ypi7/data_preview)
- **Description**: Includes information about animals such as type, breed, color, age, intake/outcome dates, and adoption status.

## Running the Analysis

1. Open the Jupyter Notebook `animal_adoption_analysis.ipynb` in Jupyter Notebook, JupyterLab, or VS Code.

2. Run the cells in order from top to bottom. The notebook is structured as follows:

   - **Section 1**: Load and preprocess data using pandas and numpy.
   - **Section 2**: Create analytical tables (such as adoption rates by type).
   - **Section 3**: Generate visualizations using matplotlib.
   - **Section 4**: Train and evaluate a baseline Logistic Regression classifier using scikit-learn.
   - **Section 5**: Train and evaluate a baseline MLP classifier using scikit-learn.
   - **Section 6**: Test classifiers on created examples using LIME for interpretability.

3. The notebook includes markdown cells with explanations and code cells with outputs (plots, metrics, and LIME explanations).

## Key Libraries Used

- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computations
- **matplotlib**: Data visualization
- **scikit-learn**: Machine learning (preprocessing, models, evaluation)
- **lime**: Model interpretability (LIME explanations)

## Reproducing the Results

- The notebook is self-contained and should reproduce the same results given the same data and random seeds (where applicable).
- If you encounter any issues, make sure all packages are installed and the CSV file is accessible.

## Notes

- This analysis focuses on dogs and cats only, merging "Puppy" and "Kitten" into their adult categories.
- Rare breeds and colors are grouped into "Other" categories to prevent overfitting.
- Models are evaluated using accuracy, precision, recall, F1-score, and classification reports.
- LIME is used to explain individual predictions and analyze feature contributions.
