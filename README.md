# AI4ES Datathon 2023 - Reto B - [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository contains my code submission for the AI4ES Datathon 2023, pertaining to challenge B. The challenge consisted on predicting the electricity consumption of two office buildings in Asturias, given the datasets provided by the organization.

## Approach

I extracted relevant features from the datetime values, and downloaded some exogenous datasets (temperatures, bank holidays, etc.) from the internet. In terms of models, I used a simple [LightGBM](https://github.com/microsoft/LightGBM) model optimized with [optuna](https://optuna.org/) to turn it into a table regression problem. I won the 1st place in the Future Talent category.

## Replicating the results

To replicate the results, one only needs to install the environment specified in `requirements.txt` and run the `analysys.ipynb` notebook. 

```sh
pip install -r requirements.txt
```