# kaggle_tps_sep_22
book sale forecast

### TPS September 2022
Forecast book sales

#### input
- data spec: 
    - country: Belgium, France, Germany, Italy, Poland, Spain
    - store: KaggleMart, KaggleRama
    - product: 
        - Kaggle Advanced Techniques
        - Kaggle Getting Started
        - Kaggle Recipe Book
        - Kaggle for Kids
- train.csv: row_id,date,country,store,product,num_sold
    - start: 2017-01-01
    - end: 2020-12-31
- test.csv: row_id,date,country,store,product
    - start: 2021-01-01
    - end: 2021-12-31

#### output requirement
- sample_submission.csv: row_id, num_sold
- submission.csv: row_id, num_sold
    - the row_id is same as what in test.csv

#### measurement
- Symmetric mean absolute percentage error (SMAPE): https://en.wikipedia.org/wiki/Symmetric_mean_absolute_percentage_error


#### model:
- CatBoost https://catboost.ai/

#### reference:
- https://www.kaggle.com/code/vishnu123/tps-sep-22-eda-lasso-groupkfold-mean-ratios
- https://github.com/nanan4th/Tabular-Playground-Series/blob/main/TPS%20Sep%202022/TPS%20Sep%202022%20v1.0.ipynb
- https://towardsdatascience.com/catboost-regression-in-6-minutes-3487f3e5b329
- https://catboost.ai/en/docs/concepts/python-reference_catboostregressor
- https://www.projectpro.io/recipes/find-optimal-parameters-for-catboost-using-gridsearchcv-for-regression


