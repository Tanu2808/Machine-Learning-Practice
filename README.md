# Machine Learning Practice

A structured, hands-on repository for learning **Machine Learning from
fundamentals to practical projects** using Python.

This repository documents my learning process: understanding the theory,
implementing concepts, experimenting with data, evaluating results, and
reviewing my own understanding. AI tools may support explanations,
debugging, and implementation, but I will validate the code and make
sure I can explain the important decisions myself.

> **Learning principle:** Theory → Implementation → Experimentation →
> Evaluation → Personal Review.

------------------------------------------------------------------------

## Table of Contents

-   [Objectives](#objectives)
-   [Learning Method](#learning-method)
-   [Curriculum Checklist](#curriculum-checklist)
-   [Repository Structure](#repository-structure)
-   [Standard Workflow for Each
    Topic](#standard-workflow-for-each-topic)
-   [Notebook and Review Guidelines](#notebook-and-review-guidelines)
-   [Tools and Technologies](#tools-and-technologies)
-   [Projects](#projects)
-   [Research and Paper Reproduction](#research-and-paper-reproduction)
-   [Setup](#setup)
-   [How to Run the Notebooks](#how-to-run-the-notebooks)
-   [Progress Tracking](#progress-tracking)
-   [Definition of Done](#definition-of-done)
-   [Responsible and Reproducible
    Practice](#responsible-and-reproducible-practice)
-   [Future Learning](#future-learning)
-   [Learning Resources](#learning-resources)

------------------------------------------------------------------------

## Objectives

The goals of this repository are to:

-   Build a solid conceptual understanding of Machine Learning.
-   Strengthen Python skills needed for data analysis and model
    development.
-   Understand the mathematics and assumptions behind common algorithms.
-   Implement algorithms with libraries and, where useful, from scratch.
-   Learn how to prepare data, select features, train models, and
    evaluate results.
-   Develop good experimental habits and avoid common sources of
    misleading results.
-   Build progressively more realistic ML projects.
-   Record explanations, mistakes, questions, and lessons learned.
-   Create a public portfolio that demonstrates both practical ability
    and conceptual understanding.

## Learning Method

I will follow this cycle for each major topic:

1.  **Study the theory.** Understand the problem an algorithm solves,
    its intuition, assumptions, mathematics, strengths, and limitations.
2.  **Work through a small example.** Use simple inputs and
    visualizations to make the concept concrete.
3.  **Implement in Python.** Start with a clear implementation;
    implement the core idea from scratch when appropriate.
4.  **Use established libraries.** Compare my implementation with a
    trusted library such as scikit-learn.
5.  **Experiment.** Change data, parameters, assumptions, and inputs.
    Predict outcomes before running experiments.
6.  **Evaluate.** Use suitable metrics, baselines, validation methods,
    and error analysis.
7.  **Review independently.** Explain the concept in my own words and
    answer questions without copying notes.
8.  **Document and commit.** Record findings, limitations, references,
    and next steps in GitHub.

### Using AI as a learning assistant

AI can help explain unfamiliar concepts, suggest experiments, review
code, and diagnose errors. It should not replace understanding or
verification.

-   Ask for explanations and hints, not only finished code.
-   Verify formulas, code behavior, library APIs, and claims.
-   Run the code and inspect the output.
-   Test edge cases and compare results with expected behavior.
-   Be able to explain each important code block and design decision.
-   Record what AI helped with when that context is useful.
-   Treat generated code as a proposal to inspect, test, and improve.

------------------------------------------------------------------------

## Curriculum Checklist

This checklist is a living plan. Work through it in sequence, but
revisit earlier concepts when a later algorithm requires them. Not every
item needs a separate notebook; combine related exercises when that
keeps the repository clear.

### 00 --- Environment and Python for ML

-   [ ] Install Python and configure an editor or Jupyter environment.
-   [ ] Learn variables, basic data types, operators, and control flow.
-   [ ] Practice lists, tuples, sets, and dictionaries.
-   [ ] Write functions and understand scope and return values.
-   [ ] Work with comprehensions, exceptions, and file handling.
-   [ ] Understand modules, imports, and basic object-oriented
    programming.
-   [ ] Create and use a virtual environment.
-   [ ] Install packages and record dependencies.
-   [ ] Learn basic Git and GitHub workflows.

### 01 --- Machine Learning Foundations

-   [ ] Define Artificial Intelligence, Machine Learning, and Deep
    Learning and explain how they relate.
-   [ ] Understand what Machine Learning is and when it is useful.
-   [ ] Distinguish supervised, unsupervised, semi-supervised, and
    reinforcement learning at a high level.
-   [ ] Understand regression, classification, clustering, and
    dimensionality reduction.
-   [ ] Learn the meaning of dataset, sample/observation, feature,
    target/label, and prediction.
-   [ ] Understand training, validation, and test data.
-   [ ] Learn the typical ML workflow from problem definition to
    evaluation.
-   [ ] Identify limitations, risks, and unsuitable use cases for ML.
-   [ ] Implement small examples that demonstrate these concepts.

### 02 --- Data and Python Libraries

-   [ ] Learn NumPy arrays, dimensions, shapes, indexing, slicing, and
    broadcasting.
-   [ ] Practice vectorized operations and basic linear algebra with
    NumPy.
-   [ ] Learn pandas Series and DataFrames.
-   [ ] Load, inspect, filter, sort, group, and combine datasets.
-   [ ] Understand data types, missing values, duplicates, and
    inconsistent values.
-   [ ] Learn basic plotting with Matplotlib and/or Seaborn.
-   [ ] Practice reading CSV and other common data formats.
-   [ ] Explain how rows, columns, features, and targets are represented
    in code.

### 03 --- Mathematics and Statistics for ML

-   [ ] Review scalars, vectors, matrices, and matrix operations.
-   [ ] Understand dot products and matrix multiplication.
-   [ ] Review mean, median, variance, and standard deviation.
-   [ ] Understand probability, conditional probability, and Bayes'
    theorem.
-   [ ] Learn common distributions and sampling concepts.
-   [ ] Understand covariance and correlation, including their
    limitations.
-   [ ] Review functions, slopes, derivatives, and partial derivatives.
-   [ ] Understand gradients and the intuition behind gradient descent.
-   [ ] Connect mathematical expressions to small Python
    implementations.

### 04 --- Exploratory Data Analysis and Preprocessing

-   [ ] Inspect dataset shape, columns, types, and summary statistics.
-   [ ] Analyze distributions and relationships between variables.
-   [ ] Visualize numerical and categorical features.
-   [ ] Identify missing values, duplicates, outliers, and data-quality
    issues.
-   [ ] Learn appropriate strategies for missing-value imputation.
-   [ ] Encode categorical variables when required.
-   [ ] Understand feature scaling and when standardization or
    normalization is useful.
-   [ ] Split data into training, validation, and test sets
    appropriately.
-   [ ] Recognize data leakage and prevent it.
-   [ ] Fit preprocessing steps on training data only, then apply them
    consistently.
-   [ ] Write an EDA summary with findings and limitations.

### 05 --- Supervised Learning

For each algorithm, study the intuition, objective or mathematical idea,
assumptions, hyperparameters, suitable use cases, limitations, and
evaluation.

-   [ ] Linear regression.
-   [ ] Multiple linear regression.
-   [ ] Polynomial regression and nonlinear relationships.
-   [ ] Logistic regression.
-   [ ] k-Nearest Neighbors (k-NN).
-   [ ] Decision trees.
-   [ ] Random forests.
-   [ ] Support Vector Machines (SVM).
-   [ ] Naive Bayes.
-   [ ] Compare models on a suitable dataset and explain the
    differences.

### 06 --- Unsupervised Learning

-   [ ] Understand clustering and situations where labels are
    unavailable.
-   [ ] Implement k-means clustering.
-   [ ] Explore hierarchical clustering.
-   [ ] Explore DBSCAN and density-based clustering.
-   [ ] Understand dimensionality reduction and its purpose.
-   [ ] Implement Principal Component Analysis (PCA).
-   [ ] Visualize and interpret results cautiously.
-   [ ] Understand the limitations of evaluating unsupervised models.

### 07 --- Model Evaluation and Selection

-   [ ] Establish a simple baseline before comparing complex models.
-   [ ] Understand regression metrics: MAE, MSE, RMSE, and R².
-   [ ] Understand classification metrics: accuracy, precision, recall,
    F1-score, and ROC-AUC where appropriate.
-   [ ] Interpret a confusion matrix.
-   [ ] Understand class imbalance and why accuracy can be misleading.
-   [ ] Learn cross-validation and its appropriate use.
-   [ ] Explain overfitting and underfitting.
-   [ ] Understand the bias--variance trade-off.
-   [ ] Tune hyperparameters using an appropriate validation strategy.
-   [ ] Separate model selection from final test-set evaluation.
-   [ ] Perform error analysis and document failure cases.

### 08 --- Feature Engineering and Pipelines

-   [ ] Create useful features from raw data.
-   [ ] Select features using appropriate methods.
-   [ ] Understand feature importance and its limitations.
-   [ ] Build preprocessing and modeling pipelines.
-   [ ] Use `ColumnTransformer` when different columns require different
    preprocessing.
-   [ ] Keep transformations consistent between training and inference.
-   [ ] Check for leakage in feature creation and selection.
-   [ ] Compare a model before and after justified feature engineering.

### 09 --- Implement Algorithms from Scratch

Implement the core ideas for selected algorithms to deepen
understanding. Keep the implementations educational and compare them
with library results.

-   [ ] Simple linear regression.
-   [ ] Gradient descent for a suitable objective.
-   [ ] Logistic regression for binary classification.
-   [ ] k-Nearest Neighbors.
-   [ ] Understand parameter initialization, loss, updates, and stopping
    criteria where applicable.
-   [ ] Compare scratch implementations with scikit-learn on controlled
    data.
-   [ ] Explain any differences in preprocessing, optimization, or
    numerical results.

### 10 --- Mini Projects

-   [ ] Student performance analysis or prediction.
-   [ ] House price prediction.
-   [ ] Customer churn classification.
-   [ ] Select suitable datasets and document their provenance.
-   [ ] Define the problem, target, and success metric before modeling.
-   [ ] Create a baseline, preprocessing pipeline, and at least one
    model.
-   [ ] Evaluate results and explain errors and limitations.
-   [ ] Write a project README with setup instructions and conclusions.

### 11 --- End-to-End ML Projects

-   [ ] Complete one regression project from raw data to evaluated
    model.
-   [ ] Complete one classification project from raw data to evaluated
    model.
-   [ ] Organize reusable code separately from exploratory notebooks
    where appropriate.
-   [ ] Make the workflow reproducible.
-   [ ] Document assumptions, data limitations, metrics, and failure
    modes.
-   [ ] Save model artifacts only when useful and safe to distribute.
-   [ ] Provide clear instructions for reproducing the result.
-   [ ] Optionally create an interactive demo after the core project is
    complete.

### 12 --- Research and Reproduction

-   [ ] Maintain a list of papers and technical articles to read.
-   [ ] Summarize each paper's problem, method, assumptions, results,
    and limitations.
-   [ ] Identify what is feasible to reproduce with available data and
    compute.
-   [ ] Implement a small, clearly scoped experiment inspired by a
    paper.
-   [ ] Compare reproduced results with the paper and explain
    discrepancies.
-   [ ] Cite the original paper and any code or datasets used.

------------------------------------------------------------------------

## Repository Structure

The directory structure follows the learning sequence. Create folders as
needed rather than generating empty notebooks for every future topic.

``` text
machine-learning-practice/
├── README.md
├── ROADMAP.md
├── requirements.txt
├── .gitignore
│
├── 00-setup-and-python/
├── 01-ml-foundations/
├── 02-data-fundamentals/
├── 03-data-analysis-and-preprocessing/
├── 04-mathematics-for-ml/
├── 05-supervised-learning/
├── 06-unsupervised-learning/
├── 07-model-evaluation-and-selection/
├── 08-feature-engineering/
├── 09-ml-from-scratch/
├── 10-mini-projects/
├── 11-end-to-end-ml-projects/
├── 12-research-and-reproduction/
│
└── resources/
    ├── datasets.md
    ├── references.md
    └── glossary.md
```

### Suggested structure for an algorithm

``` text
05-supervised-learning/
└── 01-linear-regression/
    ├── README.md
    ├── theory-notes.md
    ├── 01-visual-intuition.ipynb
    ├── 02-implementation-from-scratch.ipynb
    ├── 03-implementation-with-sklearn.ipynb
    ├── 04-experiments-and-analysis.ipynb
    └── review.md
```

Adapt the structure to the topic. A small exercise may need only one
notebook and a short explanation; a major algorithm or project may
justify separate theory, implementation, experiments, and review files.

------------------------------------------------------------------------

## Standard Workflow for Each Topic

Use the following checklist before marking a topic complete:

-   [ ] **Theory:** Explain the problem, intuition, assumptions, and
    limitations.
-   [ ] **Mathematics:** Understand the relevant equation or objective
    where applicable.
-   [ ] **Implementation:** Write and run a small, understandable
    example.
-   [ ] **Library comparison:** Compare with a standard library
    implementation when one exists.
-   [ ] **Experimentation:** Change inputs or parameters and observe the
    effect.
-   [ ] **Evaluation:** Select an appropriate metric or validation
    method.
-   [ ] **Error analysis:** Inspect incorrect or unexpected results.
-   [ ] **Independent explanation:** Explain the concept without copying
    the notebook.
-   [ ] **Review notes:** Record what is clear, what remains confusing,
    and what to revisit.
-   [ ] **Documentation:** Add instructions, references, and
    conclusions.
-   [ ] **Git commit:** Commit a coherent, working unit of progress.

## Notebook and Review Guidelines

### Notebook conventions

-   Give each notebook a descriptive title and state its learning
    objective.
-   Explain important code blocks in Markdown cells.
-   Keep examples small enough to understand and reproduce.
-   Set random seeds where they help make experiments reproducible.
-   Label plots and explain what they show.
-   Avoid putting passwords, tokens, or private information in
    notebooks.
-   Restart the kernel and run all cells from top to bottom before
    publishing.
-   Keep outputs that help explain the result; remove unnecessarily
    large outputs.
-   Record library or dataset requirements when they are not obvious.

### Personal review template

Use this structure in `review.md` or at the end of a notebook:

``` markdown
# Topic Review

## 1. Concept in My Own Words
Explain the idea without copying the source.

## 2. Problem It Solves
What problem is this method designed to address?

## 3. Key Assumptions
Which assumptions matter, and what happens if they do not hold?

## 4. Mathematical or Technical Intuition
Explain the important equation, objective, or mechanism.

## 5. Experiment Results
What did I change, what did I expect, and what actually happened?

## 6. Limitations and Failure Cases
When might this approach perform poorly?

## 7. Questions I Still Have
List unresolved questions.

## 8. Independent Check
Can I explain the idea and reproduce the essential implementation without following a finished solution?

## 9. Next Step
What should I revisit or learn next?
```

------------------------------------------------------------------------

## Tools and Technologies

The tools below will be introduced as they become useful. I do not need
to learn every tool before starting practical exercises.

  -----------------------------------------------------------------------
  Tool                                Purpose
  ----------------------------------- -----------------------------------
  Python                              Main programming language

  Jupyter Notebook                    Interactive experiments and
                                      explanations

  NumPy                               Numerical computing and arrays

  pandas                              Data manipulation and analysis

  Matplotlib / Seaborn                Data visualization

  scikit-learn                        Classical ML algorithms,
                                      preprocessing, pipelines, and
                                      evaluation

  Git / GitHub                        Version control, documentation, and
                                      portfolio

  VS Code or JupyterLab               Development environment

  Hugging Face Hub / Spaces           Optional sharing of selected models
                                      and interactive demos later
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## Projects

Each substantial project should have its own README. Use this outline as
a starting point:

``` markdown
# Project Name

## Problem Statement
What problem am I trying to solve?

## Objective and Success Metric
What does success mean, and how will I measure it?

## Dataset
Where did the data come from? What are its limitations?

## Approach
What analysis, preprocessing, features, and models did I use?

## Baseline
What simple method did I compare against?

## Experiments
What alternatives did I test, and why?

## Results
Which metrics did I obtain? Include relevant plots or tables.

## Error Analysis
Where does the model fail, and what might explain the failures?

## Limitations and Ethics
What should users not infer from these results?

## Reproduction
How can someone set up the environment and run the project?

## References
List datasets, documentation, papers, and other sources.
```

Project progression:

1.  **Exploratory analysis:** Learn to inspect data, ask questions, and
    communicate findings.
2.  **First predictive model:** Build a baseline and evaluate it
    correctly.
3.  **Model comparison:** Compare appropriate algorithms using
    consistent data splits and metrics.
4.  **End-to-end project:** Combine preprocessing, modeling, evaluation,
    and reproducible instructions.
5.  **Optional demo:** Publish a selected result as an interactive
    application when it adds value.

------------------------------------------------------------------------

## Research and Paper Reproduction

Research work should be scoped to the current level of understanding.
Start by reproducing a small, clearly described experiment rather than
attempting to recreate an entire complex paper.

For every paper, record:

-   Full title, authors, publication venue, year, and DOI or stable URL
    when available.
-   The problem being addressed.
-   The core idea and how it differs from previous approaches.
-   The dataset, evaluation method, and reported results.
-   The parts reproduced and the parts omitted.
-   Differences between the reported and reproduced results.
-   Limitations, questions, and follow-up experiments.

Credit original authors, respect dataset and code licenses, and clearly
distinguish reproduced results from the paper's reported findings.

------------------------------------------------------------------------

## Setup

### 1. Clone the repository

``` bash
git clone <your-repository-url>
cd machine-learning-practice
```

Replace `<your-repository-url>` with the URL of your GitHub repository.

### 2. Create a virtual environment

**Windows (PowerShell):**

``` powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

**macOS / Linux:**

``` bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

If a `requirements.txt` file is present:

``` bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

A starter `requirements.txt` can contain:

``` text
jupyter
numpy
pandas
matplotlib
seaborn
scikit-learn
```

Add other dependencies only when a notebook needs them. For long-lived
projects, record tested versions so results can be reproduced more
reliably.

### 4. Launch Jupyter

``` bash
jupyter notebook
```

Alternatively, open the repository in VS Code and select the virtual
environment as the notebook kernel.

------------------------------------------------------------------------

## How to Run the Notebooks

1.  Read the notebook's objective and prerequisites.
2.  Confirm the required packages are installed.
3.  Download or prepare the dataset as described by the notebook.
4.  Select the correct Python environment or kernel.
5.  Run the notebook from top to bottom.
6.  Inspect outputs and plots; do not assume successful execution means
    the reasoning is correct.
7.  Read the conclusion and complete the personal review.
8.  Commit the updated notebook and related documentation.

If a notebook relies on a dataset that is not stored in Git, document
where it can be obtained and how to place it in the expected location.

------------------------------------------------------------------------

## Progress Tracking

Use the checklists in this README or maintain a more detailed
`ROADMAP.md`. Mark a topic complete only when the implementation and
review reflect actual understanding---not merely because the code ran.

A useful progress log includes:

  Date         Topic        What I implemented   What I learned   Next step
  ------------ ------------ -------------------- ---------------- -------------
  YYYY-MM-DD   Topic name   Short summary        Key takeaway     Next action

Keep the log concise and update it after meaningful learning sessions.

------------------------------------------------------------------------

## Definition of Done

A topic is ready to mark complete when I can:

-   Explain the concept in my own words.
-   Identify the problem it solves and its key assumptions.
-   Run and interpret a practical implementation.
-   Explain the important parts of the code.
-   Change an input or parameter and reason about the result.
-   Evaluate the result using an appropriate method.
-   Identify at least one limitation or failure case.
-   Record questions that remain unresolved.
-   Reproduce the example from a clean environment when practical.

For major projects, also document the dataset, baseline, evaluation
strategy, error analysis, limitations, and reproduction steps.

------------------------------------------------------------------------

## Responsible and Reproducible Practice

-   Use datasets only in accordance with their licenses and terms.
-   Do not commit credentials, private information, or confidential
    datasets.
-   Avoid data leakage by keeping test data separate and fitting
    preprocessing steps only on training data.
-   Choose evaluation metrics that match the problem and its
    consequences.
-   Do not present correlation as proof of causation.
-   Explain uncertainty and limitations instead of overstating model
    performance.
-   Make experiments reproducible where practical, while recognizing
    that some numerical differences can occur across environments.
-   Cite external material, datasets, papers, and code that influenced
    an implementation.
-   Distinguish educational experiments from models validated for
    real-world deployment.

------------------------------------------------------------------------

## Future Learning

After building a solid foundation in classical Machine Learning, this
repository can lead to further learning in:

-   Deep Learning and neural networks.
-   Natural Language Processing and computer vision.
-   Modern generative AI and large language models.
-   Model deployment and APIs.
-   Testing, monitoring, and ML operations (MLOps).
-   Backend integration and system design for ML applications.

These are later stages. The immediate priority is to understand the
fundamentals, build reliable practical habits, and complete meaningful
ML projects.

------------------------------------------------------------------------

## Learning Resources

Prefer official documentation and primary sources when checking APIs or
technical claims.

-   [Python documentation](https://docs.python.org/3/)
-   [NumPy documentation](https://numpy.org/doc/)
-   [pandas documentation](https://pandas.pydata.org/docs/)
-   [Matplotlib documentation](https://matplotlib.org/stable/)
-   [scikit-learn user
    guide](https://scikit-learn.org/stable/user_guide.html)
-   [Jupyter documentation](https://docs.jupyter.org/)
-   [Git documentation](https://git-scm.com/doc)
-   [GitHub documentation](https://docs.github.com/)
-   [Hugging Face Hub
    documentation](https://huggingface.co/docs/hub/index)

Add course notes, books, papers, and other useful references to
`resources/references.md` as the learning journey develops.

------------------------------------------------------------------------

## Final Note

This repository is a record of continuous learning, not a race to
complete a checklist. I will focus on understanding concepts, testing
ideas, documenting mistakes, and improving through practical work.

**Understand the theory. Implement the idea. Test the result. Review it
yourself.**
