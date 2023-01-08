# Real Estate Analyser

### Real Estate Analyser proides investors with data visualization techniques, including aggregation, interactive visualizations, and geospatial analysis, to find properties that are viable investment opportunities in the San Francisco market. This tool can be used to explore and detect potential real estate investment opportunities in any other locations too.

---

![RealEstate](Images/rental.jpg)

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

2. PyViz is a Python visualization package that provides a single platform for accessing multiple visualization libraries. Two of these libraries are hvPlot and GeoViews.<br/> The [hvPlot ](https://hvplot.holoviz.org/) and [GeoViews ](https://geoviews.org/) libraries are visualization libraries that are designed to work with Pandas DataFrames and that we can use to create interactive plots for our data.

- [PyViz ](https://pyviz.org/) - For guidance on how to start visualization, interactive visualization, styles and layouts customazation.

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

To install PyViz, in Terminal run:

```python
# conda
conda install -c pyviz hvplot geoviews
```

Confirm the installation of all the PyViz packages by running the following commands in Terminal type:

```python
 conda list hvplot
 conda list geoviews
```

---

## Usage

> Application summary<br/>

Real Estate Analyser assists proptech companies with vizualisation techniques to assess the availability of "buy-and-rent" properties in the selected locations (in our example San Francisco and its neighborhoods) by:

1. Analysing the trends in housing units over a selected time period in the selected location:<br/>
   ![Housing_Units](Images/zoomed-housing-units-by-year.png)<br/>

2. Plotting and analysing the gross rent and sale price per square foot over the selected time period in the location of interest:<br/>
   ![Rent_Sale](Images/avg-sale-px-sq-foot-gross-rent.png)<br/>
   and further exploring the average sale price per square foot and rental income by neighborhood.:<br/>
   ![Rent_Sale_hood](Images/pricing-info-by-neighborhood.png)<br/>
3. Building an interactive neighborhood map and exploring the geospatial relationships in the data by using interactive visualizations with hvPlot and GeoViews. :<br/>
   ![Rent_Sale_interactive](Images/6-4-geoviews-plot.png)<br/>

> Getting started<br/>

- To use the Real Estate Analyser first clone the repository to your PC.<br/>
- Open `Jupyter lab` as per the instructions in the [Installation Guide](#installation-guide) to run the application.<br/>

  At the very end of the application you can find a summary and conclusion drawn based on the generated vizualisations. It can serve as a sample for your analysis.

---

## Contributors

Contact Details:

Boris Dudkin:

- [Email](boris.dudkin@gmail.com)
- [LinkedIn](www.linkedin.com/in/Boris-Dudkin)

---

## License

MIT

---
