# Pandas 生态

Increasingly, packages are being built on top of Pandas to address specific needs in data preparation, analysis and visualization. This is encouraging because it means Pandas is not only helping users to handle their data tasks but also that it provides a better starting point for developers to build powerful and more focused data tools. The creation of libraries that complement Pandas’ functionality also allows Pandas development to remain focused around it’s original requirements.

This is an inexhaustive list of projects that build on Pandas in order to provide tools in the PyData space. For a list of projects that depend on Pandas, see the [libraries.io usage page for Pandas](https://libraries.io/pypi/Pandas/usage) or [search pypi for Pandas](https://pypi.org/search/?q=Pandas).

We’d like to make it easier for users to find these projects, if you know of other substantial projects that you feel should be on this list, please let us know.

## Statistics and Machine Learning

### [Statsmodels](https://www.statsmodels.org/)

Statsmodels is the prominent Python “statistics and econometrics library” and it has a long-standing special relationship with Pandas. Statsmodels provides powerful statistics, econometrics, analysis and modeling functionality that is out of Pandas’ scope. Statsmodels leverages Pandas objects as the underlying data container for computation.

### [sklearn-Pandas](https://github.com/paulgb/sklearn-Pandas)

Use Pandas DataFrames in your [scikit-learn](https://scikit-learn.org/) ML pipeline.

### [Featuretools](https://github.com/featuretools/featuretools/)

Featuretools is a Python library for automated feature engineering built on top of Pandas. It excels at transforming temporal and relational datasets into feature matrices for machine learning using reusable feature engineering “primitives”. Users can contribute their own primitives in Python and share them with the rest of the community.

## Visualization

### [Altair](https://altair-viz.github.io/)

Altair is a declarative statistical visualization library for Python. With Altair, you can spend more time understanding your data and its meaning. Altair’s API is simple, friendly and consistent and built on top of the powerful Vega-Lite JSON specification. This elegant simplicity produces beautiful and effective visualizations with a minimal amount of code. Altair works with Pandas DataFrames.

### [Bokeh](https://bokeh.pydata.org/)

Bokeh is a Python interactive visualization library for large datasets that natively uses the latest web technologies. Its goal is to provide elegant, concise construction of novel graphics in the style of Protovis/D3, while delivering high-performance interactivity over large data to thin clients.

### [seaborn](https://seaborn.pydata.org/)

Seaborn is a Python visualization library based on matplotlib. It provides a high-level, dataset-oriented interface for creating attractive statistical graphics. The plotting functions in seaborn understand Pandas objects and leverage Pandas grouping operations internally to support concise specification of complex visualizations. Seaborn also goes beyond matplotlib and Pandas with the option to perform statistical estimation while plotting, aggregating across observations and visualizing the fit of statistical models to emphasize patterns in a dataset.

### [yhat/ggpy](https://github.com/yhat/ggpy)

Hadley Wickham’s ggplot2 is a foundational exploratory visualization package for the R language. Based on “The Grammar of Graphics” it provides a powerful, declarative and extremely general way to generate bespoke plots of any kind of data. It’s really quite incredible. Various implementations to other languages are available, but a faithful implementation for Python users has long been missing. Although still young (as of Jan-2014), the yhat/ggpy project has been progressing quickly in that direction.

### [IPython Vega](https://github.com/vega/ipyvega)

[IPython Vega](https://github.com/vega/ipyvega) leverages [Vega](https://github.com/trifacta/vega) to create plots within Jupyter Notebook.

### [Plotly](https://plot.ly/python)

Plotly’s Python API enables interactive figures and web shareability. Maps, 2D, 3D, and live-streaming graphs are rendered with WebGL and D3.js. The library supports plotting directly from a Pandas DataFrame and cloud-based collaboration. Users of matplotlib, ggplot for Python, and Seaborn can convert figures into interactive web-based plots. Plots can be drawn in IPython Notebooks , edited with R or MATLAB, modified in a GUI, or embedded in apps and dashboards. Plotly is free for unlimited sharing, and has cloud, offline, or on-premise accounts for private use.

### [QtPandas](https://github.com/draperjames/qtPandas)

Spun off from the main Pandas library, the qtPandas library enables DataFrame visualization and manipulation in PyQt4 and PySide applications.

## IDE

### [IPython](https://ipython.org/documentation.html)

IPython is an interactive command shell and distributed computing environment. IPython tab completion works with Pandas methods and also attributes like DataFrame columns.

### [Jupyter Notebook / Jupyter Lab](https://jupyter.org/)

Jupyter Notebook is a web application for creating Jupyter notebooks. A Jupyter notebook is a JSON document containing an ordered list of input/output cells which can contain code, text, mathematics, plots and rich media. Jupyter notebooks can be converted to a number of open standard output formats (HTML, HTML presentation slides, LaTeX, PDF, ReStructuredText, Markdown, Python) through ‘Download As’ in the web interface and jupyter convert in a shell.

Pandas DataFrames implement _repr_html_``and ``_repr_latex methods which are utilized by Jupyter Notebook for displaying (abbreviated) HTML or LaTeX tables. LaTeX output is properly escaped. (Note: HTML tables may or may not be compatible with non-HTML Jupyter output formats.)

See Options and Settings and Available Options for Pandas display. settings.

### [quantopian/qgrid](https://github.com/quantopian/qgrid)

qgrid is “an interactive grid for sorting and filtering DataFrames in IPython Notebook” built with SlickGrid.

### [Spyder](https://www.spyder-ide.org/)

Spyder is a cross-platform PyQt-based IDE combining the editing, analysis, debugging and profiling functionality of a software development tool with the data exploration, interactive execution, deep inspection and rich visualization capabilities of a scientific environment like MATLAB or Rstudio.

Its [Variable Explorer](https://docs.spyder-ide.org/variableexplorer.html) allows users to view, manipulate and edit Pandas Index, Series, and DataFrame objects like a “spreadsheet”, including copying and modifying values, sorting, displaying a “heatmap”, converting data types and more. Pandas objects can also be renamed, duplicated, new columns added, copyed/pasted to/from the clipboard (as TSV), and saved/loaded to/from a file. Spyder can also import data from a variety of plain text and binary files or the clipboard into a new Pandas DataFrame via a sophisticated import wizard.

Most Pandas classes, methods and data attributes can be autocompleted in Spyder’s Editor and IPython Console, and Spyder’s Help pane can retrieve and render Numpydoc documentation on Pandas objects in rich text with Sphinx both automatically and on-demand.

## API

### [Pandas-datareader](https://github.com/pydata/Pandas-datareader)

Pandas-datareader is a remote data access library for Pandas (PyPI:Pandas-datareader). It is based on functionality that was located in Pandas.io.data and Pandas.io.wb but was split off in v0.19. See more in the [Pandas-datareader docs](https://Pandas-datareader.readthedocs.io/en/latest/):

The following data feeds are available:

- Google Finance
- Tiingo
- Morningstar
- IEX
- Robinhood
- Enigma
- Quandl
- FRED
- Fama/French
- World Bank
- OECD
- Eurostat
- TSP Fund Data
- Nasdaq Trader Symbol Definitions
- Stooq Index Data
- MOEX Data

### [quandl/Python](https://github.com/quandl/Python)

Quandl API for Python wraps the Quandl REST API to return Pandas DataFrames with timeseries indexes.

### [pydatastream](https://github.com/vfilimonov/pydatastream)

PyDatastream is a Python interface to the [Thomson Dataworks Enterprise (DWE/Datastream)](http://dataworks.thomson.com/Dataworks/Enterprise/1.0/) SOAP API to return indexed Pandas DataFrames or Panels with financial data. This package requires valid credentials for this API (non free).

### pandaSDMX(https://Pandasdmx.readthedocs.io/)

pandaSDMX is a library to retrieve and acquire statistical data and metadata disseminated in [SDMX](https://www.sdmx.org/) 2.1, an ISO-standard widely used by institutions such as statistics offices, central banks, and international organisations. pandaSDMX can expose datasets and related structural metadata including data flows, code-lists, and data structure definitions as Pandas Series or MultiIndexed DataFrames.

### [fredapi](https://github.com/mortada/fredapi)

fredapi is a Python interface to the [Federal Reserve Economic Data (FRED)](https://fred.stlouisfed.org/) provided by the Federal Reserve Bank of St. Louis. It works with both the FRED database and ALFRED database that contains point-in-time data (i.e. historic data revisions). fredapi provides a wrapper in Python to the FRED HTTP API, and also provides several convenient methods for parsing and analyzing point-in-time data from ALFRED. fredapi makes use of Pandas and returns data in a Series or DataFrame. This module requires a FRED API key that you can obtain for free on the FRED website.

## Domain Specific

### [GeoPandas](https://github.com/kjordahl/geoPandas)

GeoPandas extends Pandas data objects to include geographic information which support geometric operations. If your work entails maps and geographical coordinates, and you love Pandas, you should take a close look at GeoPandas.

### [xarray](https://github.com/pydata/xarray)

xarray brings the labeled data power of Pandas to the physical sciences by providing N-dimensional variants of the core Pandas data structures. It aims to provide a Pandas-like and Pandas-compatible toolkit for analytics on multi- dimensional arrays, rather than the tabular data for which Pandas excels.

Out-of-core

### [Blaze](http://blaze.pydata.org/)

Blaze provides a standard API for doing computations with various in-memory and on-disk backends: NumPy, Pandas, SQLAlchemy, MongoDB, PyTables, PySpark.

### [Dask](https://dask.readthedocs.io/en/latest/)

Dask is a flexible parallel computing library for analytics. Dask provides a familiar DataFrame interface for out-of-core, parallel and distributed computing.

### [Dask-ML](https://dask-ml.readthedocs.io/en/latest/)

Dask-ML enables parallel and distributed machine learning using Dask alongside existing machine learning libraries like Scikit-Learn, XGBoost, and TensorFlow.

### [Odo](http://odo.pydata.org/)

Odo provides a uniform API for moving data between different formats. It uses Pandas own read_csv for CSV IO and leverages many existing packages such as PyTables, h5py, and pymongo to move data between non Pandas formats. Its graph based approach is also extensible by end users for custom formats that may be too specific for the core of odo.

### [Ray](https://ray.readthedocs.io/en/latest/Pandas_on_ray.html)

Pandas on Ray is an early stage DataFrame library that wraps Pandas and transparently distributes the data and computation. The user does not need to know how many cores their system has, nor do they need to specify how to distribute the data. In fact, users can continue using their previous Pandas notebooks while experiencing a considerable speedup from Pandas on Ray, even on a single machine. Only a modification of the import statement is needed, as we demonstrate below. Once you’ve changed your import statement, you’re ready to use Pandas on Ray just like you would Pandas.

```python
# import Pandas as pd
import ray.dataframe as pd
```

### [Vaex](https://docs.vaex.io/)

Increasingly, packages are being built on top of Pandas to address specific needs in data preparation, analysis and visualization. Vaex is a python library for Out-of-Core DataFrames (similar to Pandas), to visualize and explore big tabular datasets. It can calculate statistics such as mean, sum, count, standard deviation etc, on an N-dimensional grid up to a billion (109) objects/rows per second. Visualization is done using histograms, density plots and 3d volume rendering, allowing interactive exploration of big data. Vaex uses memory mapping, zero memory copy policy and lazy computations for best performance (no memory wasted).

- vaex.from_Pandas
- vaex.to_Pandas_df

## Data validation

### Engarde

Engarde is a lightweight library used to explicitly state your assumptions about your datasets and check that they’re actually true.

## Extension Data Types

Pandas provides an interface for defining [extension types](https://Pandas.pydata.org/Pandas-docs/stable/development/extending.html#extending-extension-types) to extend NumPy’s type system. The following libraries implement that interface to provide types not found in NumPy or Pandas, which work well with Pandas’ data containers.

### [cyberPandas](https://cyberPandas.readthedocs.io/en/latest)

CyberPandas provides an extension type for storing arrays of IP Addresses. These arrays can be stored inside Pandas’ Series and DataFrame.

## Accessors

A directory of projects providing [extension accessors](https://Pandas.pydata.org/Pandas-docs/stable/development/extending.html#extending-register-accessors). This is for users to discover new accessors and for library authors to coordinate on the namespace.

Library | Accessor | Classes
---|---|---
[cyberPandas](https://cyberPandas.readthedocs.io/en/latest) | ip | Series
[pdvega](https://jakevdp.github.io/pdvega/) | vgplot | Series, DataFrame