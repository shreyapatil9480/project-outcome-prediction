# Project Performance Analysis

This repository contains a self‑contained data analytics project designed to showcase skills relevant to **business analysts**, **program managers**, and **data analysts**. It uses a synthetic dataset to simulate project management scenarios and demonstrates how to perform exploratory data analysis (EDA), build predictive models, and communicate results clearly.

## Contents

- **`data/project_data.csv`** – Synthetic dataset of 300 company projects with features such as budget, duration, complexity, category, region, manager experience, risk score and success outcome.
- **`analysis.ipynb`** – Jupyter Notebook that loads the dataset, performs EDA with visualizations, builds a logistic regression model to predict project success, and discusses results.
- **`requirements.txt`** – Python dependencies needed to run the notebook.

## Dataset Description

The dataset was generated synthetically (no real customer or project data is used) and includes the following columns:

| Column | Description |
|-------|-------------|
| `project_id` | Unique identifier for each project. |
| `start_date` | Date when the project began (YYYY‑MM‑DD). |
| `end_date` | Date when the project ended. |
| `duration_days` | Length of the project in days. |
| `budget_k_usd` | Budget allocated to the project, in thousands of USD. |
| `team_size` | Number of team members involved. |
| `complexity` | Complexity score from 1 (simple) to 10 (complex). |
| `category` | Project category (Digital Transformation, Infrastructure, Human Resources, Marketing, Research). |
| `region` | Region where the project took place (North, South, East, West, Central). |
| `manager_experience_years` | Years of experience of the project manager. |
| `risk_score` | Risk rating on a 0–100 scale (higher means riskier). |
| `success` | Target variable: 1 if the project was successful, 0 otherwise. |

These features were generated with realistic distributions and a logistic function to determine the probability of success based on complexity, risk, manager experience and budget. Feel free to inspect the `data/project_data.csv` file for more details.

## How to Use This Project

1. **Clone or download the repository**

   ```bash
   git clone <REPO_URL>
   cd <REPO_NAME>
   ```

2. **Install dependencies**

   It is recommended to use a virtual environment. You can install the required packages using:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   pip install -r requirements.txt
   ```

3. **Run the notebook**

   Launch Jupyter Notebook or JupyterLab, and open `analysis.ipynb`:

   ```bash
   jupyter notebook  # or `jupyter lab`
   ```

   The notebook will guide you through loading the dataset, exploring its structure, visualizing key relationships, and building a logistic regression model. You can run the cells sequentially and experiment by modifying the code or trying different algorithms.

## Extending the Project

Here are a few ideas for taking this project further:

- **Feature engineering:** Create new variables (e.g., average budget per team member, normalized risk score) and evaluate their impact on the model.
- **Model comparison:** Try other classification algorithms (Random Forest, Gradient Boosting, SVM) and compare performance using cross‑validation.
- **Interactive dashboards:** Use tools like Plotly Dash or Streamlit to build an interactive dashboard for stakeholders to explore project metrics.
- **Project timeline analysis:** Perform time series analysis on project start dates or budgets to identify trends over years or seasons.

## License

This project is provided under the MIT License. You are free to use, modify, and distribute it for learning or demonstration purposes.

## Author

This repository was generated automatically to demonstrate proficiency in data analysis and machine learning techniques. You can adapt it to your needs or use it as a template for your own analytics projects.
