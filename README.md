# IRIS Species Detection — Decision Tree Classifier

**Overview**
- **Purpose:**: A compact project demonstrating species classification on the classic Iris dataset using a Decision Tree classifier. The repository contains a runnable Python script and an exploratory Jupyter notebook that train, evaluate, and visualize model results.
- **Scope:**: Educational/example code for supervised classification, model evaluation, and simple feature analysis.

**Files**
- **`iris_species_decisiontree.py`**: Script to load the Iris dataset, train a Decision Tree classifier, evaluate performance, and save/print basic results.
- **`iris_species_decisiontree.ipynb`**: Interactive notebook with step-by-step data exploration, visualization, model training, and evaluation. Good for learning and demonstration.
- **`README.md`**: This file — project overview and usage instructions.

**Requirements**
- **Python:**: 3.8 or newer recommended.
- **Main packages:**: `scikit-learn`, `pandas`, `numpy`, `matplotlib`, `seaborn`, and `jupyter` (for the notebook).

**Installation**
- **Clone the repo:**

```powershell
git clone https://github.com/ChinmayaPanda38/IRIS_SPECIES_DETECTION.git
cd IRIS_SPECIES_DETECTION
```

- **Create a virtual environment (recommended):**

```powershell
python -m venv .venv; .\.venv\Scripts\Activate.ps1
```

- **Install dependencies:**

```powershell
pip install --upgrade pip
pip install scikit-learn pandas numpy matplotlib seaborn jupyter
```

Optionally, create a `requirements.txt` by running `pip freeze > requirements.txt` after installing.

**Usage**
- **Run the script:** The script `iris_species_decisiontree.py` is written to run end-to-end (train → evaluate → print/save results).

```powershell
python iris_species_decisiontree.py
```

- **Open the notebook:** Launch Jupyter and open `iris_species_decisiontree.ipynb` for an interactive walkthrough.

```powershell
jupyter notebook iris_species_decisiontree.ipynb
```

**What the project does**
- **Data loading:** Uses the classic Iris dataset (from `sklearn.datasets`) containing measurements for three iris species.
- **Model:** Trains a `DecisionTreeClassifier` to predict species from the four input features (sepal/petal length and width).
- **Evaluation:** Produces standard classification metrics (accuracy, precision, recall, F1) and visualizations (confusion matrix, decision boundaries/feature importance) — implemented in the notebook and summarized by the script.

**Reproducibility & Notes**
- **Random state:**: If the repository code uses randomness (train/test split, model state), set a fixed `random_state` for reproducible results.
- **Expected results:**: Results will vary slightly depending on package versions and random seed, but the Iris dataset is simple — typical Decision Tree accuracy is high (>90% on hold-out splits) for default settings.
- **Extending:** Swap the classifier (e.g., `RandomForestClassifier`, `SVC`) or add hyperparameter search (GridSearchCV) for experiments.

**Project structure summary**
- **Data:** The dataset is loaded at runtime from `sklearn.datasets` — no external data files are required.
- **Outputs:** The script prints evaluation metrics and may save figures or a trained model if implemented.

**Contributing**
- **Issues & PRs:**: Open issues or pull requests for bugs, suggested improvements, or enhancements.
- **Style:**: Keep changes focused, add tests or a short note in the PR describing the change, and ensure reproducibility where possible.

**Contact**
- **Contact:**: For questions or help, open an issue in the repository or contact the maintainer (repository owner).
