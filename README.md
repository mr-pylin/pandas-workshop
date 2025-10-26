# pandas-workshop

[![License](https://img.shields.io/github/license/mr-pylin/pandas-workshop?color=blue)](https://github.com/mr-pylin/pandas-workshop/blob/main/LICENSE)
[![Python Version](https://img.shields.io/badge/Python-3.13.9-yellow?logo=python&logoColor=white)](https://www.python.org/downloads/release/python-3137/)
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/0843bff4f1494209a528380dca88999a)](https://app.codacy.com/gh/mr-pylin/pandas-workshop/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
[![Code Style](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
![Repo Size](https://img.shields.io/github/repo-size/mr-pylin/pandas-workshop?color=lightblue)
![Last Updated](https://img.shields.io/github/last-commit/mr-pylin/pandas-workshop?color=orange)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen?color=brightgreen)](https://github.com/mr-pylin/pandas-workshop/pulls)

An essential guide to mastering data manipulation with Pandas, covering core to advanced techniques for managing, analyzing, and transforming structured data in data science and machine learning.

## 📖 Table of Contents

### 📖 Main Notebooks

1. [**Introduction to Pandas**](./code/01-introduction.ipynb)
1. [**Data Structures**](./code/02-data-structures.ipynb)
1. [**Data Input and Output**](./code/03-data-io.ipynb)
1. [**Indexing and Selection**](./code/04-indexing-selection.ipynb)

## 📋 Prerequisites

- 👨‍💻 **Programming Fundamentals**
  - Proficiency in **Python** (data types, control structures, functions, classes, etc.).
    - My Python Workshop: [**github.com/mr-pylin/python-workshop**](https://github.com/mr-pylin/python-workshop)
- 🔢 **Basic Knowledge of NumPy**
  - Understanding of NumPy arrays and basic operations.
    - My NumPy Workshop: [**github.com/mr-pylin/numpy-workshop**](https://github.com/mr-pylin/numpy-workshop)

## ⚙️ Setup

This project requires Python **v3.10** or higher. It was developed and tested using Python **v3.13.9**. If you encounter issues running the specified version of dependencies, consider using this version of Python.

### 📝 List of Dependencies

[![ipykernel](https://img.shields.io/badge/ipykernel-7.0.1-ff69b4)](https://pypi.org/project/ipykernel/7.0.1/)
[![matplotlib](https://img.shields.io/badge/matplotlib-3.10.7-blue)](https://pypi.org/project/matplotlib/3.10.7/)
[![numpy](https://img.shields.io/badge/numpy-2.3.4-orange)](https://pypi.org/project/numpy/2.3.4/)
[![openpyxl](https://img.shields.io/badge/openpyxl-3.1.5-lightblue)](https://pypi.org/project/openpyxl/3.1.5/)
[![pandas](https://img.shields.io/badge/pandas-2.3.3-yellow)](https://pypi.org/project/pandas/2.3.3/)
[![plotly](https://img.shields.io/badge/plotly-6.3.1-lightgrey)](https://pypi.org/project/plotly/6.3.1/)
[![pyarrow](https://img.shields.io/badge/pyarrow-22.0.0-purple)](https://pypi.org/project/pyarrow/22.0.0/)
[![scipy](https://img.shields.io/badge/scipy-1.16.2-darkblue)](https://pypi.org/project/scipy/1.16.2/)
[![sqlalchemy](https://img.shields.io/badge/sqlalchemy-2.0.44-green)](https://pypi.org/project/SQLAlchemy/2.0.44/)
[![tables](https://img.shields.io/badge/tables-3.10.2-red)](https://pypi.org/project/tables/3.10.2/)

### 📦 Installing Dependencies

#### 📦 Method 1: uv (**Recommended** ✅)

- Use [**uv**](https://docs.astral.sh/uv/) for dependency management. It handles dependencies, virtual environments, and locking versions more efficiently than pip.  
- To install exact dependency versions specified in [**uv.lock**](./uv.lock) for consistent environments **without** installing the current project as a package:

  ```bash
  uv sync --no-install-project               # Install core dependencies
  uv sync --no-install-project --all-extras  # Install core + all optional dependencies
  ```

#### 📦 Method 2: Pip

- Install all dependencies listed in [**requirements.txt**](./requirements.txt) using [**pip**](https://pip.pypa.io/en/stable/installation/):

  ```bash
  pip install -r requirements.txt
  ```

- **Note**: The [**requirements.txt**](./requirements.txt) includes complete installation of dependencies. Comment `matplotlib`, `plotlib`, `openpyxl`, `pyarrow`, `sqlalchemy` and `tables` in order to install only core dependencies.

### 🛠️ Usage Instructions

1. Open the root folder with [**VS Code**](https://code.visualstudio.com/) (`Ctrl/Cmd + K` followed by `Ctrl/Cmd + O`).
1. Open `.ipynb` files using the [**Jupyter extension**](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) integrated with **VS Code**.
1. Select the correct Python kernel and virtual environment where the dependencies were installed.
1. Allow **VS Code** to install any recommended dependencies for working with Jupyter Notebooks.

✍️ **Notes**:  

- It is **highly recommended** to stick with the exact dependency versions specified in [**uv.lock**](./uv.lock) or [**requirements.txt**](./requirements.txt) rather than using the latest package versions. The repository has been **tested** on these versions to ensure **compatibility** and **stability**.
- This repository is **actively maintained**, and dependencies are **updated regularly** to the latest **stable** versions.
- The **table of contents** embedded in the **notebooks** may not function correctly on **GitHub**.
- For an improved experience, open the notebooks **locally** or view them via [**nbviewer**](https://nbviewer.org/github/mr-pylin/pandas-workshop).

## 🔗 Useful Links

### **Pandas**

- Official Website:
  - The official website for Pandas, providing information, tutorials, and resources for the Pandas library
  - Official site: [pandas.pydata.org](https://pandas.pydata.org/)
- Documentation
  - Comprehensive guide and reference for all functionalities and features of the Pandas library
  - Doc: [pandas.pydata.org/docs](https://pandas.pydata.org/docs/)
- Source Code
  - Over 3000 contributors are currently working on Pandas.
  - Link: [github.com/pandas-dev/pandas](https://github.com/pandas-dev/pandas)

### **Looking Ahead**

- **NumPy**
  - The fundamental package for scientific computing in Python, providing support for arrays and mathematical functions
  - Official site: [numpy.org](https://numpy.org/)
  - My NumPy Workshop: [**github.com/mr-pylin/numpy-workshop**](https://github.com/mr-pylin/numpy-workshop)
- **Data Visualization**
  - A comprehensive collection of Python libraries for creating static, animated, and interactive visualizations: **Matplotlib**, **Seaborn**, and **Plotly**.
  - Official sites: [matplotlib.org](https://matplotlib.org/) | [seaborn.pydata.org](https://seaborn.pydata.org/) | [plotly.com](https://plotly.com/)
  - My MatPlotLib Workshop: [**github.com/mr-pylin/data-visualization-workshop**](https://github.com/mr-pylin/data-visualization-workshop)
- **PyTorch**
  - An open-source **machine learning** library for Python developed by [**Meta AI**](https://ai.meta.com/), used for applications such as **deep learning** and **neural networks**.
  - Official site: [pytorch.org](https://pytorch.org/)
  - My PyTorch Workshop: [**github.com/mr-pylin/pytorch-workshop**](https://github.com/mr-pylin/pytorch-workshop)
- **Media Processing**
  - A comprehensive resource to explore media processing, from fundamental concepts to advanced techniques.
  - Official sites: [opencv.org](https://opencv.org/) | [scikit-image.org](https://scikit-image.org/) | [pillow.readthedocs.io](https://pillow.readthedocs.io/en/stable/index.html) | [scipy.org](https://scipy.org/)
  - My Media Processing Workshop: [**github.com/mr-pylin/media-processing-workshop**](https://github.com/mr-pylin/media-processing-workshop)

## 🔍 Find Me

Any mistakes, suggestions, or contributions? Feel free to reach out to me at:

- 📍[**linktr.ee/mr_pylin**](https://linktr.ee/mr_pylin)

I look forward to connecting with you! 🏃‍♂️

## 📄 License

This project is licensed under the **[Apache License 2.0](./LICENSE)**.  
You are free to **use**, **modify**, and **distribute** this code, but you **must** include copies of both the [**LICENSE**](./LICENSE) and [**NOTICE**](./NOTICE) files in any distribution of your work.

### ©️ Copyright Information

- The images located in the [**assets/images/pandas/**](./assets/images/pandas/) folder are sourced from the [**Pandas documentation**](https://pandas.pydata.org/docs/) and are licensed under the [**BSD 3-Clause License**](https://github.com/pandas-dev/pandas/blob/main/LICENSE).
