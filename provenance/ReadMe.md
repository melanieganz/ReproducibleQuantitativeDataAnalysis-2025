# Provenance in Practice

This folder contains a practical exercise demonstrating the importance of data provenance in reproducible research. The notebook `ProvenanceInPractice.ipynb` presents a simple example of data analysis and challenges users to reproduce the results.

## Exercise Overview

Given the data in the .csv file on Melanie's ice cream habits, have a look at the IPython notebook and the analysis presented there. You can visualize the notebook on GitHub. Now try and redo the "scientific" analysis presented to you there! You can do it in your favorite programming language/analysis program.

**For teachers:** use the ProvenanceInPractice notebook with students - their job being to figure out how to obtain the same results

## Environment Setup

To run the notebook, you'll need to create a conda environment with the required dependencies.

### Option 1: Using the environment.yml file (Recommended)

```bash
# Create the environment from the file
conda env create -f environment.yml

# Activate the environment
conda activate provenance_env

# Launch Jupyter
jupyter notebook
```

### Option 2: Manual installation

```bash
# Create a new environment
conda create -n provenance_env python=3.12

# Activate the environment
conda activate provenance_env

# Install required packages
conda install numpy matplotlib pandas seaborn jupyter ipykernel notebook
```

## Required Packages

The notebook requires the following Python packages:
- **numpy**: For numerical computations and random number generation
- **matplotlib**: For creating plots and data visualizations
- **pandas**: For data manipulation and analysis with DataFrames
- **seaborn**: For statistical data visualization and plot styling
- **jupyter**: For running the notebook interface
- **ipykernel**: For Jupyter kernel support

## Running the Notebook

### Option 1: Jupyter Notebook Interface

1. Ensure the conda environment is activated: `conda activate provenance_env`
2. Start Jupyter: `jupyter notebook`
3. Open `ProvenanceInPractice.ipynb` in the Jupyter interface
4. Run the cells to work through the provenance exercise

### Option 2: Visual Studio Code

1. Open Visual Studio Code
2. Install the Python and Jupyter extensions if not already installed
3. Open the `ProvenanceInPractice.ipynb` file in VS Code
4. When prompted to select a kernel, choose the `provenance_env` environment:
   - Click "Select Kernel" in the top-right corner of the notebook
   - Choose "Python Environments..."
   - Select `provenance_env (Python 3.12.x)` from the list
5. Alternatively, you can:
   - Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac)
   - Type "Python: Select Interpreter"
   - Choose the interpreter from the `provenance_env` environment
6. Run the cells using `Shift+Enter` or the Run buttons

**Note**: VS Code will automatically detect conda environments. If `provenance_env` doesn't appear, ensure:
- The environment is properly created and activated once
- VS Code Python extension is up to date
- Reload VS Code window if necessary (`Ctrl+Shift+P` → "Developer: Reload Window")

## Learning Objectives

- Understand the importance of data provenance in scientific research
- Experience the challenges of reproducing results without proper documentation
- Learn best practices for documenting data generation and analysis processes
- Practice critical evaluation of data analysis claims

## Key Learning Points

### What You'll Discover:
- **Missing Information** - Critical details about data generation are absent
- **Reproducibility Challenges** - Difficulty in verifying claims without proper provenance
- **Documentation Importance** - How lack of metadata affects scientific validity

### Questions to Consider:
- How was the data collected?
- What methods were used for analysis?
- Are there any assumptions or preprocessing steps?
- Can the conclusion be verified from the provided information? we make a small exercise on provenance!
Given the data in the .csv file on Melanie's ice cream habits, have a look at the IPython notebook and the analysis presented there. You cna visualize the notebook on GitHub. Now try and redo the “scientific” analysis presented to you there! You can do it in your favorite programming language/analysis program.

**For teachers:** use the ProvenancePractice notebook with students - their job being to figure out how to obtain the same results
