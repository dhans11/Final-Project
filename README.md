<a name="readme-top"></a>

<div align='center'>
    <h1><b>Comprehensive Used Car Listings And Recommendation System</b></h1>
    <img src='cars.jpeg'/>
    <br><br>
    <p>This project is focused on creating a Natural Language Processing (LLM) model that can determine if reviews are positive or negative (performing sentiment analysis) and provide recommendations based on the results.</p>
    <br>

---

## FTDS-017-HCK-group-001

**Team Members**:

1. Michael Parsaoran (Data Engineer)
2. Ahmad Dani Rifai (Data Analyst)
3. Muhammad Fiqih Al-Ayubi (Data Scientist - )
4. Vicky Belario (Data Scientist - )

## Project Overview

This project focuses on performing segmentation analysis on e-commerce sales data. By employing K-Means Clustering, the objective is to segment customers effectively, providing insights for a recommender system application that tailors product recommendations to each cluster. Moreover, the project aims to assist the marketing team in crafting targeted campaigns for each segment, ultimately enhancing sales and revenue.

## Background

### Problem Statement

The dataset provides a comprehensive list of used cars with various attributes and features. The challenge is to extract meaningful insights and patterns from this data to help potential buyers make informed decisions. The key problems to address include identifying factors that influence car prices, understanding the distribution of car features, and determining the impact of different attributes on monthly installment amounts.

### Objectives

- Determine the primary factors influencing the price of used cars.
- Analyze the distribution and frequency of different car features (e.g., rear camera, sunroof).
- Examine the relationship between car attributes (e.g., brand, year, mileage) and their corresponding monthly installment amounts.
- Provide data-driven insights to assist potential buyers in evaluating and comparing used cars based on their preferences and budget.
- Identify any trends or patterns in the location of car listings and their features.

### Dataset

The dataset used in this project is sourced from Kaggle.com, uploaded by Carrie. It can be accessed [here](https://www.kaggle.com/datasets/indraputra21/used-car-listings-in-indonesia/data).

## Project Structure

### Workflow

The workflow is divided into three main phases, each assigned to different roles:

#### Data Engineering

- **Raw Data Loading**: Set up Apache Airflow DAG to load and store raw data in Postgres.
- **Fetch Data & Data Preprocessing**: Retrieve raw data from Postgres and preprocess it into cleaned data.
- **Clean Data Loading**: Store the cleaned data back into Postgres.

#### Data Analysis

- **Data Interpretation**: Analyze the cleaned data to extract insights.
- **Visualization**: Create visual representations of the analysis for easier interpretation and presentation on Tableau.
- **Reporting**: Compile findings and insights into a comprehensive report.

#### Data Science

- **Model Development**:
- **Model Optimization**:
- **Recommender System**:
- **Model Deployment**: Build an application that integrates the developed models to automate customer segmentation and product recommendations.

## Tools

- **Docker**: Containerization to ensure reproducibility of the data pipeline.
- **Apache Airflow**: Orchestration and automation of the data pipeline.
- **PostgreSQL**: Data storage and retrieval.
- **K-Means Clustering**: Used for building and training the customer segmentation model.
- **Python**: Primary programming language for data processing, analysis, and modeling.
- **Streamlit & Huggingface**: Building an application for the model and recommender system.

## Setup and Installation

To replicate this project, ensure you have the following prerequisites:

1. Dataset files, downloadable [here](#dataset).
2. Docker.
3. Python.
4. Environment Configuration: `.env` file for the Airflow containers to access PostgreSQL.

To replicate the project:

1. Clone this repository:

```bash
git clone git@github.com:dhans11/Final-Project.git
```

2. Compose the containers:

```bash
docker compose -f airflow.yaml up
```

3. Access the Airflow webserver and set up the database credentials for PostgreSQL.
4. Trigger the DAG.
5. Download the cleaned data from the PostgreSQL database.
6. Run the `modeling.ipynb` file to create the models.

Alternatively, the models are available in the repository, and a deployed model can be found on [our Huggingface]().

Visualizations are accessible on [our Tableau]().

## Conclusions & Further Improvement

The project's outcome provides valuable insights and solutions, although there is room for further development:

**Conclusion & Business Recommendations**

**Further Improvements**
