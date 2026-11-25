# Statistical Machine Learning (ED408)

This repository contains lab assignments, implementations from scratch, optimization algorithms, and accompanying lab reports for the **Statistical Machine Learning (ED408)** course. The work is organized into three modules covering foundational supervised/unsupervised learning, metaheuristic optimization and kernel methods, and probabilistic modeling.

---

## Repository Structure

```text
statistical-machine-learning-ed408/
├── Module 1/   # Core ML algorithms, dimensionality reduction & preprocessing
├── Module 2/   # Metaheuristic optimization, regularization & kernel methods
└── Module 3/   # Expectation-Maximization (EM) algorithm
```

### Module 1: Core Machine Learning & Preprocessing
* **`Lab01_kNN_from_Scratch.ipynb`** – Implementation of the $k$-Nearest Neighbors algorithm from scratch.
* **`Lab02_Decision_Tree.ipynb`** – Decision Tree classification and analysis.
* **`Lab03_Naive_Bayes.ipynb`** – Naive Bayes classifier implementation.
* **`Lab04_Logistic_Regression_Scratch.ipynb`** – Logistic Regression built from scratch using gradient descent.
* **`Lab05_PCA_tSNE.ipynb`** – Dimensionality reduction and visualization using PCA and t-SNE.
* **`Lab06_Outlier_Detection.ipynb`** – Techniques for identifying and handling anomalies/outliers.
* **`Lab07_LogReg_vs_SVM.ipynb`** – Comparative study of Logistic Regression and Support Vector Machines (SVM).
* **`ED408_Module_1_Lab_Assignments_Report.pdf`** – Compiled lab report for Module 1.

### Module 2: Optimization, Regularization & Kernel Methods
* **`ACO.ipynb`** – Ant Colony Optimization (ACO) implementation.
* **`Genetic_Algorithm_TSP_Beginner_Notebook.ipynb`** – Genetic Algorithm applied to the Traveling Salesman Problem (TSP).
* **`Simulated_Annealing_User_Input_With_Path_.ipynb`** – Interactive Simulated Annealing with path tracking.
* **`pso.ipynb`** – Particle Swarm Optimization (PSO).
* **`Q11_L1_L2_Elastic_Net_Regularization.ipynb`** – Comparison of L1 (Lasso), L2 (Ridge), and Elastic Net regularization.
* **`Q12_Kernel_PCA_Nonlinear_Separation.ipynb`** – Kernel PCA for nonlinearly separable datasets.
* **`sml_lab(14_09) (1).ipynb`** – Additional in-class lab exercises.
* **`ED408_File_Keeping_MODULE2_Updated.pdf`** – Compiled lab report for Module 2.

### Module 3: Probabilistic Modeling
* **`EM.ipynb`** – Implementation and analysis of the Expectation-Maximization (EM) algorithm.
* **`ED408_EM_Algorithm_Report.docx`** – Detailed report covering the theory and results of the EM lab.

---

## Getting Started

### Prerequisites
Ensure you have Python 3.8+ installed along with Jupyter Notebook or JupyterLab. Most notebooks rely on standard scientific Python libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn scipy jupyter
```

### Running the Notebooks
1. Clone the repository:
   ```bash
   git clone https://github.com/gautam0211/statistical-machine-learning-ed408.git
   cd statistical-machine-learning-ed408
   ```
2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Navigate to any module folder (`Module 1`, `Module 2`, or `Module 3`) and open the desired `.ipynb` file.

---

## Author
Maintained by **[@gautam0211](https://github.com/gautam0211)** for coursework in Statistical Machine Learning (ED408).
