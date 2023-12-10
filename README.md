PowerCo_DataScience
==============================

PowerCo is a major gas and electricity utility that supplies to corporate, SME (Small & Medium Enterprise), and residential customers. The power-liberalization of the energy market in Europe has led to significant customer churn, especially in the SME segment. They have partnered with BCG to help diagnose the source of churning SME customers.

Data Description
==========================
1. **client_data.csv**

   * 	id = client company identifier
   * 	activity_new = category of the company’s activity
   *	channel_sales = code of the sales channel
   *	cons_12m = electricity consumption of the past 12 months
   *	cons_gas_12m = gas consumption of the past 12 months
   *	cons_last_month = electricity consumption of the last month
   *	date_activ = date of activation of the contract
   *	date_end = registered date of the end of the contract
   *	date_modif_prod = date of the last modification of the product
   *	date_renewal = date of the next contract renewal
   *	forecast_cons_12m = forecasted electricity consumption for next 12 months
   *	forecast_cons_year = forecasted electricity consumption for the next calendar year
   *	forecast_discount_energy = forecasted value of current discount
   *	forecast_meter_rent_12m = forecasted bill of meter rental for the next 2 months
   *	forecast_price_energy_off_peak = forecasted energy price for 1st period (off peak)
   *	forecast_price_energy_peak = forecasted energy price for 2nd period (peak)
   *	forecast_price_pow_off_peak = forecasted power price for 1st period (off peak)
   *	has_gas = indicated if client is also a gas client
   *	imp_cons = current paid consumption
   *	margin_gross_pow_ele = gross margin on power subscription
   *	margin_net_pow_ele = net margin on power subscription
   *	nb_prod_act = number of active products and services
   *	net_margin = total net margin
   *	num_years_antig = antiquity of the client (in number of years)
   *	origin_up = code of the electricity campaign the customer first subscribed to
   *	pow_max = subscribed power
   *	churn = has the client churned over the next 3 months
----------------------------------
2. **price_data.csv**
   
   *    id = client company identifier
   *	price_date = reference date
   *	price_off_peak_var = price of energy for the 1st period (off peak)
   *	price_peak_var = price of energy for the 2nd period (peak)
   *	price_mid_peak_var = price of energy for the 3rd period (mid peak)
   *	price_off_peak_fix = price of power for the 1st period (off peak)
   *	price_peak_fix = price of power for the 2nd period (peak)
   *	price_mid_peak_fix = price of power for the 3rd period (mid peak)


Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
