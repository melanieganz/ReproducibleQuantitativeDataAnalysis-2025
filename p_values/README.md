# P-Values Computational Approach Environment

This folder contains the Jupyter notebook `p_values.ipynb` which demonstrates a computational approach to understanding p-values, based on arguments from https://f1000research.com/articles/4-621/v3.

## Environment Setup

To run the notebook, you'll need to create a conda environment with the required dependencies.

### Option 1: Using the environment.yml file (Recommended)

```bash
# Create the environment from the file
conda env create -f environment.yml

# Activate the environment
conda activate p_values_env

# Launch Jupyter
jupyter notebook
```

### Option 2: Manual installation

```bash
# Create a new environment
conda create -n p_values_env python=3.12

# Activate the environment
conda activate p_values_env

# Install required packages
conda install numpy matplotlib seaborn scipy jupyter ipykernel notebook
```

## Required Packages

The notebook requires the following Python packages:
- **numpy**: For numerical computations and array operations
- **matplotlib**: For creating plots and visualizations
- **seaborn**: For statistical data visualization and styling
- **scipy**: For statistical functions (t-tests, probability distributions)
- **jupyter**: For running the notebook interface
- **ipykernel**: For Jupyter kernel support

## Running the Notebook

### Option 1: Jupyter Notebook Interface

1. Ensure the conda environment is activated: `conda activate p_values_env`
2. Start Jupyter: `jupyter notebook`
3. Open `p_values.ipynb` in the Jupyter interface
4. Run the cells to explore the computational approach to p-values

### Option 2: Visual Studio Code

1. Open Visual Studio Code
2. Install the Python and Jupyter extensions if not already installed
3. Open the `p_values.ipynb` file in VS Code
4. When prompted to select a kernel, choose the `p_values_env` environment:
   - Click "Select Kernel" in the top-right corner of the notebook
   - Choose "Python Environments..."
   - Select `p_values_env (Python 3.12.x)` from the list
5. Alternatively, you can:
   - Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac)
   - Type "Python: Select Interpreter"
   - Choose the interpreter from the `p_values_env` environment
6. Run the cells using `Shift+Enter` or the Run buttons

**Note**: VS Code will automatically detect conda environments. If `p_values_env` doesn't appear, ensure:
- The environment is properly created and activated once
- VS Code Python extension is up to date
- Reload VS Code window if necessary (`Ctrl+Shift+P` → "Developer: Reload Window")

## Notebook Content

The notebook covers:
- Definition of p-values with computational examples
- Bootstrap simulations under the null hypothesis
- Common misconceptions about p-values
- Visualization of p-value distributions
- Effect of sample size and effect size on p-values
