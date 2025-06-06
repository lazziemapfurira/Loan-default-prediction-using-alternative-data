![banner](images/Default_Prediction.png)
Banner [source](https://banner.godori.dev/)

![Python version](https://img.shields.io/badge/Python%20version-3.10%2B-lightgrey)
![GitHub last commit](https://img.shields.io/github/last-commit/lazziemapfurira/Loan-default-prediction-using-alternative-data)
![GitHub repo size](https://img.shields.io/github/repo-size/lazziemapfurira/Loan-default-prediction-using-alternative-data)
![Type of ML](https://img.shields.io/badge/Type%20of%20ML-Binary%20Classification-red)
![License](https://img.shields.io/badge/License-MIT-green)
[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/lazziemapfurira/Loan-default-prediction-app/main/streamli_app.py)
[![Open Source Love](https://badges.frapsoft.com/os/v3/open-source-200x33.png?v=103)](https://github.com/ellerbrock/open-source-badges/)
Badge [source](https://shields.io/)

# Key findings: 


## Authors

- [@lazziemapfurira](https://github.com/lazziemapfurira)

## Table of Contents

  - [People with the highest education level, and who are either husbands or wifes make more money](#people-with-the-highest-education-level-and-who-are-either-husbands-or-wifes-make-more-money)
  - [Authors](#authors)
  - [Table of Contents](#table-of-contents)
  - [Business problem](#business-problem)
  - [Data source](#data-source)
  - [Methods](#methods)
  - [Tech Stack](#tech-stack)
  - [Quick glance at the results](#quick-glance-at-the-results)
  - [Lessons learned and recommendation](#lessons-learned-and-recommendation)
  - [Limitation and what can be improved](#limitation-and-what-can-be-improved)
  - [Run Locally](#run-locally)
  - [Explore the notebook](#explore-the-notebook)
  - [App deployed on Streamlit](#app-deployed-on-streamlit)
  - [Contribution](#contribution)
  - [License](#license)




## Business problem
This app predicts the likelihood that a loan applicant will default on their loan. Financial institutions face significant risk when issuing loans, especially without clear insight into a borrower’s credit behaviour. This predictive system helps lenders assess a borrower’s default risk before approving a loan by analysing historical, behavioural, and social economic data. Predicting default probability supports smarter lending decisions minimizing financial losses while promoting responsible lending.

## Data source

- [Kaggle Home Credit Default Risk](https://www.kaggle.com/competitions/home-credit-default-risk)

## Methods

- Bivariate Analysis
- Exploratory Data Analysis 
- Feature Engineering 
- Model Interpretability
- Model deployment
## Tech Stack

- Python (refer to requirement.txt for the packages used in this project)
- Streamlit (interface for the model)


## Quick glance at the results

Correlation between the features.

![heatmap](assets/heatmap.png)

Confusion matrix of gradrient boosting classifier.

![Confusion matrix](assets/confusion_matrix.png)

ROC curve of gradrient boosting classifier.

![ROC curve](assets/roc.png)

Top 3 models

| Model     	                | AUC 	|
|-------------------	        |------------------	|
| LightGBM                  	| 88% 	            |
| CatBoost    	              | 87% 	            |
| XGBoost               	    | 86% 	            |


- ***The final model used are: LightGBM and XGBoost***
- ***Metrics used: AUC***



## Lessons learned and recommendation


## Limitation and what can be improved




## Run Locally
Initialize git

```bash
git init
```


Clone the project

```bash
git clone https://github.com/lazziemapfurira/Loan-default-prediction-app.git
```

enter the project directory

```bash
cd Credit-card-approval-prediction-classification
```

Create a conda virtual environment and install all the packages from the environment.yml (recommended)

```bash
conda env create --prefix <env_name> --file assets/environment.yml
```

Activate the conda environment

```bash
conda activate <env_name>
```

List all the packages installed

```bash
conda list
```

Start the streamlit server locally

```bash
streamlit run cc_approval_pred.py
```
If you are having issue with streamlit, please follow [this tutorial on how to set up streamlit](https://docs.streamlit.io/library/get-started/installation)

![Streamlit GIF](assets/gif_streamlit.gif)

## Contribution

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change or contribute.

## License

MIT License

Copyright (c) 2025 Lazarus Mapfurira

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

Learn more about [MIT](https://choosealicense.com/licenses/mit/) license
