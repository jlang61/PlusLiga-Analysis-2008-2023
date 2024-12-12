# Men's Volleyball Analysis (PlusLiga 2008-2023)

This repository contains an exploratory data analysis and predictive modeling project focused on the **PlusLiga**, the top professional men's volleyball league in Poland. The dataset spans the years 2008 to 2023 and includes detailed match statistics, enabling deep insights into team performances and volleyball techniques.

## Features

### Data Source

The dataset was sourced from [Kaggle](https://www.kaggle.com/), specifically the **Men’s Volleyball - PlusLiga - 2008-2023** dataset shared by user `kacpergregorowicz`. The data was compiled from the official PlusLiga volleyball website and contains rich match-level statistics.

### Machine Learning Analysis Highlights

- **Data Transformation**: Data manipulation was employed to split team-specific statistics (e.g., Team 1 and Team 2) into individual observations for better compatibility with predictive models.

- **Exploratory Data Analysis (EDA)**:

  - Distribution plots to explore match outcomes (win/loss).
  - Relationship analysis between attacking efficiency and match outcomes using jitter plots.
  - Multi-variable comparisons of serving and attacking efficiencies across teams using faceted scatter plots.
  - Correlation matrix visualization to identify key relationships between variables.

- **Techniques for Data Tidying**:

  - Converted percentage values and other character fields into numeric formats.
  - Leveraged AI-guided functions for consistent variable naming (e.g., `clean_names`).

### Key Scripts

- **Data Loading and Cleaning**: Scripts for importing and preprocessing the dataset, including handling missing values and converting character columns to numeric.
- **Visualization**: Scripts to generate key insights through plots using `ggplot2`.
- **Model Preparation**:
  - Splitting data into training and testing sets with stratification to preserve outcome distributions.
  - Initial exploration of important predictors using visual and statistical methods.

### Machine Learning Integration

The project heavily utilized Machine Learning to:

- Provide recommendations for data transformation strategies.
- Enhance the exploratory analysis by suggesting and validating visualization approaches.
- Assist in multivariate analysis by integrating intuitive insights and practical coding solutions.

### Machine Learning Methods Used

- **Logistic Regression**: Used to predict match winners based on significant predictors like attacking efficiency and blocking performance. This method is simple and interpretable, making it useful for understanding the impact of individual predictors.
- **Linear Discriminant Analysis**: Applied to classify match outcomes by finding a linear combination of features that best separates the classes (winners and losers).
- **Quadratic Discriminant Analysis**: Used for classification with non-linear decision boundaries, allowing for more flexibility in modeling the relationship between features and match outcomes.
- **Elastic Net**: Combines Lasso and Ridge regression for variable selection and regularization. This method helps in handling multicollinearity and selecting important features by applying both L1 and L2 penalties.
- **Random Forests**: Applied to understand variable importance and create robust predictions of match outcomes. This ensemble method builds multiple decision trees and combines their predictions to improve accuracy and control overfitting.
- **Boosted Trees**: Used to improve prediction accuracy by combining multiple weak models. This method sequentially builds trees, with each tree correcting the errors of the previous ones, leading to a strong overall model.

### Example Analyses

- **Win Prediction Based on Attacking Efficiency**:
  Teams with higher attacking efficiencies were more likely to win their matches, though serving efficiency had limited predictive power.
- **Team-Specific Performance Trends**:
  Observed variability in serving and attacking efficiencies across teams, highlighting inconsistencies and standout performers.

## Dependencies

- **R Programming Language**
  - `tidyverse`
  - `dplyr`
  - `ggplot2`
  - `visdat`
  - `corrplot`

## Installation and Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/mens-volleyball-analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd mens-volleyball-analysis
   ```
3. Open the R scripts or R Markdown file to explore the analysis.

## Future Directions

- Implementation of advanced machine learning models to predict match winners with higher accuracy.
- Further exploration of individual player statistics (if available).
- Development of interactive dashboards for real-time visualization.

## Acknowledgments

- Dataset by [kacpergregorowicz](https://www.kaggle.com/kacpergregorowicz).
- The official **PlusLiga** website for making match data accessible.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

