# CORONAVIRUS FUTURE PREDICTION
### Last Updated: 30 August 2021

To view/edit notebook:
1. [View on Github Pages](https://vyaduvanshi.github.io/ds-projects/coronavirus-future-prediction/)
2. [View on nbviewer](https://nbviewer.jupyter.org/github/vyaduvanshi/ds-projects/blob/master/coronavirus-future-prediction/coronavirus-future-prediction.ipynb) (Does not render maps)
3. [View/Edit on Kaggle]()
4. [Edit on Google Colab](https://colab.research.google.com/drive/1XD3bK2NFmeRGfD9qnuDSkcgvNXRoziY1?usp=sharing)
5. [Edit on Binder](https://mybinder.org/v2/gh/vyaduvanshi/ds-projects/798d7311fed5ea38bf944bb8fa41a0f6bd1b7f87?urlpath=lab%2Ftree%2Fcoronavirus-future-prediction%2Fcoronavirus-future-prediction.ipynb) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/vyaduvanshi/ds-projects/HEAD?filepath=coronavirus-future-prediction%2Fcoronavirus-future-prediction.ipynb)

The main project file is `coronavirus-future-prediction.ipynb`. A normal cell-by-cell run of the file should be good enough as long as the data sources don't alter the data itself. As for the normal daily updates of data, that should not pose a problem. All data imports are done via external sources, you only need the files to do a static run of the last updated date.

The files exist to either serve a static running version of the project which would be error-free and won't break, or take care of imports in case the one executing the cells decides to use the `JUMP` points inside the project to skip sections. The use of each file is explained below-


| File        |    Purpose        |
| ------------- |:-------------:|
| static_\*.csv      | Data files to get a static error-free version of the project |
| final_\*.csv      | If you skip preprocessing and jump directly to EDA (`final_world_df.csv` if jump to ML)     |
| helper_functions.py | File containing functions and custom theme (only helpful if you jump to ML)      |
| parallel.py | If you want to implement multithreading in SARIMA grid search      |

Sources of Data:
1. https://github.com/owid/covid-19-data/tree/master/public/data
2. https://github.com/CSSEGISandData/COVID-19/
3. https://github.com/OxCGRT/covid-policy-tracker
4. https://www.google.com/covid19/mobility/
5. https://commons.wikimedia.org/wiki/Data:Cross-country_literacy_rates_-_World_Bank,_CIA_World_Factbook,_and_other_sources_(OWID_2762).tab
6. https://www.gapminder.org/data/documentation/democracy-index/
