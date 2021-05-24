# Useful Python Modules

Module lists:
- https://github.com/vinta/awesome-python/
- https://github.com/ml-tooling/best-of-web-python

Cheatsheets:
- https://devhints.io/

API List:
- https://public-apis.io/

Data & IO:
- csvkit: Library for working with csv files
- json-traverse: simple JSON parser
- JmesPath: declarative access to json elements
- xml.etree.ElementTree - parse XML files
- chardet: for detecting character set for a file
- docx2txt: extract text from MSWord docx format
- catdoc: extract text from MSWord doc format
- Pickle / cpickle: for serializing objects for storage
    - Shelve – higher level for pickle
- Tablib: format agonistic tabular dataset library supporting json, csv, xls, yaml etc
- dvc: Data version control. Git for data.

Configuration Management:
- configparser: for working with ini files
- python-dotenv: Reads the key-value pair from .env file and adds them to environment variable. It is great for managing app settings during development and in production using 12-factor principles
- Dynaconf: can read most config formats
- Hydra: dynamically create hierarchial config and overide with command line options and save each session into a custom config

Excel files:
- Openpyxl: for working with excel files
- XlsxWriter: module for creating Excel XLSX files
- xlrd: For reading older Excel (.xls) documents
- xlwt: For writing older Excel (.xls) documents
- formulas: interpreter for parsing and calculating excel formulae
- xlwings: Works with new Excel formats and has macro capabilities but depends on excel
- PyXLL: use python instead of macros in excel making python accessible from excel

PDFs:
- pText: pure python pdf manipulation as a JSON like structure support read and editing
- fpdf2: minimalist PDF creation library successor to PyFPDF
- Pypdf2: for working with pdf’s
- ReportLab: for creating PDFs programmatically
- PDFx: extract data, links and metadata from pdfs as CLI or library
- PyPDFParser: Visualize and extract structured data from PDF files
- pdfminer: for mining pdf files
- Camelot: Extract tables from text based PDF files

Data Pipeline:
- Dataprep: lets you prepare your data using a single library with a few lines of code

Workflow Automation / ETL pipeline:
- Luigi: from Spotify
- Airflow: from Airbnb
- Dagster: data orchestrator for machine learning, analytics, and ETL

Build Automation / CI/CD:
- invoke: task execution tool and libary similar to make
- tox: task automation tool which can make venvs to run builds, tests, docs, publishing etc a complete CI/CD workflow which can also execute make commands

Data Analytics:
- pytables: Data storage for df from within pandas
- pystore: Data storage for df from within pandas
- Dplython: dyplr R equivalent for summarizing
- missingno: Missing data visualisation in pandas

Project Folder Structure Skeleton:
- cookiecutter / ccds: folder structure for datascience

REPL:
- jupyter-console: ipython like REPL for other kernels like C and Java
- bpython: python repl with undo, autoformatting, autocomplete, highlighting in terminal

Jupyter and notebook:
- nblint: pylint for notebooks
- nbdime: provides tools for diffing and merging of Jupyter Notebooks
    - nbdiff: compare notebooks in a terminal-friendly way
    - nbmerge: three-way merge of notebooks with automatic conflict resolution
    - nbdiff-we:b shows you a rich rendered diff of notebooks
    - nbmerge-web: gives you a web-based three-way merge tool for notebooks
    - nbshow: present a single notebook in a terminal-friendly way
- nbterm: simple notebook for terminal
- nbstripout: strip output from Jupyter and IPython notebooks
- nbconvert: Convert Notebooks to other formats pdf, static presentations (installed with jupyter)
- jupytext: code is saved in a specified format (py, md, Rst etc.) and converted to ipynb on load
- nbdev: allows you to develop a python library in Jupyter Notebooks with features such as debugging, refactoring, writing tests, create docs, publish packages etc.
- ipywidgets: adds interactivity to jupyter notebooks
- papermill: parametrizing jupyter notebooks so the notebook can be run for different values and also build workflow based on results of the notebook
- rise: reveal.js based presentation for live notebooks
- voila: GUI's from jupyter notebook based on ipywidgets
- bqplot: interactive 2-D visualization system for Jupyter, based on the constructs of the Grammar of Graphics

EDA libraries:
- Flenser: simple automated data exploration tool that runs tests on dataset and provides summary
- data-describe: toolkit for Exploratory Data Analysis (EDA). It aims to accelerate data exploration and analysis by providing automated and opinionated analysis widgets
- lux: API for Intelligent Visual Data Discovery
- pandas-profiling: EDA support for pandas dataframe

Pandas Alternatives:
- datatable: h2oai's table based on extremely fast data.table from R
- StaticFrame: a consistent interface for working with datafames alternative to pandas
- RAPIDS: drop in replacement library for pandas to speed up data science analysis optimised CUDA (Nvidia) - better than pandas with GPU
- Dask: better with parallel task, slower will non parallel
- Modin: Drop in replacement for pandas to speed up common timeconsuming task by parellelising code

Pandas:
- Quickstart:
    - http://pandas.pydata.org/pandas-docs/stable/10min.html
    - http://pandas.pydata.org/pandas-docs/stable/cookbook.html
    - https://github.com/jvns/pandas-cookbook
- bamboolib: GUI for pandas df
- pandas-gui: GUI for pandas df
- sidetable: Create Simple Summary Tables in Pandas

Plotting Meta Package:
- Holoviz: High-level tools to simplify visualization in Python

Plotting:
https://pyviz.org/tools
- Mathplotlib: plting library
    - Seaborn - Higher level interface for mathplotlib
    - Dexplot - simple and intuitive user experience for mathplotlib
- bqplot: interactive 2-D visualization system for Jupyter, based on the constructs of the Grammar of Graphics
- Plotnine: ggplot2 inspired plotting library
- Altair: Vega based Plotly alternative
- gleam: interactive web visualisations
- Pygal: SVG Plots
- Plotly: Web plots
- Ggplot: based on R ggplot
- pyecharts: echarts libary for python
- Pandas-Bokeh: Bokeh plotting backend for Pandas, GeoPandas and Pyspark DataFrames

Dashboards:
- Dash: based on Plotly
- PyViz, Bokeh, Bowtie
- Panel: built on top of bokeh

Spatial / Geography / Mapping:
- pyrosm: parsing OpenStreetMap data
- geoplotlib: visualizing geographical data and making maps
- cartopy: geospatial data processing in order to produce maps and other geospatial data analyses
- pyshp: reading shape files
- fiona: Fast reading of shp files
- geopandas: High level library using numpy, pandas, cartopy, fiona etc to make maps
- basemap: mpl_toolkits submodule for plotting on maps
- geopy: client for several popular geocoding web services
- Nominatim: API to search OSM data by name and address and to generate synthetic addresses of OSM points (reverse geocoding) without signup

Web Scraping:
- BeautifulSoup: html parser
- Scrapy: creating web crawlers
- Requests: frontend for
- playwright: puppeteer devs new project after moving to microsoft for browser control similar API as puppeteer runs on NodeJS backend
- pyppeteer: Headless chrome/chromium automation library (unofficial port of puppeteer)
- Elemental: makes Selenium automation faster and easier by adding automatic waits and common missing usecases from selenium
    - Selenium – Browser automation
- selenium-wire: give access to underlying requests made by the browser

Text Extraction:
- textract: Text extraction from variety of document and images
- texthero: Text preprocessing, representation and visualization
- Flashtext: Fast full word replacement
- Emoji: Unicode emoji conversion

NLP:
- NLTK: Oldest NLP
- SpaCy: New NLP
- Gensim: robust semantic analysis, topic modeling and vector-space modelling
- nlp: lightweight and extensible library to easily share and access datasets and evaluation metrics for Natural Language Processing (NLP) based on tensorflow dataset tfds

Finance:
- yahooquery: Yahoo finance API unofficial
- talib: Technical Analysis
- Backtrader: Backtesting
- pandas-ta: Technical Analysis Indicators - Pandas TA is an easy to usePandas Extension with 120+ Indicators
- backtesting.py
- Zipline: Backtesting
- Pyfolio: To check portfolio perf metrics
- Nsepy: API for nse including CLI depends on numpy and pandas
- Mibian: Options Pricing

Task Queue:
- Celery: Task queues used as a mechanism to distribute work across threads or machines
- Joblib: set of tools to provide lightweight pipelining in Python, transparent disk caching and parellel computing
- Dramatiq is a background task processing library for Python with a focus on simplicity, reliability and performance
- appscheduler: python scheduler for apps
- python-advanced-scheduler: very advanced scheduler
- sched: simple scheduler
- python-crontab: uses os specific scheduler in the background
- schedule: declarative scheduler similar to crontab, easier syntax

Machine Learning:
- mlfinlab: machine learning for finance
- scikit-learn: algorithms of machine learning and data mining tasks
- XGBoost/LightGBM - optimised, scalable and fast implementations of gradient
- shogun: machine learning toolbox written in C++ available for multiple languages
- Hummingbird: compile trained traditional ML models into tensor computations PyTorch
- Libra: automates the end-to-end machine learning process in just one line of code. It is built for both non-technical users and software professionals of all kinds.
- LazyPredict: help build a lot of basic models without much code and helps understand which models works better without any parameter tuning

Deep Learning:
- keras: makes deep learning easier to learn with a simpler api and clear error messages
    - TensorFlow - Googles framework for deep learning / machine learning
- PyTorch: Performs tensor computations with GPU acceleration, create dynamic computational graphs and automatically calculate gradients
- fastai: simplified neural net training with best practices with out of the box support for many types of ML
- H20: AI library

Graphs:
- NetworkX, igraph - Graph analysis
- nxviz: Graph Visualiation
- Pydot: graph plotting
    - Graphviz – underlying for pydot

Stats:
- Statsmodels: for statistical and unit tests
- PyMC3: statistical modeling tool for Bayesian statistical modeling & Probabilistic Machine Learning which focuses on advanced Markov chain Monte Carlo and variational fitting algorithms
- ppscore: Predictive Power Score (PPS) replacement for corelation to detect relationships using decision trees ML model from sklearn internally

Time Series:
- darts: easy manipulation and forecasting of time series
- sktime: machine learning toolbox for time series forecasting
- PyFlux: time series model library for Python
- dtw-python: Dynamic time warping to fit data two time series by finding minimum distance between the series

Testing:
- unittest: First unit testing framework of the std library
- nose: Extends unit testing for other packages
- doctest: test generation based on output from shell interpreter
- pytest: easy to write small tests, yet scales to support complex functional testing for applications and libraries
- pydantic: data parsing and validation using python type hints
- parameterized: parameterized tests compatible with pytest and unittest supports tests written as functions or methods
- hypothesis: property based tests creating unit tests which are simpler to write and more powerful when run, finding edge cases in your code you wouldn’t have thought to look for

Image Processing:
- Pytesseract: Tesarract 4 python bindings
- imageio: image manipulation library depends on numpy and pillow
    - pillow: maintained version of PIL, for working with images
- imutils: image maniputlation utilities
- OpenCV-Python: Open computer vision library

Audio Processing:
- SpeechRecognition: Library for performing speech recognition, with support for several engines and APIs, online and offline
- Picovoice: voice recognition library to add Alexa like feature to python apps

Email:
- email: For managing email messages. With this we will setup the email message itself, including subject, body, and attachments.
- smtplib: Handles the SMTP connection

RPA:
- pynput: Monitor and control input devices like KB and Mouse used for interceptors and keyloggers
- rpa: RPA package for python
- pyautogui: GUI automation

GUI:
- PyWebIO: simple web app interface generation in python script also can be made info a webapp
- pyrustic: framwwork for making GUI's uses tk
- PySimpleGUI: Simple python GUI framework
- re-wx: library for building modern declarative desktop applications in WX
- Kivy: cross-platform framework for development of applications that make use of innovative, multi-touch user interfaces
- Toga: Python native, OS native, cross platform GUI toolkit
- atlas-python: Atlas toolkit is the easiest way to add a web-based graphical user interface
- streamlit: create beautiful, performant apps in a few hours in pure Python
- voila: GUI's from jupyter notebook based on ipywidgets

Console-GUI:
- curses: used to create text user interface is restricted to Unix-like systems
- WConio: is a wrapper for Turbo-C’s CONIO.H, used to create text user interfaces
- WConio2: pure python implementation of WConio
- Rich: for rendering rich text and beautiful formatting to the terminal with rich text REPL
- Colorama: colouring command-line text
- tabulate: pretty print tabular data

Argument Parser:
- cliche: Build a simple command-line interface from your functions using a decorator while keeping it usage for other scripts
- argparse: it is powerful, but you need a lot of code to construct an argparse CLI
- click -    you need a lot of decorators to construct a CLI, and not obvious how to use it
- python-fire: low set up, but annoying traces all the time / ugly design, does not show default values nor types
- cleo: requires too much code/objects to construct
- python-fire: automatically generating command line interfaces (CLIs) from absolutely any Python object

API:
- tweepy: Twitter streaming API library
- twitter-scraper: Twitter frontend (JavaScript) has it's own API, reverse–engineered. No API rate limits. No restrictions. Extremely fast
- InstaPy: Instagram selenium bot
- google-api-python-client: google api client
- clarifai: computer vision AI platform 5k free calls/mo

Endpoint Frameworks:
- Brython: run python in place of javascript
- Django: a framework for building a complex, data-driven websites;
- djangorestframework: powerful and flexible toolkit for building Web APIs using REST
- Flask: micro-web framework, that helps to build an APIs and supports unit testing;
- CherryPy: minimalist, manipulable, light with lot of plugins
- Bottle: lightweight and self contained micro framework with webserver and no additional dependencies
- Web2py: light with no dependencies, fully-featured IDE, full stack, old fashioned
- FastAPI: light and fast built on top of Starlette and Uvicorn
- Tornado: also an asynchronous networking library allows for large and scaling solution
- Quart: combination of asyncio and flask
- Pyramid: scalable and OO
- Falcon: minimalist web API framework which is very fast used for large scale encourages REST
- Enferno: A Python framework based on Flask microframework, with batteries included, and best practices in mind
- instant-api: Instantly create an HTTP API with automatic type conversions, JSON RPC, and a Swagger UI with all the boring stuff done for you
- hug (cli): connected to a whole web framework, but gets a lot right

WSGI servers:
- Gunicorn

ASGI server:
- Uvicorn: ASGI server
- Starlette: toolbox of higher-level components such as requests and responses that you can use to abstract away some of the details of ASGI

Time and date:
- datetime: working with date and time
- python-dateutil: working with timezones
- pytz: alternative to python-dateutil (has different interface compared to dateutil so dateutil is preferred)
- dateparser: Natural language date parsing, supports multiple languages
- arrow: offers a sensible and human-friendly approach to creating, manipulating, formatting and converting dates, times and timestamps
- pendulum: improves API consistency over arrow

Python Grammer:
- collections: additional data types
- itertools/functools - tools for using iterators and functions as functional progamming
- toolz (itertoolz/functoolz/distoolz) - supplementary to above which implements some missing functionality

Performance:
- lru_cache: caching recent calculations
- cache: in functool (>=python3.9.2) same as above

Linting, formatting, styling:
- mypy: optional static type checker
- typing: type hinting and annotations with modern IDE's
- black: automatic code formatter following pep8 works well with pre-commit and poetry for CI
- autopep8: built on pycodestyle for autoformatting code
    - pycodestyle: formally called pep8
- pylint: superset of flake8
    - flake8 - check for errors and style wrapper on pyflakes and few other tools
        - pyflakes - A simple program which checks Python source files for error
- pytype: checks and infers types for your Python code - without requiring type annotations also support cross function inference which is not available with mypy and also allows runtime lenience compared to mypy(windows support pending) (Google)
- pyre: static type checker (Facebook)
- pyright: static type checker (Microsoft)
- isort an automatic import formatter
    - seed-isort-config: statically populate the known_third_party part of the .isort.cfg

Dynamic Type Checkers:
- enforce
- typeguard
- typo
- ducktype
- strictconf

Profiling:
- time python <script_name.py>
- python -m timeit -s <script_name.py>
- cProfile: profiler part of stdlib
- line_profiler: profile the time each individual line takes to execute
- memory_profiler: monitoring memory consumption in a process or you can use it for a line-by-line analysis of the memory consumption
- profilehooks: multiple profiling options
- pyinstrument: online profiler
- VizTracer: traces concurrent python programs and also helps in debugging

Refactoring:
- Bowler: refactoring tool for manipulating Python at the syntax tree level
- rope: refactoring library
- vulture: find dead/unused code
- bandit: find common security issues in Python code

Debugging:
- print statement: f"{hello=}" # >=python3.8
- sys.settrace and sys.setprofile
- pudb: text GUI debugger
- traceback_with_variables: Adds variables to python traceback, colouring or to file log
- frosch: Runtime Error Debugger with formatted like with variable list
- watchpoints: prints watched variables whenever its value changes and can even trigger pdb
- PySnooper: poor mans debugger, prints every variable change
- pycrunch-trace: debugging and time travel from pytrace.com
- jurigged: hotpatching code while script is being run when files is modified and saved
- pyrasite: Inject code into running Python processes
- Cyberbrain: Backtraces variable change, See every state of program execution, including variables' values

SQL / Databases:
- Alembic: for database migration
- SQLAlchemy: Most popular ORM for python
- zodb: Python object-oriented database
- piccolo: fast, user friendly ORM and query builder which supports asyncio
- preql: interpreted relational query language that complies python to sql written in python
- Vinum: use SQL on python datatypes in-memory for data analytics using Postgress's pglast parser
- DuckDB: run SQL queries on many data files including on pandas dataframes

Package Management:
- virtualenvwrapper: wrapper for virtualenv tool
- Poetry: simplifies dependeny management for python projects and packages

Android / Mobile phone:
- ppadb: pure python implementation of adb client which interfaces with the adb server on PC

Utilities:
- pprint: pretty print
- pint: Python units library
- faker: Fake data generator
- calender: generate calendars for any month
- logging: logging library
- pyperclip: clipboard access
- re: regular expression
- difflib: library for comparison and identify difference between patters with many helpful methods
- shutil: Shell utility function like file properties and manipulation
- pathlib: Object-oriented filesystem paths
- importlib: working with modules and package resource tool (install importlib_resouces py < 3.7)
- flit: tool to simplify package creation and publishing to PyPI
- webbrowser: Convenient Web-browser controller
- progress and tqdm – progress bars
- alive-progress: smart progress bar
- reticulate: tools for interoperability between Python and R
- Packet-Sniffer: pure-Python network packet sniffer based on PF_PACKET (Linux only)
- pytube: lightweight, dependency-free Python library (and command-line utility) for downloading YouTube Videos
    - youtube-dl: download vidoes from multple sites
- Python-Markdown: python implementation of John Grubers markdown
- manim - create animations with python scripts

HTML / Web page generation:
- Flatpages / Flask - markdown supported static website creation https://www.jamesharding.ca/posts/simple-static-markdown-blog-in-flask/
- Esparto: Create webpages to display data and outputs using bootstrap and jinja2
- jinja2: templating engine

Packaging:
- py2exe: create exe's for supported versions of python - doesn't require extraction
- Briefcase: tool for converting a Python project into a standalone native application
- pyoxidizer: similar to py2exe runs by extracting to memory but is a rust app requires rust to work
- pyinstaller: extracts to temp and runs, requires virtualenv

Apps:
- HTTPie: command-line HTTP client to make CLI interaction with web services as human-friendly as possible alternative to curl
- ChatterBot: ML based python chatbot
- JSMon: JavaScript Change Monitor for BugBounty
- pygooglenews: A python wrapper of the Google News RSS feed
- Ciphey: automated decryption tool. Input encrypted text, get the decrypted text back
- byob: Python based botnet
- clearview.ai
- ngrap: app tunneling https://ngrok.com/
- jprq: ngrok alternative

Compilers:
- pyston: JIT with upto 30% improvement on server benchmarks and more for simpler programs
- pyjion: JIT which convert code to native CIL and runs with .NET 5 CLR
- cinder: Instagram version of python JIT complier
- pypy: python JIT compiler
- Numexpr: extension library for scipy which can further speed up Numpy and Pandas
- numba: similar to numexpr
- nutika and shedskin: transpiler which convert to C++
