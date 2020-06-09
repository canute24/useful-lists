# useful-modules
List of useful modules for python and R

Data & IO:
csvkit – Library for working with csv files
Pypdf2 – for working with pdf’s
Py PDF Parser - Visualize and extract structured data from PDF files
Textract - Text extraction from variety of document and images
Camelot - Extract tables from text based PDF files
Openpyxl – for working with excel files
JmesPath – declarative access to json elements
Pprint – pretty print
Chardet – for detecting character set for a file
pathlib — Object-oriented filesystem paths

Data Analytics:
table - fast and lightweight alternative to pandas also feature limited
pytables - Data storage for df from within pandas
pystore - Data storage for df from within pandas
Pickle / cpickle - for serializing objects for storage
  Shelve – higher level for pickle
Dplython - dyplr R equivalent for summarizing
missingno - Missing data visualisation in pandas
sidetable - Create Simple Summary Tables in Pandas

Plotting:
Mathplotlib - plting library
   Seaborn - Higher level interface for mathplotlib
Bqplot – 2D plotting library for Jupyter notebook
Plotnine – ggplot2 inspired plotting library
Altair - Vega based Plotly alternative
gleam - interactive web visualisations
Pygal - SVG Plots
Plotly - Web plots
Ggplot –based on R ggplot
Dash, PyViz, Bokeh and Bowtie – Dashboards
Holoviz = High-level tools to simplify visualization in Python

Spatial / mapping:
geoplotlib - visualizing geographical data and making maps
Cartopy -  geospatial data processing in order to produce maps and other geospatial data analyses
pyshp - reading shape files
Fiona - Fast reading of shp files
Geopandas - High level library using numpy, pandas, cartopy, fiona etc to make maps

Web Scraping:
BeautifulSoup – html parser
Scrapy – creating web crawlers
Requests - frontend for urllib3

Text:
NLTK - Oldest NLP
SpaCy - New NLP
Flashtext – Fast full word replacement
Gensim - robust semantic analysis, topic modeling and vector-space modelling
Emoji – Unicode emoji conversion

Spatial:
Geopy - client for several popular geocoding web services

Finance:
yahooquery - Yahoo finance API unofficial
talib - Technical Analysis
Backtrader – Backtesting
Zipline – Backtesting
Pyfolio – To check portfolio perf metrics
Nsepy
Mibian - Options Pricing

AI:
Scikit - Machine Learning
shogun - machine learning toolbox written in C++ available for multiple languages
NetworkX, igraph - Graph analysis
nxviz - Graph Visualiation
Pydot – graph plotting
  Graphviz – underlying for pydot

ML Platforms:
H2O
Keras
  Tensorflow
clarifai - computer vision AI platform 5k free calls/mo

Stats:
Statsmodels – for statistical and unit tests
PyFlux - time series model library for Python

Testing:
UnitTest – First unit testing framework of the std library
Nose – Extends unit testing for other packages
DocTest - test generation based on output from shell interpreter
Pytest – to write small tests when supporting complex functional testing

Image Processing:
Pytesseract - Tesarract 4 python bindings
Pillow – python version of PIL, for working with images
imutils
OpenCV-Python – Open computer vision library

Audio Processing:
SpeechRecognition - Library for performing speech recognition, with support for several engines and APIs, online and offline

WebApps:
Django – for larger projects and handles most of the details
Flask – for smaller projects where you can control most of the details

Email:
email - For managing email messages. With this we will setup the email message itself, including subject, body, and attachments.
smtplib - Handles the SMTP connection

Workflow Automation:
Airflow – from Airbnb
Luigi – from Spotify

RPA:
Rpa – RPA package for python
Pyautogui – GUI automation
Selenium – Browser automation

GUI:
PySimpleGUI – Simple python GUI framework

Non-GUI:
curses - used to create text user interface is restricted to Unix-like systems
WConio - is a wrapper for Turbo-C’s CONIO.H, used to create text user interfaces
Rich - for rendering rich text and beautiful formatting to the terminal
Colorama – colouring command-line text

API:
twitter-scraper - Twitter frontend (JavaScript) has it's own API, reverse–engineered. No API rate limits. No restrictions. Extremely fast
InstaPy – Instagram selenium bot

Time and date:
Datetime – working with date and time
python-dateutil - working with timezones
pytz - alternative to python-dateutil (has different interface compared to dateutil so dateutil is preferred)
dateparser - Natural language date parsing, supports multiple languages

Python Grammer:
mypy - optional static type checker
Collections – additional data types

Python debugging and profiling:
cProfile - profiler part of stdlib
line_profiler - profile the time each individual line takes to execute
memory_profiler - monitoring memory consumption in a process or you can use it for a line-by-line analysis of the memory consumption
profilehooks - multiple profiling options
pycrunch-trace - debugging and time travel from pytrace.com

Utilities:
Logging – logging library
Pyperclip – clipboard access
Re – regular expression
Shutil – Shell utility function like file properties and manipulation
Webbrowser - Convenient Web-browser controller
progress and tqdm – progress bars

R:
reticulate - tools for interoperability between Python and R

http://pandas.pydata.org/pandas-docs/stable/10min.html
http://pandas.pydata.org/pandas-docs/stable/cookbook.html
https://github.com/jvns/pandas-cookbook
http://pandas.pydata.org/pandas-docs/stable/missing_data.html
http://pandas.pydata.org/pandas-docs/stable/groupby.html
http://pandas.pydata.org/pandas-docs/stable/reshaping.html
http://pandas.pydata.org/pandas-docs/stable/merging.html
http://pandas.pydata.org/pandas-docs/stable/io.html
http://pandas.pydata.org/pandas-docs/stable/text.html
http://pandas.pydata.org/pandas-docs/stable/visualization.html
http://pandas.pydata.org/pandas-docs/stable/timeseries.html
http://pandas.pydata.org/pandas-docs/stable/timedeltas.html
http://pandas.pydata.org/pandas-docs/stable/categorical.html
http://pandas.pydata.org/pandas-docs/stable/computation.html
http://pandas.pydata.org/pandas-docs/stable/advanced.html

R:
Tidyverse - Collection R modules for data science
ggplot2 - Plotting library
Shiny - Webapp and web visualisations
Rmarkdown – Rmd notebook like ipython
Ggplot2 – for plotting
Lattice – for multivariate relationships

rCharts – for javascript charts
googleVis – for using Google charts for vis
ggvis – interactive grammer of graphics, when rendering in browser

pqR – New version of R interpreter
renjin, FastR – R writer in Java
Riposte – Fast interpreter and JIT for R
RevoScaleR – Commercial tool to handle big datasets
Foreach – Commercial tool for parallel programming

quantmod - development, testing, and deployment of statistically based trading models

---------------------
Exploratory analysis:
Split your data into complementary sets for training, validation (for parameter tuning, feature selection etc) and testing. This is actually more complex than it sounds: optimally, the test set should be as ‘similar’ as possible to the present ‘state of the market’, and both validation and test set should follow the same distribution. Otherwise you might waste effort tuning the model parameters on the validation set only to find that it poorly generalizes to the test set.

Following the concept of ‘market regimes’?—?ie extended periods where a specific combination of commodities dominates the price dynamics of your target instrument?—?it might be worthwhile to first have a clustering algorithm of unsupervised learning discover defining correlations in the data and then evaluate model performance on data in the validation and test set belonging to the same clusters (see Figure 3?—?in this project, clustering increased predictive performance by 8%).

Data Transformations:
Moving averages can provide historical context and trends when your choice of learning algorithm does not have explicit memory cells like Recurrent Neural Networks or LSTMs.
Using data or derived inputs such as indicators/indices which may be less accurate than the data you have may have some use specially if other participants can influence the output you are trying to model in which case they indicators/indices can provide inputs about how other participants will behave.

Model Validation:
Genetic algorithms allow you to explore the policy space, starting from a first generation of say 100 randomly chosen policy parameters, iteratively eliminating the 80 worst performers and making the 20 survivors produce 4 offspring each. Or you can employ a grid search in the multidimensional parameter space: starting from some plausible values for the parameters of the policy, what is the best-performing setting you can achieve by varying the parameter values one-by-one.

A good measure to prevent overfitting the parameters to the validation set is a cross-validation with a ‘walk-forward-test’ (WTF) verifying the robustness of your approach: optimize the policy parameters on a validation segment, test them forward in time on data following the validation segment, shift the validation segment forward to include that test data, repeat. The basic assumption here is that the recent past is a better gauge for the future than the more distant past.

Optimisation:
Exploring the space of policy parameters in this framework is done via inefficient numerical optimisation, not with the powerful gradient optimization of your predictive Machine Learning model.
https://towardsdatascience.com/https-medium-com-skuttruf-machine-learning-in-finance-algorithmic-trading-on-energy-markets-cb68f7471475
