
## Project Structure

- **`traffic_air_sg.ipynb`**: The main Jupyter Notebook for running data analytics and modeling. It contains the entire workflow, from data preprocessing to feature importance analysis.
- **`README.md`**: Documentation for the project.

## Requirements

The project relies on Python 3 and the following libraries:

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`
- `holiday`
- `googletrans`

To install these dependencies, run:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn holiday googletrans==4.0.0-rc1
```

## Workflow

### Data Preprocessing:
- Load and clean the data.
- Merge traffic and air quality data by date and time.
- Handle missing values and outliers.

### Exploratory Data Analysis (EDA):
- Explore relationships between traffic conditions and air pollution levels using visualizations like scatter plots and heatmaps.
- Examine time trends and region-based differences.

### Feature Engineering:
- Create new features such as `is_holiday_or_weekend` to capture the effect of weekends or holidays on traffic and air quality.
- Compute traffic congestion indices.

### Machine Learning Models:
- Train a **Random Forest Regressor** to predict vehicle volume based on traffic and air quality features.
- Evaluate the model’s performance using R-squared (R²) and other metrics.

### Feature Importance:
- Identify the key features that contribute to traffic volume and air pollution levels using model-based feature importance.

### Visualization:
- Generate plots to illustrate the relationships between variables, including feature importance graphs and time series plots.

