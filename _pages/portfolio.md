---
layout: archive
title: "Portfolio"
classes: wide
permalink: /portfolio/
---

## ML Utility Library

**GitHub Repository:** [https://github.com/FutureAdLabs/python-mlops/tree/alpha](https://github.com/FutureAdLabs/python-mlops/tree/alpha)
<img src="/assets/images/aws.png" width="400" height="auto" alt="" align="center" style="padding-top:15px;padding-right: 30px;" /> 
<img src="/assets/images/google-cloud8906.jpg" width="400" height="auto" alt="" align="center" style="padding-top:15px;padding-right: 30px;" /> 

### Introduction
This Python-based utility project was developed to provide the data science team with a comprehensive set of tools to streamline their workflows and enhance productivity. The goal was to create a library that offered custom tools for preparing environments, managing dependencies, and integrating with various external services, including common databases like MongoDB and MySQL. This utility library addresses common tasks and challenges faced by the team, ensuring consistency and efficiency across different projects.

### Submodules

    - **AWS**  
      Tools for managing AWS resources, including EC2, S3, and EMR clusters, facilitating the team's ability to leverage cloud infrastructure for data analysis, storage, and deployment tasks.

    - **Conda**  
      Scripts for managing Conda environments, ensuring consistent and reproducible setups across projects by handling dependencies efficiently.

    - **Git**  
      Tools to automate common Git tasks and maintain version control best practices, streamlining the development workflow.

    - **Google**  
      Integrations with Google APIs like Google Sheets, automating data retrieval and collaboration with seamless access to Google services.

    - **LLM (Language Models)**  
      Integrations with language models (e.g., OpenAI), enabling advanced language processing tasks such as natural language understanding and text generation.

    - **Local Environment**  
      Tools for managing local development environments, mirroring production setups to streamline development.

    - **Native Utilities**  
      Functions for common tasks like date-time operations, file handling, and data parsing, ensuring code reusability and reliability.

    - **Slack**  
      Functions for interacting with Slack, enabling communication and notifications directly within workflows.

    - **Database**  
      Interfaces for MongoDB and MySQL to streamline common database operations like queries, transactions, and data migrations, enhancing data handling efficiency.

### Outcome
This project has proven to be a valuable asset, streamlining Python workflows, reducing setup times, and enabling seamless integration with various services. By following best practices and integrating industry-standard tools, I created a robust and scalable utility library that meets the diverse needs of our data science projects. This library promotes collaboration and consistency across the team, leading to more efficient project delivery.

---

## Real Time Bidding Algorithm

**GitHub Repository:** [https://github.com/FutureAdLabs/ttd-bid-algo](https://github.com/FutureAdLabs/ttd-bid-algo)

### Introduction
The objective of this project was to build a Machine Learning algorithm using an innovative statistical approach to score advertisement spaces probabilistically and translate these scores into bid values. Factors such as audience appropriateness, client budget, market trends, and ad space performance were considered. This project aims to facilitate real-time bidding for ad inventory, directly impacting financial efficiency in programmatic advertising.

### Data Engineering
The data engineering phase involved collecting large datasets from a demand-side platform, using Python, SQL, and PySpark. While Snowflake was tested, we opted for AWS Athena for its robustness in processing BigQuery data. Data engineering was critical for building reliable and accurate models.

### Machine Learning Model Build
Models were built based on probability distributions for success and cost, focusing on Return on Ad Spend (ROAS). The models dynamically identified appropriate bid values while adjusting to market conditions, ensuring financial optimization of ad campaigns.

### MLOps
MLOps practices were employed to validate models, version them, and monitor their performance using MLFlow. Each module generated artifacts to ensure robust and reliable deployments, which were essential for managing significant advertising budgets effectively.

### Outcome
This project became the core component of Lorenzo, Adludio's AI-driven platform ([Lorenzo AI](https://www.adsapiens.com/about)). It delivers highly targeted, high-performance advertising at scale, and continues to evolve with new business needs, driving successful programmatic advertising campaigns globally.