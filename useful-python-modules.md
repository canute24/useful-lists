https://developers.redhat.com/cheat-sheets/linux-commands-cheat-sheet
https://developers.redhat.com/cheat-sheets/advanced-linux-commands

# Useful Python Modules

As Python is finding use in many different applications and huge number of modules with a similar objective but different ideology / features are introduced, a list of propular / useful modules for quick reference helps a lot.

The main categorisation is between python apps in the traiditonal sense vs the more recent but rapidly growing data science ecosystem. While the common sections seperated out.

## Other Similar Collations

Module lists:
- https://github.com/vinta/awesome-python/
- https://github.com/ml-tooling/best-of-web-python
- https://github.com/florimondmanca/awesome-asgi

Cheatsheets:
- https://devhints.io/

## Input & Output / IO

System:
- sh: full-fledged subprocess replacement that allows you to call any program as if it were a function
- shutil: Shell utility function like file properties and manipulation
- pathlib: Object-oriented filesystem paths
- webbrowser: Convenient Web-browser controller
- pyperclip: clipboard access

Compatibility:
- win32api: Windows system calls
- reticulate: tools for interoperability between Python and R
- rpy/rpy2: calling R from python

Data Parsing / Conversion:
- stream_unzip: steam data from zip files instead of reading / loading the entire file
- difflib: library for comparison and identify difference between patterns with many helpful methods
- ujson: Extremely fast json library written in C
- json-traverse: simple JSON parser
- JmesPath: declarative access to json elements
- jsonpath-ng: traverse JSON elements in `.` (dot) notation (JSON notation) link in javascript
- jpath: access lists and dicts with `.` (dot) notation like JSON with wildcard, slicing and conditionals support
- xml.etree.ElementTree - parse XML files
- chardet: for detecting character set for a file
- python-markdown: python implementation of John Grubers markdown
- docx2txt: extract text from MSWord docx format
- catdoc: extract text from MSWord doc format
- Shelve: pickle wrapper
    - Pickle / cpickle: for serializing objects for storage
- fsspec: provides an abstract filesystem with a consistent API for file access

Data Pipeline:
- Dataprep: lets you prepare your data using a single library with a few lines of code

Workflow Automation / ETL pipeline:
- Luigi: from Spotify
- Airflow: from Airbnb
- Dagster: data orchestrator for machine learning, analytics, and ETL
- Orchest: visual orchestration tool for ETL, parametrisation with jupyterlab interface

Datafiles / CSV / TSV:
- tablib: format agonistic tabular dataset library supporting json, csv, xls, yaml etc
- csvkit: Library for working with csv files

SQL / Databases:
- Alembic: for database migration
- SQLAlchemy: Most popular ORM for python
- zodb: Python object-oriented database
- piccolo: fast, user friendly ORM and query builder which supports asyncio
- preql: interpreted relational query language that complies python to sql written in python
- Vinum: use SQL on python datatypes in-memory for data analytics using Postgress's pglast parser
- DuckDB: run SQL queries on many data files including on pandas dataframes
- SQLFluff: dialect-flexible and configurable SQL linter written in python

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

Web Scraping:
- BeautifulSoup: html parser
- Scrapy: creating web crawlers
- Requests: frontend for
- playwright: puppeteer devs new project after moving to microsoft for browser control similar API as puppeteer runs on NodeJS backend
- pyppeteer: Headless chrome/chromium automation library (unofficial port of puppeteer)
- Elemental: makes Selenium automation faster and easier by adding automatic waits and common missing usecases from selenium
    - Selenium – Browser automation
- selenium-wire: give access to underlying requests made by the browser

Text Processing:
- textract: Text extraction from variety of document and images
- texthero: Text preprocessing, representation and visualization
- Flashtext: Fast full word replacement
- Emoji: Unicode emoji conversion

Email:
- email: For managing email messages. With this we will setup the email message itself, including subject, body, and attachments.
- smtplib: Handles the SMTP connection
- IMAPlib: working with IMAP connections

Network / Communication:
- packet-sniffer: pure-Python network packet sniffer based on PF_PACKET (Linux only)
- httpx: next generation HTTP client for Python based on requests

### GUI / Interface

Indicators:
- progress / fastprogress / alive-progress / tqdm: progress bars

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
- windows-curses: curses compatible module for windows
- WConio: is a wrapper for Turbo-C’s CONIO.H, used to create text user interfaces
- WConio2: pure python implementation of WConio
- Rich: for rendering rich text and beautiful formatting to the terminal with rich text REPL
- Colorama: colouring command-line text
- tabulate: pretty print tabular data
- py_cui: Tk like API for creating CUI/TUI interfaces with widgets, inspired by gocui
- textual: CUI/TUI interface with widgets based on Rich module for formatting

Argument Parser:
- cliche: Build a simple command-line interface from your functions using a decorator while keeping it usage for other scripts
- argparse: it is powerful, but you need a lot of code to construct an argparse CLI
- click: you need a lot of decorators to construct a CLI, and not obvious how to use it
- python-fire: low set up, but annoying traces all the time / ugly design, does not show default values nor types
- cleo: requires too much code/objects to construct
- python-fire: automatically generating command line interfaces (CLIs) from any Python object
- docopt: Command-line interface description language

Password:
- getpass: portable password input without echoing

## General Programming

REPL:
- jupyter-console: ipython like REPL for other kernels like C and Java
- bpython: python repl with undo, autoformatting, autocomplete, highlighting in terminal

Compilers:
- pyston: JIT with upto 30% improvement on server benchmarks and more for simpler programs
- pyjion: JIT which convert code to native CIL and runs with .NET 5 CLR
- cinder: Instagram version of python JIT complier
- pypy: python JIT compiler
- numexpr: extension library for scipy which can further speed up Numpy and Pandas
- numba: similar to numexpr
- nutika and shedskin: transpiler which convert to C++

Python Grammer:
- collections: additional data types
- itertools/functools - tools for using iterators and functions as functional progamming
- functools.singledispatch: provide basic multiple dispatch functionality (function overloading)
- multipledispatch: full featured multiple dispatch
- toolz (itertoolz/functoolz/distoolz) - supplementary to above which implements some missing functionality

Packages / Modules / Enviornments:
- virtualenvwrapper: wrapper for virtualenv tool
- Poetry: simplifies dependeny management for python projects and packages
- flit: tool to simplify package creation and publishing to PyPI
- importlib: working with modules and package resource tool (install importlib_resouces py < 3.7)

Packaging:
- py2exe: create exe's for supported versions of python - doesn't require extraction
- briefcase: tool for converting a Python project into a standalone native application
- pyoxidizer: similar to py2exe runs by extracting to memory but is a rust app requires rust to work
- pyinstaller: extracts to temp and runs, requires virtualenv

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

Debugging:
- print statement: f"{hello=}" # >=python3.8
- sys.settrace and sys.setprofile
- pdbpp: debugger based on pdb with many convenient features
- ipdb: IPython debugger
- pudb: text GUI debugger
- border_patrol: logs all imports and versions
- traceback_with_variables: Adds variables to python traceback, colouring or to file log
- frosch: Runtime Error Debugger with formatted like with variable list
- watchpoints: prints watched variables whenever its value changes and can even trigger pdb
- PySnooper: poor mans debugger, prints every variable change
- pycrunch-trace: debugging and time travel from pytrace.com
- jurigged: hotpatching code while script is being run when files is modified and saved
- pyrasite: Inject code into running Python processes
- Cyberbrain: Backtraces variable change, See every state of program execution, including variables' values

Refactoring:
- Bowler: refactoring tool for manipulating Python at the syntax tree level
- rope: refactoring library
- vulture: find dead/unused code
- bandit: find common security issues in Python code

Performance:
- lru_cache: caching recent calculations
- cache: in functool (>=python3.9.2) same as above
- QuickPotato: create automated tests for profiling performance

Profiling:
- time python <script_name.py>
- python -m timeit -s <script_name.py>
- cProfile: profiler part of stdlib
- line_profiler: profile the time each individual line takes to execute
- memory_profiler: monitoring memory consumption in a process or you can use it for a line-by-line analysis of the memory consumption
- profilehooks: multiple profiling options
- pyinstrument: online profiler
- VizTracer: traces concurrent python programs and also helps in debugging

RPA:
- mouse: monitor and control mouse
- keyboard: monitor and control keyboard, with features such as callback, hotkeys, macro recording and playback etc.
- pynput: Monitor and control input devices like KB and Mouse used for interceptors and keyloggers
- rpa: RPA package for python
- pyautogui: GUI automation
- pywinauto: set of python modules to automate the GUI on Windows and Linux

Configuration Management:
- configparser: for working with ini files
- configupdater: complements configparser with ability to selectively update .ini files
- python-dotenv: Reads the key-value pair from .env file and adds them to environment variable. It is great for managing app settings during development and in production using 12-factor principles
- Dynaconf: can read most config formats
- Hydra: dynamically create hierarchial config and overide with command line options and save each session into a custom config

Testing:
- faker: Fake data generator useful for testing
- unittest: First unit testing framework of the std library
- nose: Extends unit testing for other packages
- doctest: test generation based on output from shell interpreter
- pytest: easy to write small tests, yet scales to support complex functional testing for applications and libraries
- pydantic: data parsing and validation using python type hints
- parameterized: parameterized tests compatible with pytest and unittest supports tests written as functions or methods
- hypothesis: property based tests creating unit tests which are simpler to write and more powerful when run, finding edge cases in your code you wouldn’t have thought to look for
- QuickPotato: create automated tests for profiling performance

Build Automation / CI/CD:
- invoke: task execution tool and libary similar to make
- tox: task automation tool which can make venvs to run builds, tests, docs, publishing etc a complete CI/CD workflow which can also execute make commands

Task Queue / Scheduling:
- Celery: Task queues used as a mechanism to distribute work across threads or machines
- Dramatiq: background task processing library for Python with a focus on simplicity, reliability and performance
- appscheduler: python scheduler for apps
- python-advanced-scheduler: very advanced scheduler
- sched: simple scheduler
- python-crontab: uses os specific scheduler in the background
- schedule: declarative scheduler similar to crontab, easier syntax

Multi-threading / Multi-processing:\
P.S: On non-compute oriented OS's malloc syscalls are not parallelized and hence taking heaving in this aspect will not see a speed up: https://cosmiccoding.com.au/tutorials/multiprocessing
- uvloop: ultra fast event loop implemented with Cython
- concurrent.futures: higher level library for multiprocessing / multithreading libraries
- Joblib: set of tools to provide lightweight pipelining in Python, transparent disk caching and parellel computing with special focus on numpy and can use any of the below backends including dask or a custom backend
    - loky: easy to use executor function
        - threading: library for working with threads
        - multiprocessing: library for working with processess
- Entangle: ightweight (serverless) native python parallel processing framework based on simple decorators and call graphs

Distributed Computing:
- mpi4py: MPI (Mesasge Parsing Interface) distribute workloads on multiple CPU's
- ray: easy to use distributed computing framework
- p_tqdm: distributed computing wrapper based on pathos
    - pathos: framework for heterogeneous computing

### Android / Mobile phone

- ppadb: pure python implementation of adb client which interfaces with the adb server on PC

### Electronics / Microcontrollers

- coolterm: module to automate coolterm - a serial monitor app
- pyserial: python library for interacting with serial port

### Web Programming

Webscripting:
- Brython: run python in place of javascript in the frontend

HTML / Web page generation:
- jinja2: templating engine
- Flatpages / Flask - markdown supported static website creation https://www.jamesharding.ca/posts/simple-static-markdown-blog-in-flask/
- mkdocs: static site generator for documentation
- Esparto: Create webpages to display data and outputs using bootstrap and jinja2

Webservice API:
- https://public-apis.io/
- https://github.com/public-apis/public-apis
- clarifai: computer vision AI platform 5k free calls/mo
- clearview.ai: computer vision API
- openvisionapi: open source computer vision API

Webservice API modules:
- tweepy: Twitter streaming API library
- twitter-scraper: Twitter frontend (JavaScript) has it's own API, reverse–engineered. No API rate limits. No restrictions. Extremely fast
- facebook-scraper: similar to twitter-scraper to scrape data without API
- python-telegram-bot: telegram bot wrapper
- InstaPy: Instagram selenium bot
- google-api-python-client: google api client
- pygooglenews: A python wrapper of the Google News RSS feed

Endpoint Frameworks:
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

## Data Science

Project Folder Structure Skeleton:
- cookiecutter / ccds: folder structure for datascience
- PyScaffold: tool for bootstrapping high quality Python packages, ready to be shared on PyPI and installable via pip
    - pyscaffoldext-dsproject: extension for datascience projects

Process / Best Practices:
- recommenders: Best Practices on Recommendation Systems

Data Storage:
- dvc: Data version control. Git for data
- pytables: Data storage for df from within pandas
- pystore: Data storage for df from within pandas

Data Cleaning:
- Dplython: dyplr R equivalent for summarizing
- pyjanitor: Clean APIs for data cleaning. Python implementation of R package Janitor

EDA libraries:
- Flenser: simple automated data exploration tool that runs tests on dataset and provides summary
- data-describe: toolkit for Exploratory Data Analysis (EDA). It aims to accelerate data exploration and analysis by providing automated and opinionated analysis widgets
- lux: API for Intelligent Visual Data Discovery
- pandas-profiling: EDA support for pandas dataframe

Pandas:
- Quickstart:
    - http://pandas.pydata.org/pandas-docs/stable/10min.html
    - http://pandas.pydata.org/pandas-docs/stable/cookbook.html
    - https://github.com/jvns/pandas-cookbook
- bamboolib: GUI for pandas df
- pandas-gui: GUI for pandas df
- sidetable: Create Simple Summary Tables in Pandas
- missingno: Missing data visualisation in pandas

Pandas Alternatives:
- datatable: h2oai's table based on extremely fast data.table from R
- polars: fast, multithreaded DataFrames library implemented in Rust using Apache Arrow as memory model
- Vaex: lazy out-of-core dataframes
- StaticFrame: a consistent interface for working with datafames alternative to pandas
- RAPIDS: drop in replacement library for pandas to speed up data science analysis optimised CUDA (Nvidia) - better than pandas with GPU
- Dask: build on top of pandas to parallelize it, slower will non parallel
- Modin: Drop in replacement for pandas to speed up common timeconsuming task by parellelising code using Ray or Dask

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
- geemap: Google Earth Engine API
- leafmap: geemap alternative based on folium and ipyleaflet

Graphs:
- NetworkX, igraph - Graph analysis
- nxviz: Graph Visualiation
- Pydot: graph plotting
    - Graphviz – underlying for pydot

NLP:
- NLTK: Oldest NLP
- SpaCy: New NLP
- Gensim: robust semantic analysis, topic modeling and vector-space modelling
- nlp: lightweight and extensible library to easily share and access datasets and evaluation metrics for Natural Language Processing (NLP) based on tensorflow dataset tfds

### Finance:

Data:
- yahooquery: Yahoo finance API unofficial
- Nsepy: API for nse including CLI depends on numpy and pandas

Technical Analysis:
- talib: Technical Analysis
- pandas-ta: Technical Analysis Indicators - Pandas TA is an easy to usePandas Extension with 120+ Indicators
- finta: Common financial technical indicators implemented in Pandas

Strategies:
- Backtrader: Backtesting
- backtesting.py
- Zipline: Backtesting
- Pyfolio: To check portfolio perf metrics
- Mibian: Options Pricing

Data Analytics:
- Pyodide: Python with the scientific stack, compiled to WebAssembly

IPython / Jupyter / Notebooks:
- jupyterlife: JupyterLab distribution that runs entirely in the browser based on Pyodide
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
- jupyter-notify: notification when long running notebooks finish running
- ipywidgets: adds interactivity to jupyter notebooks
- papermill: parametrizing jupyter notebooks so the notebook can be run for different values and also build workflow based on results of the notebook
- rise: reveal.js based presentation for live notebooks
- voila: GUI's from jupyter notebook based on ipywidgets
- bqplot: interactive 2-D visualization system for Jupyter, based on the constructs of the Grammar of Graphics
- powerbi-jupyter: IPyWidget that enables customers to use PowerBI embedding capabilities in a Jupyter notebook seamlessly

### Modelling

Stats:
- Statsmodels: for statistical and unit tests
- PyMC3: statistical modeling tool for Bayesian statistical modeling & Probabilistic Machine Learning which focuses on advanced Markov chain Monte Carlo and variational fitting algorithms
- ppscore: Predictive Power Score (PPS) replacement for corelation to detect relationships using decision trees ML model from sklearn internally

Time Series:
- darts: easy manipulation and forecasting of time series
- sktime: machine learning toolbox for time series forecasting
- PyFlux: time series model library for Python
- dtw-python: Dynamic time warping to fit data two time series by finding minimum distance between the series
- greykite: fast, intuitive, flexible forecasting model from linkedin
- prophet: timeseries forecasting model from facebook

Machine Learning:
- mlfinlab: machine learning for finance
- scikit-learn: algorithms of machine learning and data mining tasks
- XGBoost/LightGBM - optimised, scalable and fast implementations of gradient
- shogun: machine learning toolbox written in C++ available for multiple languages
- Hummingbird: compile trained traditional ML models into tensor computations PyTorch
- Libra: automates the end-to-end machine learning process in just one line of code. It is built for both non-technical users and software professionals of all kinds.
- LazyPredict: help build a lot of basic models without much code and helps understand which models works better without any parameter tuning
- PyGAD: library for Building the Genetic Algorithm and Training Machine Learning Algoithms (Keras & PyTorch).

Deep Learning:
- keras: makes deep learning easier to learn with a simpler api and clear error messages
    - TensorFlow - Googles framework for deep learning / machine learning
- PyTorch: Performs tensor computations with GPU acceleration, create dynamic computational graphs and automatically calculate gradients
- fastai: simplified neural net training with best practices with out of the box support for many types of ML
- H20: AI library

Image Processing / Character Recognition (OCR) / Image Recognition / Computer Vision:
- Pytesseract: Tesarract 4 python bindings
- imageio: image manipulation library depends on numpy and pillow
    - pillow: maintained version of PIL, for working with images
- imutils: image maniputlation utilities
- opencv-contrib:
    - OpenCV-Python: Open computer vision library

Audio Processing / Speech Recognition:
- SpeechRecognition: Library for performing speech recognition, with support for several engines and APIs, online and offline
- voice2json: speech recognition, transcription, intent recognition command line tools
- Picovoice: voice recognition library to add Alexa like feature to python apps

## Utilities

- pint: Python units library

Time and date:
- datetime: working with date and time
- python-dateutil: working with timezones
- pytz: alternative to python-dateutil (has different interface compared to dateutil so dateutil is preferred)
- dateparser: Natural language date parsing, supports multiple languages
- arrow: offers a sensible and human-friendly approach to creating, manipulating, formatting and converting dates, times and timestamps
- pendulum: improves API consistency over arrow
- calender: generate calendars for any month

Multi-Media:
- pytube: lightweight, dependency-free Python library (and command-line utility) for downloading YouTube Videos
    - youtube-dl: download vidoes from multple sites
- manim: create animations with python scripts
- pyFLAC: Real-time lossless audio compression in Python based on Soundfile which in turn is based on libsndfile, CFFI and numpy
- gdb: python module for GDB scripting

## Apps
- HTTPie: command-line HTTP client to make CLI interaction with web services as human-friendly as possible alternative to curl
- ChatterBot: ML based python chatbot
- JSMon: JavaScript Change Monitor for BugBounty
- Ciphey: automated decryption tool. Input encrypted text, get the decrypted text back
- byob: Python based botnet
- ngrap: app tunneling https://ngrok.com/
- jprq: ngrok alternative
- pywhat: `what` wrapper to identify any data such as email, domains etc in pcap or text files
- recoverypy: search and recover blocks in block devices transparent to overwritten files
