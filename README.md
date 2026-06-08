# Python TF Sessions

This repository contains beginner-friendly Jupyter Notebook practice materials for Teaching Fellow sessions in **Introduction to Computation and Programming with Python**.

The notebooks reinforce Python basics, data structures, object-oriented programming, algorithms, recursion, searching, sorting, computational complexity, NumPy, pandas, matplotlib, scikit-learn, supervised learning, unsupervised learning, neural networks, multi-armed bandits, case-study preparation, and final project planning.

## Open Notebooks Locally

1. Clone or download this repository.
2. Open a terminal in the repository folder.
3. Install the requirements:

```bash
pip install -r requirements.txt
```

4. Start Jupyter:

```bash
jupyter notebook
```

5. Open notebooks from `notebooks/student/`.

## Open Notebooks in Google Colab

You can open a notebook from GitHub in Google Colab by choosing **File -> Open notebook -> GitHub** and pasting the repository URL. If you use Colab, keep the `data/` folder available by uploading it or cloning the repository inside Colab.

If you are using Google Colab, you may not need to install anything manually.

## Recommended Order

1. `01_python_basics_student.ipynb`
2. `02_data_structures_oop_student.ipynb`
3. `03_algorithms_complexity_student.ipynb`
4. `04_data_exploration_case_study_student.ipynb`
5. `05_supervised_learning_student.ipynb`
6. `06_unsupervised_learning_student.ipynb`
7. `07_neural_networks_and_bandits_student.ipynb`
8. `08_final_project_planning_student.ipynb`
9. `09_project_debugging_and_results_student.ipynb`
10. `10_presentation_and_report_checklist_student.ipynb`

## Student Notebook Notes

Student notebooks contain TODOs, blanks, debugging prompts, challenge exercises, and reflection questions. Run cells from top to bottom so variables are created before later cells use them.

## Troubleshooting

- If a variable is missing, restart the kernel and run from the top.
- If a CSV file is not found, check that the `data/` folder is in the repository.
- If imports fail locally, run `pip install -r requirements.txt`.
- If a plot does not appear, rerun the cell and check that `matplotlib.pyplot` was imported as `plt`.
- Read error messages from the bottom line upward.
