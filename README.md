## Experimental Evaluation of Gradient Boosting Models for Intermittent Demand Forecasting

#### Overview
The research explores the potential of gradient boosting models to improve forecasting performance.
To do this, it compared the predictions from statistical (ETS), specialized (SBA, TSB, ADIDA, IMAPA), gradient boosting regression (XGBoost, CatBoost), and the ensemble (IMAPA + CatBoost) approaches.

#### Dataset
The Royal Air Force (RAF) dataset is available in the "RAF data - 7 years demand - 5000 items.xls" file.

#### How to Use
* Either open the "RAF.ipynb" file in Google Colab by simply clicking the blue button on the first line of the Jupyter Notebook file

* Either clone the repository
  
```sh
git clone https://github.com/vkislinskii/intermittent_demand_forecasting_paper.git
```

Install all the needed packages

   ```sh
   pip install pandas
   pip install numpy
   pip install matplotlib
   pip install sklearn
   pip install statsforecast
   pip install xgboost
   pip install catboost
   pip install optuna
   ```
Finally, open either of the two projects in Jupyter Notebook 

#### Results
* Comparing single models, IMAPA performed the best, and gradient boosting models performed worse than specialized approaches.
* The CatBoost classifier improved the IMAPA model’s performance by up to 10% according to the RMSSE metric in the combination, showing that even a simple ensemble performs better than any single model.

