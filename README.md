# Real Estate Analyser

### Real Estate Analyser proides investors with data visualization techniques, including aggregation, interactive visualizations, and geospatial analysis, to find properties in the San Francisco market that are viable investment opportunities. This tool can be used to analyse potential real estate investment opportunities in any other locations too.

---

![RealEstate](Images/real_estate.png)

---

## Table of contents

1. [Technologies](#technologies)
2. [Installation Guide](#installation-guide)
3. [Usage](#usage)
4. [Contributors](#contributors)
5. [License](#license)

---

## Technologies

`Python 3.9`

`Jupyter lab`

_Prerequisites_

1. Pandas is a Python package that provides fast, flexible, and expressive data structures designed to make working with large sets of data easy and intuitive.

- [pandas](https://github.com/pandas-dev/pandas) - For the documentation, installation guide and dependencies.

- [matplotlib ](https://matplotlib.org/) - For guidance on how to start visualization, interactive visualization, styles and layouts customazation.

2. Python modules and libraries to facilitate API requests:

- Requests: The Python Requests library helps you access data via APIs.

- JSON: This library puts the response (that is, the data) from an API into a human-readable format.

  The Requests and JSON libraries get installed with Anaconda. To verify, in Terminal type:

```python
conda list requests
conda list json
```

3. Python-dotenv Library is used to interact with APIs. With the python-dotenv library, you can read key-value pairs from an environment file (.env) and add them as environment variables.

4. Alpaca is an API for stock trading. With the Alpaca SDK, you can interact with the Alpaca API. Sign up for the Alpaca API Key and Secret Keys at https://app.alpaca.markets/signup

---

## Installation Guide

Jupyter lab is a preferred software to work with Risk Return Analysis application.<br/> Jupyter lab is a part of the **[anaconda](https://www.anaconda.com/)** distribution package and therefore it is recommended to download **anaconda** first.<br/> Once dowloaded, run the following command in your terminal to lauch Jupyter lab:

```python
jupyter lab
```

Before using the application first install the following dependencies by using your terminal:

To install pandas run:

```python
#  PuPi
pip install pandas
```

```python
# or conda
conda install pandas
```

If Requests and JSON libraries are missing, in Terminal run:

```python
conda install -c anaconda requests
conda install -c jmcmurray json
```

To install the python-dotenv Library, in Terminal run:

```python
pip install python-dotenv
```

To Install the Alpaca SDK, in Terminal run:

```python
pip install alpaca-trade-api
```

---

## Usage

> Application summary<br/>

Fiancial Planner consists of two financial analysis tools:

1. **A financial planner for emergencies.**<br/>The fund owners (memeber of the union in our example) will be able to use this tool to visualize their current savings:<br/>
   ![Composition2](Images/Portf_comp.PNG)
   ![Composition](Images/Composition.PNG)

The members can then determine if they have enough reserves for an emergency fund by comparing the value of their portfolio to the emergency reserves threshold amount.

2. **A financial planner for retirement.** <br/>This tool will forecast the performance of members' retirement portfolio for different time horizons (in 30 and 10 years in our example) and for different asset allocations. To do this, the tool will make an Alpaca API call via the Alpaca SDK to get historical price data for use in Monte Carlo simulations. Monte Carlo simulation will calculate the range of possible outcomes based on your asset mix, chosen investment horizon and a number of simulation runs.<br/> The application users will be presented with:

- `Simulation outcomes:`<br/>
  30Y:<br/>
  ![30ySim](Images/MC_30year_sim_plot.png)<br/>

  10Y:<br/>
  ![10ySim](Images/MC_10year_sim_plot.png)

- `Probability distribution of the Monte Carlo simulation`:<br/>
  30Y:<br/>
  ![30yDis](Images/MC_30year_dist_plot.png)<br/>

  10Y:<br/>
  ![10yDis](Images/MC_10year_dist_plot.png)

- `The summary statistics that you generated from the Monte Carlo simulation:`<br/>
  30Y:<br/>
  ![30yDis](Images/30y_Stats.PNG)<br/>
  10y:<br/>
  ![10yDis](Images/10y_Stats.PNG)
  <br/>

Those statistics will help to detemine the optimal allocation mix and investement horizon of the fund holders.

> Getting started<br/>

- To use the Financial Planner application first clone the repository to your PC. The repository comes with **financial_planning_tools.ipynb** application and `MCForecastTools.py` needed to run the application <br/>
- Open `Jupyter lab` as per the instructions in the [Installation Guide](#installation-guide) to run the application.<br/>

  At the very end of the application you can find a summary and conclusion drawn based on the simulation results. It can serve as a sample for your analysis.

---

## Contributors

Contact Details:

Boris Dudkin:

- [Email](boris.dudkin@gmail.com)
- [LinkedIn](www.linkedin.com/in/Boris-Dudkin)

---

## License

MIT
