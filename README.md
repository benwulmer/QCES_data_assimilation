# QCES Climate Data: Data Assimilation

This repository contains the lecture materials and practical exercises for the **Data Assimilation** module of the QCES Climate Data course. The course introduces Bayesian methods, Kalman filters, and ensemble techniques using a pendulum as a "toy problem" to illustrate complex climate science concepts.

## 🚀 Running in Google Colab

## 🚀 Running in Google Colab

The easiest way to run these notebooks is via Google Colab. 

* **Lecture 1: Bayesian Foundations** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/da380/QCES_data_assimilation/blob/main/lectures/lecture1.ipynb)

* **Lecture 2: Kalman Filters & Ensembles** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/da380/QCES_data_assimilation/blob/main/lectures/lecture2.ipynb)


> **Note for Colab Users:** To save your progress and edits, go to **File > Save a copy in Drive**. 

--- 

## 💻 Local Installation

If you prefer to work locally, this project uses **Poetry** for dependency management.

### 1. Install Poetry
If you do not have Poetry installed, follow the [official documentation](https://python-poetry.org/docs/#installation).

### 2. Clone and Setup
Clone the repository and install the environment:
```bash
git clone [https://github.com/da380/QCES_data_assimilation.git](https://github.com/da380/QCES_data_assimilation.git)
cd data_assimilation
poetry install
poetry run jupyter notebook
```

---

### Further Reading
* Wunsch, C. (1996). *The ocean circulation inverse problem*.
* Law, K., Stuart, A. and Zygalakis, K. (2015). *Data assimilation*.
* Sanz-Alonso, D., Stuart, A. and Taeb, A. (2023). *Inverse problems and data assimilation*.