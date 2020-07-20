# Useful Modules
<pre>
List of useful modules for python and R

Data & IO:
csvkit – Library for working with csv files
Openpyxl – for working with excel files
JmesPath – declarative access to json elements
pprint – pretty print
chardet – for detecting character set for a file
configparser - for working with ini files
PyYaml - for working with yaml files
python-dotenv - Reads the key-value pair from .env file and adds them to environment variable. It is great for managing app settings during development and in production using 12-factor principles
Dataprep - lets you prepare your data using a single library with a few lines of code

PDFs:
ReportLab - for creating PDFs programmatically
Pypdf2 – for working with pdf’s
Py PDF Parser - Visualize and extract structured data from PDF files
pdfminer - for mining pdf files
Camelot - Extract tables from text based PDF files

Data Analytics:
table - fast and lightweight alternative to pandas also feature limited
pytables - Data storage for df from within pandas
pystore - Data storage for df from within pandas
Pickle / cpickle - for serializing objects for storage
  Shelve – higher level for pickle
Dplython - dyplr R equivalent for summarizing
missingno - Missing data visualisation in pandas
sidetable - Create Simple Summary Tables in Pandas

Pandas Alternatives:
StaticFrame - a consistent interface for working with datafames alternative to pandas
RAPIDS - drop in replacement library for pandas to speed up data science analysis optimised CUDA (Nvidia)

Plotting Meta Package:
Holoviz - High-level tools to simplify visualization in Python

https://pyviz.org/tools

Plotting:
Mathplotlib - plting library
  Seaborn - Higher level interface for mathplotlib
  Dexplot - simple and intuitive user experience for mathplotlib
bqplot - interactive 2-D visualization system for Jupyter, based on the constructs of the Grammar of Graphics
Plotnine – ggplot2 inspired plotting library
Altair - Vega based Plotly alternative
gleam - interactive web visualisations
Pygal - SVG Plots
Plotly - Web plots
Ggplot – based on R ggplot
pyecharts - echarts libary for python
Pandas-Bokeh - Bokeh plotting backend for Pandas, GeoPandas and Pyspark DataFrames

Dashboards:
Dash - based on Plotly
PyViz, Bokeh, Bowtie
Panel - built on top of bokeh can be  shared without jupyter

Spatial / mapping:
geoplotlib - visualizing geographical data and making maps
Cartopy -  geospatial data processing in order to produce maps and other geospatial data analyses
pyshp - reading shape files
Fiona - Fast reading of shp files
Geopandas - High level library using numpy, pandas, cartopy, fiona etc to make maps
Basemap - mpl_toolkits submodule for plotting on maps

Web Scraping:
BeautifulSoup – html parser
Scrapy – creating web crawlers
Requests - frontend for urllib3

Text Extraction:
textract - Text extraction from variety of document and images
texthero - Text preprocessing, representation and visualization
Flashtext – Fast full word replacement
Emoji – Unicode emoji conversion

NLP:
NLTK - Oldest NLP
SpaCy - New NLP
Gensim - robust semantic analysis, topic modeling and vector-space modelling
nlp - lightweight and extensible library to easily share and access datasets and evaluation metrics for Natural Language Processing (NLP) based on tensorflow dataset tfds

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

Task Queue:
Celery - Task queues used as a mechanism to distribute work across threads or machines
Joblib - set of tools to provide lightweight pipelining in Python, transparent disk caching and parellel computing
Dramatiq is a background task processing library for Python with a focus on simplicity, reliability and performance
appscheduler - python scheduler for apps
python-advanced-scheduler


Machine Learning:
mlfinlab - machine learing for finance
scikit-learn - algorithms of machine learning and data mining tasks
XGBoost/LightGBM - optimised, scalable and fast implementations of gradient
shogun - machine learning toolbox written in C++ available for multiple languages
Hummingbird - compile trained traditional ML models into tensor computations PyTorch
Libra - automates the end-to-end machine learning process in just one line of code. It is built for both non-technical users and software professionals of all kinds.
LazyPredict - help build a lot of basic models without much code and helps understand which models works better without any parameter tuning

Deep Learning:
keras - makes deep learning easier to learn with a simpler api and clear error messages
  TensorFlow - Googles framework for deep learning / machine learning
PyTorch - Performs tensor computations with GPU acceleration, create dynamic computational graphs and automatically calculate gradients
fastai - simplified neural net training with best practices with out of the box support for many types of ML
H20 - AI library

Graphs:
NetworkX, igraph - Graph analysis
nxviz - Graph Visualiation
Pydot – graph plotting
  Graphviz – underlying for pydot

Stats:
Statsmodels – for statistical and unit tests
PyMC3 - statistical modeling tool for Bayesian statistical modeling & Probabilistic Machine Learning which focuses on advanced Markov chain Monte Carlo and variational fitting algorithms

Time Series:
darts - easy manipulation and forecasting of time series
sktime - machine learning toolbox for time series forecasting
PyFlux - time series model library for Python

Testing:
unittest – First unit testing framework of the std library
nose – Extends unit testing for other packages
doctest - test generation based on output from shell interpreter
pytest - easy to write small tests, yet scales to support complex functional testing for applications and libraries
hypothesis - property based tests creating unit tests which are simpler to write and more powerful when run, finding edge cases in your code you wouldn’t have thought to look for

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
Kivy - cross-platform framework for development of applications that make use of innovative, multi-touch user interfaces
Toga - Python native, OS native, cross platform GUI toolkit
atlas-python - Atlas toolkit is the easiest way to add a web-based graphical user interface
streamlit - create beautiful, performant apps in a few hours in pure Python

Console-GUI:
curses - used to create text user interface is restricted to Unix-like systems
WConio - is a wrapper for Turbo-C’s CONIO.H, used to create text user interfaces
Rich - for rendering rich text and beautiful formatting to the terminal
Colorama – colouring command-line text

Argument Parser:
cliche - Build a simple command-line interface from your functions using a decorator while keeping it usage for other scripts
argparse - it is powerful, but you need a lot of code to construct an argparse CLI
click -  you need a lot of decorators to construct a CLI, and not obvious how to use it
hug (cli) - connected to a whole web framework, but gets a lot right
python-fire - low set up, but annoying traces all the time / ugly design, does not show default values nor types
cleo - requires too much code/objects to construct

API:
tweepy - Twitter streaming API library
twitter-scraper - Twitter frontend (JavaScript) has it's own API, reverse–engineered. No API rate limits. No restrictions. Extremely fast
InstaPy – Instagram selenium bot
google-api-python-client - google api client
clarifai - computer vision AI platform 5k free calls/mo

Endpoint Frameworks:
Django - a framework for building a complex, data-driven websites;
djangorestframework - powerful and flexible toolkit for building Web APIs using REST
Flask - micro-web framework, that helps to build an APIs and supports unit testing;
CherryPy - minimalist, manipulable, light with lot of plugins
Bottle - lightweight and self contained micro framework with webserver and no additional dependencies
Web2py - light with no dependencies, fully-featured IDE, full stack, old fashioned
FastAPI - light and fast built on top of Starlette and Uvicorn
instant-api - Instantly create an HTTP API with automatic type conversions, JSON RPC, and a Swagger UI with all the boring stuff done for you
Tornado - also an asynchronous networking library allows for large and scaling solution
Quart - combination of asyncio and flask
Pyramid - scalable and OO
Falcon - minimalist web API framework which is very fast used for large scale encourages REST

Enferno - A Python framework based on Flask microframework, with batteries included, and best practices in mind.

WSGI servers
Gunicorn

ASGI server:
Uvicorn - ASGI server
Starlette - toolbox of higher-level components such as requests and responses that you can use to abstract away some of the details of ASGI

Time and date:
Datetime – working with date and time
python-dateutil - working with timezones
pytz - alternative to python-dateutil (has different interface compared to dateutil so dateutil is preferred)
dateparser - Natural language date parsing, supports multiple languages

Python Grammer:
collections – additional data types
itertools/functools - tools for using iterators and functions as functional progamming
toolz (itertoolz/functoolz/distoolz) - supplementary to above which implements some missing functionality

Linting, formatting, styling:
mypy - optional static type checker
typing - type hinting and annotations with modern IDE's
pycodestyle - formally called pep8
black - automatic code formatter following pep8 works well with pre-commit and poetry for CI
pylint - superset of flake8
  flake8 - check for errors and style wrapper on pyflakes ans few other tools
    pyflakes - A simple program which checks Python source files for error
Pytype - checks and infers types for your Python code - without requiring type annotations also support cross function inference which is not available with mypy and also allows runtime lenience compared to mypy(windows support pending) (Google)
pyre - static type checker (Facebook)
pyright - static type checker (Microsoft)
isort an automatic import formatter
	seed-isort-config a tool to statically populate the known_third_party part of the .isort.cfg
Bandit is a tool designed to find common security issues in Python code

Dynamic Type Checkers:
enforce
typeguard
typo
ducktype
strictconf

Python debugging and profiling:
cProfile - profiler part of stdlib
line_profiler - profile the time each individual line takes to execute
memory_profiler - monitoring memory consumption in a process or you can use it for a line-by-line analysis of the memory consumption
profilehooks - multiple profiling options
pycrunch-trace - debugging and time travel from pytrace.com

ORM:
Alembic - for database migration
SQLAlchemy: Most popular ORM for python
zodb - Python object-oriented database

Package Management:
virtualenvwrapper - wrapper for virtualenv tool
Poetry - simplifies dependeny management for python projects and packages

Utilities:
logging – logging library
pyperclip – clipboard access
re – regular expression
shutil – Shell utility function like file properties and manipulation
pathlib — Object-oriented filesystem paths
webbrowser - Convenient Web-browser controller
progress and tqdm – progress bars
reticulate - tools for interoperability between Python and R

Apps:
ChatterBot - ML based python chatbot
JSMon - JavaScript Change Monitor for BugBounty
pygooglenews - A python wrapper of the Google News RSS feed
Ciphey - automated decryption tool. Input encrypted text, get the decrypted text back
byob - Python based botnet
clearview.ai
ngrap - app tunneling https://ngrok.com/
jprq - ngrok alternative

Compilers:
pypy - python JIT compiler
Numexpr - extension library for scipy which can further speed up Numpy and Pandas

VSCode Extenstions:
Python
Pylance
Indenticator
Bracket Pair Colorizer 2/3
Dash

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
</pre>
