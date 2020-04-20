# TS-Predictive-Analysis-using-Facebook-Prophet
This is a basic python script to prepare time series for a TSA using the powerful Facebook API (Prophet)

To run the file please use a jupyter notebook (Anaconda is highly recommended, especially for mac users :))

Needed imports

        - import os
        - import sys

        - import pandas as pd # to process data
        - import numpy as np # linear algebra
        - import datetime #to manipulate date formats
        - import matplotlib.pyplot as plt # for data visualization
        - import seaborn as sns # for a better data visualization
        - import itertools # for list manipulation
        - import statsmodels.api as sm # for seasonal data exploration
        - from statsmodels.tsa.stattools import adfuller, acf, pacf,arma_order_select_ic
        - import statsmodels.tsa.api as smt
        - import scipy.stats as scs
 
### PLEASE READ FIRST ABOUT FACEBOOK PROPHET BEFORE INSTALLING IT:
some good reading:
 - https://facebook.github.io/prophet/docs/quick_start.html#python-api
 - https://cran.r-project.org/web/packages/prophet/prophet.pdf
 - https://research.fb.com/prophet-forecasting-at-scale/
 - [Is Prophet Really Better than ARIMA for Forecasting Time Series Data?](https://blog.exploratory.io/is-prophet-better-than-arima-for-forecasting-time-series-fa9ae08a5851)  
to install Prophet please follow:  

Prophet is on PyPI, so you can use pip to install it:

        bash
        pip install fbprophet
The major dependency that Prophet has is pystan. PyStan has its own [installation instructions](http://pystan.readthedocs.io/en/latest/installation_beginner.html). Install pystan with pip before using pip to install fbprophet.

After installation, you can [get started](https://facebook.github.io/prophet/docs/quick_start.html#python-api)!

Windows
On Windows, PyStan requires a compiler so you’ll need to [follow the instructions](http://pystan.readthedocs.io/en/latest/windows.html). The easiest way to install Prophet in Windows is in Anaconda.

Linux
Make sure compilers (gcc, g++, build-essential) and Python development tools (python-dev, python3-dev) are installed. In Red Hat systems, install the packages gcc64 and gcc64-c++. If you are using a VM, be aware that you will need at least 4GB of memory to install fbprophet, and at least 2GB of memory to use fbprophet.

Anaconda
Use __conda install gcc__ to set up gcc. The easiest way to install Prophet is through conda-forge: __conda install -c conda-forge fbprophet__.
