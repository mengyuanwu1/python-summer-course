# Python TF Sessions

This repository contains beginner-friendly Jupyter Notebook practice materials for Teaching Fellow sessions in **Introduction to Computation and Programming with Python**.

The notebooks reinforce Python basics, data structures, object-oriented programming, algorithms, recursion, searching, sorting, computational complexity, NumPy, pandas, matplotlib, scikit-learn, supervised learning, unsupervised learning, neural networks, multi-armed bandits, case-study preparation, and final project planning.

## Setup (Recommended: Local Anaconda)

This course runs everything **locally** with Anaconda + Jupyter Notebook. (Google Colab is not accessible in mainland China, so please do not rely on it.)

### 1. Install Anaconda

Download the installer from the Tsinghua TUNA mirror (much faster than anaconda.com inside China):

- https://mirrors.tuna.tsinghua.edu.cn/anaconda/archive/

Pick the newest `Anaconda3` installer for your operating system and install with the default settings. Anaconda already includes Python, Jupyter, NumPy, pandas, matplotlib, and scikit-learn — most students will not need to install anything else.

### 2. Get this repository

**Option A — Download ZIP (easiest, no git needed):** click the green **Code** button above → **Download ZIP** → unzip to a folder you can find again (for example, your Desktop).

**Option B — Class group:** the identical ZIP is shared in the class WeChat group. Same folders, same files.

**Option C — git clone** (only if you already use git):

```bash
git clone https://github.com/mengyuanwu1/python-summer-course.git
```

If GitHub is slow or the download stalls: retry, or switch to a phone hotspot.

### 3. Install requirements (only if something is missing)

Use the Tsinghua PyPI mirror — pip's default server is slow from mainland China:

```bash
pip install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple
```

Optional — make the mirror your default:

```bash
pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
```

### 4. Start Jupyter

Open **Anaconda Prompt** (Windows) or **Terminal** (macOS), go to the repository folder, and run:

```bash
jupyter notebook
```

Your browser opens at `http://localhost:8888`. Open notebooks from `notebooks/student/`.

> **Important:** start Jupyter in (or navigate to) the unzipped repository folder, so that the `data/` folder can be found by the notebooks.

### 5. Verify your setup

Run this in a notebook cell — no error message means you are ready:

```python
import numpy, pandas, matplotlib, sklearn
print("Setup complete!")
```

## Recommended Order

1. `01_python_basics_student.ipynb`
2. `02_data_structures_oop_student.ipynb`
3. `03_algorithms_complexity_student.ipynb`

Later session notebooks are being held back from the public repo for now.

## Student Notebook Notes

Student notebooks contain TODOs, blanks, debugging prompts, challenge exercises, and reflection questions. Run cells from top to bottom so variables are created before later cells use them.

## Homework Guidance

For homework, the TF sessions focus on background concepts, problem setup, tracing, debugging, and strategy rather than giving away finished answers. Before asking for help, try to bring a small hand trace, a partial attempt, or the exact error message you are stuck on.

See [Homework Guidance: How to Get Unstuck](HOMEWORK_GUIDANCE.md) for a concrete workflow and an Assignment 2 simulation checklist.

Session 3's student notebook is intentionally split into two parts: a short algorithms practice block, then an Assignment 2 bridge on `np.random`, Bernoulli trials, and planning `single_series(...)`.

## Assignment Walkthroughs

The folder `notebooks/assignment_walkthroughs/` contains student-facing scaffolds for assignment review sessions. These notebooks are for guided practice and concept review; they are not answer keys. Assignment 2 is currently published; Assignment 3 materials are being held back for now.

## Troubleshooting

- If a variable is missing, restart the kernel and run from the top.
- If a CSV file is not found, check that the `data/` folder is in the repository and that Jupyter was started in the repository folder.
- If imports fail locally, run `pip install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple`.
- If the Tsinghua mirror is busy, try the Aliyun mirror: `https://mirrors.aliyun.com/pypi/simple/`.
- If a plot does not appear, rerun the cell and check that `matplotlib.pyplot` was imported as `plt`.
- Read error messages from the bottom line upward.
