# Simple Local Regression for Mortality Rate Prediction

This project explores the use of **local linear regression** to predict mortality rates (`MORT`) based on the percentage of families living in poverty (`POOR`). The dataset can be found in the file "pollution_cleaneddata.csv" with the code in the notebook file "Exercise_LinearRegression.ipynb". 

The regression is formulated as a weighted least-squares optimization problem, where nearby observations are given different weights according to their distance from the prediction point.

The project compares **three weighting methods** and investigates how the choice of the number of neighboring observations affects the fitted regression and prediction accuracy. The models are used to estimate mortality rates for poverty levels of **10%, 18%, and 25%**, including the corresponding standard errors.

The repository contains the implementation, visualizations, and results used to evaluate the different weighting strategies and neighborhood sizes.

## Environment Setup

This project uses **Conda** for environment and package management. The required packages and versions are specified in `environment.yml`.

### 1. Create the environment

Clone the repository and navigate to the project directory:

```bash
git clone <repository-url>
cd <repository-name>
```

Create the Conda environment using the provided `environment.yml` file:

```bash
conda env create -f environment.yml
```

### 2. Activate the environment

```bash
conda activate statistics
```

### 3. Verify the installed packages

You can check the installed packages with:

```bash
conda list
```

Or check the main dependencies individually:

```bash
conda list numpy
conda list scipy
conda list matplotlib
```

### 4. Recreate or update the environment

If the environment already exists and you want to update it according to `environment.yml`:

```bash
conda env update -f environment.yml --prune
```

### 5. Deactivate the environment

When you are finished:

```bash
conda deactivate
```

### Environment

The current environment uses:

* Python 3.14
* NumPy 2.5.3
* SciPy 1.18.0
* Matplotlib 3.11.1
