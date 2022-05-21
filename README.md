# *Monte Carlo Simulator*
---

## Monte Carlo Simulator
This project covers the use of API Requests and the python MCSimulator library to run financial simulations on portfolio balances.

>"The House always wins!"

## Technologies 

This project uses Python, Pandas Libraries, and the MC Simulator to run virtual projections of possible profits. 

[pandas](https://github.com/pandas-dev/pandas)
[MC-Simulator](https://github.com/ranaroussi/pandas-montecarlo)

### Installation Guide

In order to use this program please import and utilize the following libraries and dependencies: 

```python
import os
import requests
import json
import pandas as pd
from dotenv import load_dotenv
import alpaca_trade_api as tradeapi
from MCForecastTools import MCSimulation
%matplotlib inline
```

## Usage 
the following blocks of Pandas library are fundamental in executing the program. 

```python 
load_dotenv()
```
This imports the ENV file. 

```python
requests.get().json()
```
This is needed for making a request of the python library and formatting it in the JSON output.

```python
alpaca.get_bars()
```
This is needed to make an API request for the specific API "Alpaca".

```python
MCSimulation.calc_cumulative_return()
```
This is a portion of code for running the sequence of simulations for forecasting. 

```python
MCSimulation.plot_simulation()
```
This code will plot above simulation as an overlay line plot. 

![<alt text>](https://i.postimg.cc/QMs8HxhL/Screen-Shot-2022-05-21.png)

## Contributors

Jeffrey J. Wiley Jr

## License

MIT


