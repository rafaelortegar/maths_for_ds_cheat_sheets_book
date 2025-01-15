# Maths for Data Science: From Zero to Hero

## **Course Overview**
This repository contains a comprehensive course designed to teach the mathematical foundations and advanced concepts necessary for data science. The course progresses from basic math skills to sophisticated applications in machine learning and data analysis, ensuring learners develop a deep understanding of essential topics. With interactive Jupyter Notebooks, real-world case studies, and modern tools, this course offers a practical and engaging approach to mastering mathematics for data science.

---

## **Table of Contents**

- [Maths for Data Science: From Zero to Hero](#maths-for-data-science-from-zero-to-hero)
  - [**Course Overview**](#course-overview)
  - [**Table of Contents**](#table-of-contents)
  - [**Course Index**](#course-index)
    - [**1. Introduction to Mathematics for Data Science**](#1-introduction-to-mathematics-for-data-science)
    - [**2. Foundations of Mathematics**](#2-foundations-of-mathematics)
    - [**3. Linear Algebra**](#3-linear-algebra)
    - [**4. Calculus**](#4-calculus)
    - [**5. Probability and Statistics**](#5-probability-and-statistics)
    - [**6. Discrete Mathematics**](#6-discrete-mathematics)
    - [**7. Optimization**](#7-optimization)
    - [**8. Advanced Topics**](#8-advanced-topics)
    - [**9. Practical Applications**](#9-practical-applications)
    - [**10. Real-World Case Studies**](#10-real-world-case-studies)
    - [**11. Final Project**](#11-final-project)
    - [**12. Beyond the Course**](#12-beyond-the-course)
  - [**Features**](#features)
  - [**Folder Structure**](#folder-structure)
  - [**Initial Setup**](#initial-setup)
    - [**On Linux**](#on-linux)
    - [**On Windows**](#on-windows)
  - [**Using This Repo**](#using-this-repo)
    - [**Run with Docker**](#run-with-docker)
    - [**Run Locally with Poetry**](#run-locally-with-poetry)
    - [**Run Tests**](#run-tests)
  - [**Updating a Package**](#updating-a-package)
  - [**Contributing**](#contributing)
  - [**GitHub Actions**](#github-actions)
  - [**Beyond the Course**](#beyond-the-course)

---

## **Course Index**

### **1. Introduction to Mathematics for Data Science**
- What is Mathematics for Data Science?
- Why is Math Important in Data Science?
- Overview of the Course and Learning Objectives
- Setting Up the Environment (Python, Jupyter Notebooks, Math Libraries)

### **2. Foundations of Mathematics**
- Numbers and Operations
- Basic Algebra
- Functions and Graphs

### **3. Linear Algebra**
- Vectors and Matrices
- Linear Systems
- Applications in Data Science

### **4. Calculus**
- Differentiation
- Integration
- Multivariable Calculus

### **5. Probability and Statistics**
- Probability Basics
- Statistical Concepts

### **6. Discrete Mathematics**
- Set Theory
- Combinatorics
- Graph Theory

### **7. Optimization**
- Linear Programming
- Non-Linear Optimization
- Convex Optimization

### **8. Advanced Topics**
- Information Theory
- Fourier Transform
- Numerical Methods

### **9. Practical Applications**
- Data Preprocessing and Cleaning
- Dimensionality Reduction
- Mathematics in Machine Learning

### **10. Real-World Case Studies**
- Recommender Systems
- Supply Chain Optimization
- Network Analysis
- Time Series Forecasting

### **11. Final Project**
- End-to-End Data Science Workflow

### **12. Beyond the Course**
- Resources for Further Learning
- Practice Platforms
- Staying Updated

---

## **Features**
- **Interactive Learning**: Jupyter Notebooks for hands-on practice.
- **Comprehensive Coverage**: From fundamental math concepts to real-world applications.
- **Modern Tooling**:
  - Docker for consistent development.
  - Poetry for dependency management.
  - Pre-commit hooks for code quality.
  - GitHub Actions for automation.
- **Real-World Applications**: Practical use cases and projects.

---

## **Folder Structure**

```plaintext
.
├── LICENSE                  # License file for the project
├── README.md                # Main documentation for the repository
├── book                     # Jupyter Book content
│   ├── _build               # Built files for the Jupyter Book
│   ├── _config.yml          # Global configuration
│   ├── _toc.yml             # Table of contents
│   └── ... (source content)
├── notebooks                # Interactive notebooks
├── poetry.lock              # Poetry lock file
├── pyproject.toml           # Poetry configuration
└── tests                    # Unit tests for the project
```

---

## **Initial Setup**

### **On Linux**
1. Install Python and Poetry.
2. Clone this repository.
3. Run `poetry install` to install dependencies.

### **On Windows**
1. Use pyenv-win for Python installation.
2. Install Poetry and clone this repository.
3. Run `poetry install` to install dependencies.

---

## **Using This Repo**

### **Run with Docker**
1. Build the Docker image:
   ```bash
   docker build -t maths-ds-book -f dockerfiles/Dockerfile .
   ```
2. Run the container:
   ```bash
   docker run -it -p 8888:8888 -p 8000:8000 -v $(pwd):/app maths-ds-book
   ```

### **Run Locally with Poetry**
1. Activate the Poetry environment:
   ```bash
   poetry shell
   ```
2. Run Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

### **Run Tests**
Run all unit tests with:
```bash
pytest
```

---

## **Updating a Package**
1. Add or update a dependency:
   ```bash
   poetry add <package-name>
   ```
2. Rebuild the Docker image if necessary:
   ```bash
   docker build -t maths-ds-book -f dockerfiles/Dockerfile .
   ```

---

## **Contributing**
1. Fork this repository.
2. Clone your fork and create a feature branch.
3. Make your changes and commit with clear messages.
4. Push your branch and open a Pull Request.

---

## **GitHub Actions**
This repository uses GitHub Actions for:
- **Linting**: Ensure code quality with pre-commit hooks.
- **Testing**: Run all unit tests automatically.
- **Book Deployment**: Deploy the Jupyter Book to GitHub Pages.

---

## **Beyond the Course**
- **Resources for Further Learning**:
  - Recommended Books, Online Courses, and Tutorials.
- **Practice Platforms**:
  - Kaggle, DataCamp, HackerRank.
- **Staying Updated**:
  - Math Communities, Blogs, and Research Papers.
