# QCES Climate Data: Data Assimilation

This repository contains the lecture materials and practical exercises for the **Data Assimilation** module of the QCES Climate Data course. The course introduces Bayesian methods, Kalman filters, and ensemble techniques using a single and double penduluns as "toy problem" to illustrate complex climate science concepts.


## Running in Google Colab

The easiest way to run these notebooks is via Google Colab. 

* **Lecture 1: Bayesian Foundations**       [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/da380/QCES_data_assimilation/blob/main/lectures/lecture1.ipynb)

* **Lecture 2: Kalman Filters & Ensembles** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/da380/QCES_data_assimilation/blob/main/lectures/lecture2.ipynb)


> **How to save your work:** > When you open these links, you are in a "playground" mode. To save your own edits and solutions, go to **File > Save a copy in Drive**. This will create a copy in your personal Google Drive that you can edit and save indefinitely.

--- 

## Local Installation

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


## Assessment: Practical Report

This module is assessed via a single written report based on the work you complete in Practical 1 and Practical 2. The report should summarise the key concepts of data assimilation you have explored, supported by the results and visualizations generated from your code.

### **Report Guidelines**
* **Format:** The report should be written in the style of a technical report or short journal article. It should be accessible to someone with general knowledge of climate science but who is not familiar with this specific project.
* **Length:** Approximately 4-5 pages (single-spaced), including figures, tables, and references.
* **Content:** Your report does *not* need to be a step-by-step account of the practicals. Instead, focus on synthesizing your findings to tell a coherent story about the methods and their application to the pendulum systems.

### **Key Topics to Address**
Your report should cover the following core areas:

1.  **The Bayesian Approach (Single Pendulum):**
    * Explain the "Forecast-Analysis" cycle.
    * **Sensitivity to the Prior:** Discuss and demonstrate how the choice of the initial prior distribution affects the assimilation results. Does the solution converge to the truth regardless of the initial guess given enough observations?
    * **Reanalysis:** Show how using future data improves the estimate of past states (smoothing).

2.  **The Ensemble Kalman Filter (Double Pendulum):**
    * Explain why ensemble methods are necessary for non-linear, high-dimensional systems (chaos).
    * **Forecast Skill:** Analyze the "predictability horizon" of the double pendulum. How long does your forecast remain reliable after the last observation? How does this depend on the specific initial conditions (e.g., low energy vs. high energy/chaotic regimes)?

### **Optional Extension: The Linear Kalman Filter**
For a deeper investigation, you may wish to attempt the following extension:
* Implement a standard **Linear Kalman Filter (KF)** for the double pendulum using the provided linearised propagator code (`double.get_linear_propagator`).
* Compare the performance of the Linear KF against the Ensemble KF (EnKF).
* **Investigation:** Identify the range of initial perturbation angles for which the Linear KF produces reasonable results before the non-linearity of the system causes it to fail.

It is not necessary to undertake this optional part of the project to obtain better marks. It is included only as a suggestion for any students who are interested. 

### **Assessment Criteria**
* **Clarity of Presentation:** Quality of writing and effectiveness of figures.
* **Quality of Analysis:** Is the interpretation of the results sound? Are the conclusions supported by the data?
* **Conceptual Understanding:** Does the report demonstrate a solid grasp of Bayesian inference, chaos, and the differences between grid-based and ensemble methods?