---
layout: archive
title: "Portfolio"
classes: wide
permalink: /portfolio/
---

---
## ML Utility Library
---
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
---
**GitHub Repository:** [https://github.com/FutureAdLabs/ttd-bid-algo](https://github.com/FutureAdLabs/ttd-bid-algo)
<img src="/assets/images/pyspark.png" width="400" height="auto" alt="" align="center" style="padding-top:15px;padding-right: 30px;" /> 

### Introduction
The objective of this project was to build a Machine Learning algorithm using an innovative statistical approach to score advertisement spaces probabilistically and translate these scores into bid values. Factors such as audience appropriateness, client budget, market trends, and ad space performance were considered. This project aims to facilitate real-time bidding for ad inventory, directly impacting financial efficiency in programmatic advertising.

#### Data Engineering
The data engineering phase involved collecting large datasets from a demand-side platform, using Python, SQL, and PySpark. While Snowflake was tested, we opted for AWS Athena for its robustness in processing BigQuery data. Data engineering was critical for building reliable and accurate models.

#### Machine Learning Model Build
Models were built based on probability distributions for success and cost, focusing on Return on Ad Spend (ROAS). The models dynamically identified appropriate bid values while adjusting to market conditions, ensuring financial optimization of ad campaigns.

#### MLOps
MLOps practices were employed to validate models, version them, and monitor their performance using MLFlow. Each module generated artifacts to ensure robust and reliable deployments, which were essential for managing significant advertising budgets effectively.

### Outcome
This project became the core component of Lorenzo, Adludio's AI-driven platform ([Lorenzo AI](https://www.adsapiens.com/about)). It delivers highly targeted, high-performance advertising at scale, and continues to evolve with new business needs, driving successful programmatic advertising campaigns globally.

---
## CI/CD
---
**GitHub Repository:** [https://github.com/FutureAdLabs/data-science-cicd/tree/alpha](https://github.com/FutureAdLabs/data-science-cicd/tree/alpha)
<img src="/assets/images/circleci.png" width="400" height="auto" alt="" align="center" style="padding-top:15px;padding-right: 30px;" /> 

### Introduction
This CI/CD project became my focus when I was promoted to Senior Engineer, as the company began to grow. Recognizing the need for improved collaboration and efficiency, I led the team toward adopting industry-standard coding practices. I then integrated these practices with segregated environment setups and a seamless deployment pipeline to production.

The primary goal was to establish proper packaging and versioning for in-house libraries. Each versioned project was deployed into AWS using CloudFormation. This custom design enabled every version to be managed through CloudFormation templates, making integration with peripheral dependencies like AWS Lambda and AWS ECR seamless.

#### Package Management
Each project version was meticulously tagged using semantic versioning and stored in a private package management server, ensuring that sensitive data and dependencies were secured. This was a key part of the CI/CD process, maintaining security and integrity across all deployments.

#### Environment Setup
Each project had its own isolated environment, complete with resources like EC2 instances and AWS EMR clusters. Infrastructure, including databases and other dependencies, was automatically built upon code deployment, allowing projects to scale independently based on their specific requirements.

#### Testing and Deployment
The CI/CD pipeline was built on CircleCI, automating testing and deployment:

      - **Automated Testing**  
        I integrated continuous testing using tools like PyTest, ensuring that code quality was maintained and bugs were caught early.

      - **Linting and Code Quality Checks**  
        Tools like Coala were used to enforce coding standards and ensure high-quality code.

      - **Automated Deployment**  
        Deployment was automated using AWS services and CloudFormation, ensuring consistency and reliability in applying infrastructure changes.

### Outcome
This project became the backbone of my CI/CD operations and has significantly improved deployment efficiency and production stability. The pipeline is now a benchmark for my team, facilitating cross-team collaboration and improving our overall development processes. By integrating industry-standard tools and practices, I built a robust and scalable CI/CD pipeline that meets the needs of our growing company.

---
## TTD Orchestrator
---
**GitHub Repository:** [https://github.com/FutureAdLabs/python-ttd-orchestrator](https://github.com/FutureAdLabs/python-ttd-orchestrator)
<img src="/assets/images/ttd.png" width="400" height="auto" alt="" align="center" style="padding-top:15px;padding-right: 30px;" /> 
<img src="/assets/images/openai.png" width="400" height="auto" alt="" align="center" style="padding-top:15px;padding-right: 30px;" /> 


### Introduction
This TTD campaign orchestration library was developed to automate the process of managing campaigns on The Trade Desk (TTD) platform. Initially, a dedicated team manually handled these tasks, but the goal of this project was to identify every human workflow and ensure it was flawlessly automated.

Around this time, Language Models (LLMs) became available and were incorporated into the design to manage the human component of the tasks, enhancing the automation process. The primary objective was to provide the data science and marketing teams with powerful tools to create, monitor, and optimize ad campaigns efficiently, eliminating human intervention.

#### Submodules 

    - Monitor  
      Uses BigQuery to collect large amounts of data periodically and focuses on monitoring and analyzing the performance of both ad groups and campaigns. Key components include:
      - Data Analysis: Reviews ad space performance, providing insights into which ad spaces yield the best campaign results.
      - Pacing Strategies: Ensures that pacing strategies align with campaign goals without overspending, helping campaigns stay within budget while achieving their objectives.

    - Planner
      Responsible for planning future campaign strategies. This submodule includes:
      - Blocklist Strategies: Develops blocklist strategies at the ad group level to exclude low-performing or harmful ad spaces.
      - Bidding Strategies: Designs optimized bidding strategies based on historical data and projected performance to maximize return on ad spend (ROAS).
      - Pacing Strategies: Plans pacing strategies to ensure steady and effective use of the budget throughout the campaign period.

    - Executor
      Manages strategy execution at both ad group and campaign levels, ensuring that all planned actions are carried out accurately and effectively.  
      - Strategy Implementation: Executes the planned strategies on The Trade Desk platform.

### Technology Stack

- **Language Models (LLMs)**: Automates human-like decision-making processes.
- **BigQuery**: Used for extensive data analysis and performance monitoring.
- **MongoDB**: Handles real-time data management and campaign health monitoring.
- **MySQL**: Utilized for structured data handling in pre-release environments.
- **The Trade Desk Platform**: The primary platform targeted by the orchestration library.

This comprehensive suite of tools ensures that every aspect of campaign orchestration, from planning to execution, is automated with a high degree of precision and efficiency.

### Outcome
The development of this TTD campaign orchestration library has dramatically improved the efficiency and effectiveness of managing ad campaigns on The Trade Desk platform. By automating campaign monitoring, planning, and execution, the library reduces manual effort and enables data-driven decision-making. This initiative also led to the creation of AdSapiens ([https://www.adsapiens.com/about](https://www.adsapiens.com/about)).

The project has proven to be a valuable asset, streamlining workflows, eliminating human intervention, and empowering strategic planning and optimization. By incorporating LLMs and automating campaign management processes, I created a robust and scalable orchestration library that meets the diverse needs of our marketing and data science teams, leading to more efficient and successful ad campaigns.