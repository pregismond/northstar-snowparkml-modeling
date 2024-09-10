# Predicting Food Truck Locations Using Snowpark ML and XGBoost

![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fpregismond%2Fnorthstar-snowparkml-modeling&label=Visitors&countColor=%230d76a8&style=flat&labelStyle=none)
[![License](https://img.shields.io/badge/License-Apache_2.0-0D76A8?style=flat)](https://opensource.org/licenses/Apache-2.0)
[![Python 3.10.12](https://img.shields.io/badge/Python-3.10.12-green.svg)](https://shields.io/)
[![Snowflake 8.33.1](https://img.shields.io/badge/Snowflake-8.33.1-green?style=flat&logo=snowflake&logoColor=white)](https://shields.io/)

## Disclaimer

This repository is derived from the three-part video series for ***Module 3 - Machine Learning with Snowflake: Snowpark ML Modeling***. The original code was provided by Northstar Builder Education as part of the **[Intro to Snowflake for Devs, Data Scientists, Data Engineers](https://www.coursera.org/learn/snowflake-intro-app-developers-data-scientists-data-engineers)** course on Coursera. I have made modifications to create a complete end-to-end workflow.

### Usage

* You are welcome to use this repository as a reference or starting point for your own project.

* If you choose to fork this repository, please ensure that you comply with the terms of the Apache License and give proper credit to the original authors.

## Project Scenario

As a data engineer, my obsession with the ice cream sandwiches from the Freezing Point food truck has led me to take on this project. The challenge is that the truck’s location is unpredictable. The food truck company informs me that the truck visits only one neighborhood per day, chosen by the driver, and there are eight possible neighborhoods it might go to. They also provide me with 20 years of historical location data.

My task is to load this historical data into Snowflake, a cloud-based data warehousing platform, and analyze it to identify patterns. The goal is to develop a predictive model that can forecast the truck’s location on any given day.

## Objectives

* Create and upload a dataset to Snowflake
* Clean and transform the data
* Train an XGBoost model on the prepared data
* Evaluate the model's performance
* Register the trained model in the Snowflake Model Registry

## Dataset

For this project, the Freezing Point data was generated based on the truck driver’s strict routine, which she has followed for the past 20 years to decide which neighborhood to visit each day.

Here’s her routine: In January, she visits neighborhood 1 on the 1st, 8th, 15th, 22nd, and 29th because her mother lives there, and she likes to see her weekly. She goes to neighborhood 2 on all other days in January. From February to November, she follows a pattern where she visits neighborhood 1 on the 1st, neighborhood 2 on the 2nd, neighborhood 3 on the 3rd, and so on, looping back to neighborhood 1 after neighborhood 7. This pattern continues until the end of the month, when it restarts. December is straightforward; she visits neighborhood 8 every day because she loves the holiday decorations there.

Using this description of her neighborhood selection algorithm, one year’s worth of data was generated. This dataframe was then concatenated 20 times and uploaded to Snowflake.

## Learner

[Pravin Regismond](https://www.linkedin.com/in/pregismond)

## Acknowledgments

* Northstar Builder Education © 2024 Snowflake Inc. All rights reserved.