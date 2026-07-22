# README for Teaching Assistants

Use the student notebooks in `notebooks/student/` during TF sessions and the answer keys in `notebooks/ta_answer_key/` when checking work or preparing hints. The public repo currently shows student sessions 1-3 and TA answer keys 1-2 only; later materials are kept local for now.

## Suggested 90-minute Session Pacing

```text
0-10 min: Warm-up and concept review
10-30 min: Code-along examples
30-60 min: Guided student exercises
60-75 min: Challenge or mini-project
75-85 min: Debugging and discussion
85-90 min: Reflection and wrap-up
```

## Essential Exercises

- Notebook 01: variables, conditionals, loops, functions, debugging, grade calculator.
- Notebook 02: lists, dictionaries, lists of dictionaries, `Student` class, gradebook mini-project.
- Notebook 03: linear search, binary search, recursion, selection sort, timing.
- Notebook 04: load CSV, inspect/clean data, groupby, one labeled visualization, case-study plan.
- Notebook 05: train/test split, KNN, decision tree, evaluation, regression mini-demo.
- Notebook 06: standardization, K-means with multiple k values, elbow method, PCA plot.
- Notebook 07: MLPClassifier demo, accuracy/confusion matrix, epsilon-greedy bandit simulation.
- Notebook 08: WHAT/HOW/WHY planning table, feasibility checklist, citation checklist.
- Notebook 09: debugging categories, results table, limitations, mini-presentation.
- Notebook 10: 5-minute slide structure, report outline, reproducibility and submission checks.

## Optional Exercises

Challenge exercises and optional extensions are best for students who finish early. Encourage early finishers to add clearer explanations, extra plots, alternative model settings, or improved project planning rather than rushing ahead silently.

## How to Use Answer Keys

Answer-key notebooks keep the same headings, exercise numbers, and prompt wording as the student notebooks. They add completed solutions, expected outputs where useful, TA notes, common mistakes, and hints. Use hints first; reveal full solutions only after students have tried, tested, and explained their thinking.

## Common Setup Issues

- Missing packages: run `pip install -r requirements.txt`.
- Wrong folder: Jupyter may start outside the repository; check the `data/` folder path.
- Kernel state confusion: restart kernel and run from the top.
- Colab data issues: upload or clone the full repository so local CSVs are available.
- Plot confusion: make sure each plot cell imports or has access to `matplotlib.pyplot as plt`.

## Debugging Without Giving Away the Solution

Ask students to:

- Read the last line of the error message.
- Print variable values and types.
- Check shape, column names, and missing values for data problems.
- Explain the algorithm in words before editing code.
- Make one small change and rerun the smallest relevant cell.

Good hints are questions: "What type is this value?", "Where was this variable created?", "What does the prompt ask the function to return?", or "Which column is the target?"

## Final Project Sessions 8-10

Session 8 should help students choose a feasible individual project and state WHAT/HOW/WHY. The syllabus expects a 5-minute individual presentation and an individual written report of up to 8 pages, excluding references and appendices, with at least five scholarly sources.

Session 9 should focus on debugging, preliminary results, limitations, and mini-presentation rehearsal.

Session 10 should focus on the final talk, report structure, citation quality, reproducibility, peer review, and final submission readiness.

## Assignment Alignment

- Assignment #1: Notebook 01 functions and Notebook 02 classes.
- Assignment #2: Notebook 04 visualization and Notebook 07 randomness/bandits.
- Assignment #3: Notebooks 05, 06, and 07 scikit-learn practice.

## Assignment Walkthroughs

Use `notebooks/assignment_walkthroughs/` for student-facing Assignment 2 and Assignment 3 review sessions. Local TA-only facilitation notes can live in `notebooks/ta_assignment_walkthroughs/`, which is ignored by git and should not be published.
