# Useful Python Modules

As Python is finding use in many different applications and huge number of modules with a similar objective but different ideology / features are introduced, a list of propular / useful modules for quick reference helps a lot.

The main categorisation is between python apps in the traiditonal sense vs the more recent but rapidly growing data science ecosystem. While the common sections seperated out.

## Other Similar Collations

 - https://github.com/vinta/awesome-python/
 - https://github.com/ml-tooling/best-of-web-python
 - https://github.com/florimondmanca/awesome-asgi
 - https://www.libhunt.com/
 - https://libraries.io/

Cheatsheets:
 - https://www.programiz.com
 - https://overapi.com/python
 - https://devhints.io
 - https://pyformat.info
 - https://strftime.org

## Input & Output / IO

System:
 - stdlib> gc: garbage collector!!!
 - stdlib> shutil: Shell utility function like file properties and manipulation
 - stdlib> pathlib: Object-oriented filesystem paths
 - stdlib> glob: glob operator for files as python list
 - stdlib> webbrowser: Convenient Web-browser controller
 - stdlib> mmap: map disk to memory to read large files without completely loading them to RAM
 - fileless-elf-exec: Execute ELF files without dropping them on disk directly from memory
 - pyfilesystem: filesytem abstraction works with zip, ftp, cloud, memory, etc.
 - sh: full-fledged subprocess replacement that allows you to call any program as if it were a function
 - WinSys: Python tools for the Windows Administrator
 - pyperclip: clipboard access
 - pywin32: provides access to many of the Windows APIs from Python
     - win32com: Windows COM object and client
     - win32api: Windows system calls

Compatibility:
 - reticulate: tools for interoperability between Python and R
 - rpy/rpy2: calling R from python
 - compatlib: Python utilities for writing cross-version compatible libraries

Text Processing:
 - stdlib> string: convenience functions for text such as templates strings
 - textract: Text extraction from variety of document and images
 - texthero: Text preprocessing, representation and visualization
 - Flashtext: Fast full word replacement
 - Emoji: Unicode emoji conversion
 - emot: library to convert emojis to text with meaning
 - parse: Parse strings using a specification based on the Python format() syntax
 - numerizer: convert spelled numbers to real numbers
 - cogapp: lets you use pieces of Python code as generators in your source files to generate whatever text you need
 - docx2txt: extract text from MSWord docx format
 - catdoc: extract text from MSWord doc format
 - python-docx: create and edit MSWord documents

PDFs:
 - pText: pure python pdf manipulation as a JSON like structure support read and editing
 - fpdf2: minimalist PDF creation library successor to PyFPDF
 - Pypdf2: for working with pdf’s
 - ReportLab: for creating PDFs programmatically
 - PDFx: extract data, links and metadata from pdfs as CLI or library
 - PyPDFParser: Visualize and extract structured data from PDF files
 - pdfminer: for mining pdf files
 - camelot: Extract tables from text based PDF files

Spreadsheets:
 - openpyxl: for working with Excel 2010 format (.xlsx) excel files
 - xlsxwriter: module for creating Excel 2010 (.xlsx) files, in particular, charts
 - pyxlsb: read Excel files in the (.xlsb) format
 - xlrd: For reading older Excel (.xls) documents
 - xlwt: For writing older Excel (.xls) documents
 - formulas: interpreter for parsing and calculating Excel formulae
 - xlwings: Works with new Excel formats and has macro capabilities but depends on excel
 - PyXLL: use python instead of macros in Excel making python accessible from excel (commercial)
 - gspread: API for Google Sheets

Presentations:
 - python-pptx: create and edit Microsoft Powerpoint documents
 - gslides: Creating charts in Google slides

Documentation:
 - sphinx: Docs generator
 - mkdocs: static site generator for documentation
    - mkdocstrings: Automatic documentation from sources, for MkDocs
 - pycco: port of Docco which generates simple docs from code

JSON / HOCON:
 - pyhocon: Human-Optimized Config Object Notation (HOCON / JSON superset) parser / converter into JSON, YAML
 - ujson: Extremely fast json library written in C
 - json-traverse: simple JSON parser
 - JmesPath: declarative access to json elements
 - jsonpath-ng: traverse JSON elements in `.` (dot) notation (JSON notation) link in javascript
 - jpath: access lists and dicts with `.` (dot) notation like JSON with wildcard, slicing and conditionals support

Data Parsing / Conversion:
 - quarto: A scientific and technical publishing system built on Pandoc using markdown
    - pandoc: commandline tool to convert documents from many different formats
 - stream_unzip: steam data from zip files instead of reading / loading the entire file
 - difflib: library for comparison and identify difference between patterns with many helpful methods
 - lxml.etree: fast and wide std support (XPath, XMLSchema, XSLT)
 - xml.etree.ElementTree: parse XML files
 - untangle: simple library to access XML in a pythonic way depends on xml.sax and is designed for samll files; implemented in pure python
 - xmltodict: convert xml to python dict and vice versa
 - Python-OOXML: working with Office Open XML files >=MSOffice2013 formats
 - chardet: for detecting character set for a file
 - python-markdown: python implementation of John Grubers markdown
 - Shelve: pickle wrapper
    - Pickle / cpickle: for serializing objects for storage
 - fsspec: provides an abstract filesystem with a consistent API for file access
 - PyYAML: YAML parser
 - rst2pdf: creates PDF documents from your ReStructured Text markup

Data validation:
 - cerberus: powerful yet simple and lightweight data validation functionality out of the box and is designed to be easily extensible, allowing for custom validation
 - pydantic: data parsing and validation using python type hints making it easier to write classes
    - pydbantic: single model for shaping, creating, accessing, storing data within a Database
 - marshmellow: ORM/ODM/framework agonostic library for converting complex datatypes such as objects to and from Python datatypes
 - great_expectations: data validation framework
 - pandera: statistical data validation for pandas
 - pydeequ: scala based data validator with dynamic checks and anomaly detection

SQL / Databases:
 - sqlite-utils: library and command line tool with convenience fns for working with sqlite db
 - sqlcommenter: add meta info to your SQL queries as comments which can be useful for debugging
 - Alembic: for database migration
 - sqlmodel: SQL databases in Python, designed for simplicity, compatibility, and robustness based on Pydantic and SQLAlchemy made by FastAPI authour
    - SQLAlchemy: Most popular ORM for python
 - zodb: Python object-oriented database
 - piccolo: fast, user friendly ORM and query builder which supports asyncio
 - preql: interpreted relational query language that complies python to sql written in python
 - psycopg2: the most popular PostgreSQL database adapter for the Python
 - Vinum: use SQL on python datatypes in-memory for data analytics using Postgress's pglast parser
 - DuckDB: run SQL queries on many data files including on pandas dataframes
 - FugueSQL: run SQL queries on pandas, spark and dash within notebook cells
 - SQLFluff: dialect-flexible and configurable SQL linter written in python
 - SQLLineage: shows source and target tables for any SQL query for complex queries

Datafiles / Tabular Data:
 - dataconverters: Unified python library and command line interface to convert data from one format to another (especially tabular data)
 - tablib: format agonistic tabular dataset library supporting json, csv, xls, yaml etc
 - datamatrix: light-weight library for working with tabular data  with spreadsheet-like structure that consists of named columns and numbered rowfpa
 - csvkit: Library for working with csv files
 - comma: csv Library for Humans; python object like indexing and manipulation
    - clevercsv: drop-in replacement for the Python csv package with improved dialect detection for messy CSV files and a handy command line tool that can standardize a messy file or generate Python code to import it

Data Ecosystem:
 - dbt: data transformation within the warehouse using sofware best practices such as CI/CD, version control etc
 - blaze: set of libraries that help users store, describe, query and process data

### Network / Communication:

HTTP / TCP / UDP / Websocket:
 - requests: easy to use http client based on urllib3
    - requests-cache: Caching for requests library
 - mechanize: a browser that implements the urllib2.OpenerDirector interface with state, including navigation history, HTML form state, cookies, etc based on perl's WWW::Mechanize
 - packet-sniffer: pure-Python network packet sniffer based on PF_PACKET (Linux only)
 - httpx: next generation HTTP client for Python based on requests
 - aiohttp: asynchronous http client

XML / Atom / RSS:
 - reader: retrieve, store, and manage web feeds through a high-level API, without having to deal with feed-related details
 - feedparser: parse Atom and RSS feeds

Web Scraping:
 https://pixelscan.net/
 https://httpbin.org/headers
 http://webnumbr.com/
 - BeautifulSoup: parser for xml / html
 - elemental: makes Selenium automation faster and easier by adding automatic waits and common missing usecases from selenium
    - Selenium – Browser automation
 - selenium-wire: give access to underlying requests made by the browser
 - playwright: puppeteer devs new project after moving to microsoft for browser control similar API as puppeteer runs on NodeJS backend
 - pyppeteer: Headless chrome/chromium automation library (unofficial port of puppeteer)
 - scrapy: web crawler
 - pyspider: web crawler
 - cloudproxy: Provision proxy servers across different cloud / datacenter provider ips

Email:
 - stdlib> email: For managing email messages. With this we will setup the email message itself, including subject, body, and attachments.
 - stdlib> smtplib: Handles the SMTP connection
 - stdlib> IMAPlib: working with IMAP connections

### GUI / Interface

Indicators:
 - progress / fastprogress / alive-progress / tqdm: progress bars

GUI:
 - win10toast: Notifications in windows or win10toast-click for clickable version
 - PyWebIO: simple web app interface / GUI generation in python script
 - pyrustic: framwwork for making GUI's uses tk
 - PySimpleGUI: Simple python GUI framework using tkinter, Qt, Remi or WxPython
 - edifice: makes it simple to build a fully reactive UI based on Javascript libraries such as React
 - re-wx: library for building modern declarative desktop applications in WX
 - Kivy: cross-platform framework for development of applications that make use of innovative, multi-touch user interfaces
 - Toga: Python native, OS native, cross platform GUI toolkit
 - atlas-python: Atlas toolkit is the easiest way to add a web-based graphical user interface
 - streamlit: create beautiful, performant apps in a few hours in pure Python
 - gradio: deploy ML models, fns, API with UI
 - voila: GUI's from jupyter notebook based on ipywidgets
 - litemark: Lightweight Markdown dialect for Python desktop apps

Terminal-UI:
 - stdlib> textwrap: wrap text in console to configurable width
 - curses: used to create text user interface is restricted to Unix-like systems
 - windows-curses: curses compatible module for windows
 - WConio: is a wrapper for Turbo-C’s CONIO.H, used to create text user interfaces
 - WConio2: pure python implementation of WConio
 - rich: for rendering rich text and beautiful formatting to the terminal with rich text REPL
 - colorama: colouring command-line text
 - tabulate: pretty print tabular data
 - prettytable: pretty print tabular data
 - py_cui: Tk like API for creating CUI/TUI interfaces with widgets, inspired by gocui
 - textual: CUI/TUI interface with widgets based on Rich module for formatting
 - blessed: TUI interface similar to textual
 - bashplotlib: plot graphs in the console
 - plotext: plotting in terminal with matplotlib like interface

CLI:
 - stdlib> argparse: it is powerful, but you need a lot of code to construct an argparse CLI
 - cliche: Build a simple command-line interface from your functions using a decorator while keeping it usage for other scripts
 - typer: CLI based on type hints similar to FastAPI by FastAPI authour
    - click: you need a lot of decorators to construct a CLI, and not obvious how to use it
 - python-fire: low set up, but traces all the time / design lacking, does not show default values and types
 - cleo: requires too much code/objects to construct
 - python-fire: automatically generating command line interfaces (CLIs) from any Python object
 - docopt: Command-line interface description language

Cryptography / Hashing / Password:
 - stdlib> getpass: portable password input without echoing
 - stdlib> crypt: provides functions that could be used for password hashing dependending on your system and aren’t as strong as passlib
 - stdlib> hashlib: provides functions for file hashing
 - stdlib> secrets:
 - passlib: widely used and tested hashing library with strong encryption
 - bcrypt: bcrypt hasing algo. Password storage requires multiple passes
 - hmac: used to verify integrity and authenticity of message and doesn’t have the properties required for password hashing
 - keyring: by default uses your user account login password for encryption, so it gets automatically unlocked when you login and you therefore don’t have worry about extra password
 - pycryptodome/pycryptodomex: self-contained low-level cryptographic primitives

## General Programming

OS:
 - pyRTOS: RTOS written in Python
 - xonsh: shell language and command prompt

REPL:
 - jupyter-console: ipython like REPL for other kernels like C and Java
 - bpython: python repl with undo, autoformatting, autocomplete, highlighting in terminal
 - ptpython: REPL build on top of the prompt_toolkit library

Compilers / Decompilers:
 - dis: disassembiling CPython bytecode
 - mypyc: compiles Python modules to C extensions using standard Python type hints to generate fast code
 - pypy: python JIT compiler
 - pyston: JIT with upto 30% improvement on server benchmarks and more for simpler programs
 - pyjion: JIT which convert code to native CIL and runs with .NET 5 CLR from Microsoft
 - cinder: python JIT complier from Instagram
 - skybison: ground up high performance version of python from Instagram
 - numexpr: extension library for scipy which can further speed up Numpy and Pandas
 - numba: similar to numexpr
 - nutika and shedskin: transpiler which convert to C++
 - Rusthon: multi-language tranpiler written in python
 - pythonjs: python to JS tranpiler offering upto 20X speeup on typed code
 - taichi: parallel programming language for high-performance numerical computations embedded in Python, and its just-in-time compiler offloads compute-intensive tasks to multi-core CPUs and massively parallel GPUs

Python Grammer:
 - __future__: import features implemented in newer versions of python
 - stdlib> atexit: register function to run at sys.exit() to cleanly terminate
 - operator: python operators and convenience functions such as itemgetter, attrgetter, methodcaller for sorting with key and filtering data
 - collections: additional data types
 - itertools/functools - tools for using iterators and functions as functional progamming
 - functools.singledispatch: provide basic multiple dispatch functionality (function overloading)
 - multipledispatch: full featured multiple dispatch
 - runtype: Utilities for simplyfying run-time type validation and multiple dispatch
 - toolz (itertoolz/functoolz/distoolz) - supplementary to above which implements some missing functionality
 - operator: contains a large number of efficient functions corresponding to Python operators
 - ast: sytax parsing and manipulation for linting, patching, refactoring
 - astunparse: unparse changes done using `ast` module to convert to python code
 - python-goto: enable goto by rewriting the bytecode
 - copy: with copy and deepcopy methods for making copies of python objects

Packages / Modules / Environments:
 - stdlib> importlib: working with modules and package resource tool (install importlib_resouces py < 3.7)
 - pydeps: read code and draw a dependency graph
 - pipdeptree: command line utility for displaying the installed python packages in form of a dependency tree
 - virtualenvwrapper: wrapper for virtualenv tool
    - Virtualenv: parent of stdlib> venv with some additional features not available in venv
 - pyenv: shell script to manage multiple installations of python
 - pipx: install end user apps in a seperate isolated virtual env available globally
 - pip-tools: version pinning and hashes to mitigate supply chain attacks
 - pip-audit: scan environments for packages with known vulnerabilities
 - pipenv: dependency management for packages and projects intergrating virtual enviornments with pip
 - poetry: simplifies dependeny management for projects and packages
 - flit: tool to simplify package creation and publishing to PyPI

Distribution:
 - py2exe: create exe's for supported versions of python - doesn't require extraction
 - briefcase: tool for converting a Python project into a standalone native application
 - pyoxidizer: similar to py2exe runs by extracting to memory. Rust app so requires rust
 - pyinstaller: extracts to temp and runs, requires virtualenv
 - pyinstxtractor: Python script to extract the contents of a PyInstaller generated Windows executable file

Linting:
 - pylint: superset of flake8
 - flake8: check for errors and style wrapper on pyflakes and few other tools
    - pyflakes: A simple program which checks Python source files for error
    - mccabe: code complexity checker
    - pycodestyle: formally called pep8
 - pygrep: Find python identifiers in code files where they are imported

Type Checking:
 - stdlib> typing: type hinting and annotations with modern IDE's
 - pyannotate: Insert annotations into your source code based on call arguments and return types observed at runtime
 - MonkeyType: collects runtime types of function arguments and return values, and can automatically generate stub files or even add draft type annotations directly to your code from Instagram
 - pytype: checks and infers types without requiring type annotations
 - mypy: optional static type checker
 - pytype: checks and infers types for your Python code - without requiring type annotations also support cross function inference which is not available with mypy and also allows runtime lenience compared to mypy(windows support pending) (Google)
 - pyre: static type checker (Facebook)
 - pyright: static type checker (Microsoft)
 - attrs: creating dataclasses with less boilerplate based on type hints on which stdlib dataclasses is based on

Dynamic Type Checking:
 - enforce
 - typeguard
 - typo
 - ducktype
 - strictconf
 - pytypes

Formatting / Styling:
 - black: automatic code formatter
 - yapf: highly configurable code formatter from Google that can use multiple code styles
 - autopep8: built on pycodestyle for autoformatting code
    - pycodestyle: formally called pep8
 - pydocstyle: check doc string formatting
 - isort: automatic import formatter
    - seed-isort-config: statically populate the known_third_party part of the .isort.cfg

Logging:
 - structlog: structured logging library
 - loguru: easily configurable logging library with debugging info in log

Debugging:
 - stdlib> print statement: f"{hello=}" # >=python3.8
 - stdlib> sys.settrace and sys.setprofile
 - objexplore: terminal UI to inspect and explore Python objects
 - objprint: print Python objects in human readable format
 - icecream: pretty print and easily managable print function for debugging
 - watchpoints: prints watched variables whenever its value changes and can even trigger pdb
 - PySnooper: poor mans debugger, prints every variable change
 - pdbpp: debugger based on pdb with many convenient features
 - pudb: text GUI debugger
 - ipdb: IPython debugger
 - border_patrol: logs all imports and versions
 - friendly_traceback: clearer traceback messages
 - traceback_with_variables: Adds variables to python traceback, colouring or to file log
 - frosch: Runtime Error Debugger with formatted like with variable list
 - pycrunch-trace: debugging and time travel from pytrace.com
 - jurigged: hotpatching code while script is being run when files is modified and saved
 - pyrasite: Inject code into running Python processes
 - Cyberbrain: Backtraces variable change, See every state of program execution, including variables' values

Refactoring:
 - Bowler: refactoring tool for manipulating Python at the syntax tree level
 - rope: refactoring library
 - vulture: find dead/unused code
 - bandit: find common security issues in Python code

Caching:
 - functools> lru_cache: caching recent calculations
 - functools> cache: lru_cache enhancement (>=python3.9.2)

Profiling:
 - stdlib> time python <script_name.py>
 - stdlib> python -m timeit -s <script_name.py>
 - stdlib> python -X importtime <script_name.py>
 - stdlib> tracemalloc: tracks every individual memory blocks allocated by the Python interpreter (30% perf hit)
 - stdlib> resource: provides basic controls for resources that a program allocates (point in time reporting needs more code for running another monitoring thread for profiling multiple points but imprecise if sampling duration is too long)
 - cProfile: profiler part of stdlib
 - line_profiler: profile the time each individual line takes to execute
 - memory_profiler: monitoring memory consumption in a process or you can use it for a line-by-line analysis of the memory consumption
 - profilehooks: multiple profiling options
 - QuickPotato: create automated tests for profiling performance
 - pyinstrument: online profiler
 - VizTracer: traces concurrent python programs and also helps in debugging
 - palanteer: High performance visual profiler, debugger, tests enabler for C++ and Python
 - scalene: a high-performance, high-precision CPU, GPU, and memory profiler and find bottlenecks in data too

RPA:
 - mouse: monitor and control mouse
 - keyboard: monitor and control keyboard, with features such as callback, hotkeys, macro recording and playback etc.
 - pynput: Monitor and control input devices like KB and Mouse used for interceptors and keyloggers
 - rpa: RPA package for python
 - pyautogui: GUI automation
 - pywinauto: set of python modules to automate the GUI on Windows and Linux
 - robotframework: RPA language implemented in python

Configuration Management:
 - python-decouple: full featured config module initially designed for django compatible with ini and env with auto type casting, default config, config overiding etc
 - stdlib> configparser: for working with ini files
 - configupdater: complements configparser with ability to selectively update .ini files
 - python-dotenv: Reads the key-value pair from .env file and adds them to environment variable. It is great for managing app settings during development and in production using 12-factor principles
 - Dynaconf: can read most config formats
 - Hydra: dynamically create hierarchial config and overide with command line options and save each session into a custom config

Testing:
 - stdlib> unittest: First unit testing framework of the std library
 - stdlib> doctest: test generation based on output from shell interpreter
 - nose: Extends unit testing for other packages
 - pytest: easy to write small tests, parametric tests, scales to support complex functional testing for applications and libraries
    - xdoctest: rewrite of Python's builtin doctest module (with pytest plugin integration) with AST
 - parameterized: parameterized tests compatible with pytest and unittest supports tests written as functions or methods
 - hypothesis: property based tests creating unit tests which are simpler to write and more powerful when run, finding edge cases in your code you wouldn’t have thought to look for
 - QuickPotato: create automated tests for profiling performance

Mocking / Fake data:
 - faker: Fake data generator useful for testing
 - mockeroo: fake data generator
 - freezegun: mock datetimes for testing

Workflow / Automation Frameworks:
 - luigi: workflow automation framework from Spotify
 - airflow: workflow automation framework from Airbnb
 - redun: Yet another redundant workflow engine

Packaging / Distribution / Build / CI/CD tools:
 - Deprecated setup.py: https://pypa-build.readthedocs.io/en/stable/
 - setup.cfg: https://setuptools.pypa.io/en/latest/userguide/
 declarative_config.html#example-setup-config
 - twine: utility for publishing packages to PyPI and other repositories. It provides build system independent uploads of source and binary distribution artifacts for both new and existing projects
 - invoke: task execution tool and libary similar to make
 - pydoit: doit comes from the idea of bringing the power of build-tools to execute any kind of task
 - tox: task automation tool which can make venvs to run builds, tests, docs, publishing etc a complete CI/CD workflow which can also execute make commands
 - nox: command-line tool that automates testing in multiple Python environments, similar to tox. Unlike tox, Nox uses a standard Python file for configuration
 - pre-commit: framework for managing and maintaining multi-language pre-commit hooks
 - pants: Pants 2 is a fast, scalable, user-friendly build system for codebases of all sizes. It's currently focused on Python, Shell, Docker, and Go.

Task Queue / Message Queue / Scheduling:
 - Celery: Task queues used as a mechanism to distribute work across threads or machines
 - Dramatiq: background task processing library for Python with a focus on simplicity, reliability and performance
 - pika: pure-Python implementation of the AMQP 0-9-1 protocol including RabbitMQ’s extensions
 - APScheduler: very advanced scheduler
 - sched: simple scheduler
 - python-crontab: uses os specific scheduler in the background
 - schedule: declarative scheduler similar to crontab, easier syntax

Multi-threading / Multi-processing:\
 P.S: On non-compute oriented OS's malloc syscalls are not parallelized and hence taking heaving in this aspect will not see a speed up: https://cosmiccoding.com.au/tutorials/multiprocessing
 - uvloop: ultra fast event loop implemented with Cython
 - concurrent.futures: higher level library for multiprocessing / multithreading libraries
 - promiseio: promises like JS for any non-async fn which will run without calling fn with await
 - mpire: easy multiprocessing, but faster than multiprocessing
 - Joblib: set of tools to provide lightweight pipelining in Python, transparent disk caching and parellel computing with special focus on numpy and can use any of the below backends including dask or a custom backend
    - loky: easy to use executor function
        - threading: library for working with threads
        - multiprocessing: library for working with processess
 - Entangle: lightweight (serverless) native python parallel processing framework based on simple decorators and call graphs

Distributed Computing:
 - mpi4py: MPI (Mesasge Parsing Interface) distribute workloads on multiple CPU's
 - ray: easy to use distributed computing framework
 - p_tqdm: distributed computing wrapper based on pathos
    - pathos: framework for heterogeneous computing

### Android / Mobile phone

 - python-adb: pure-python implementation of the ADB and Fastboot protocols, without using daemon between the client and the device, and therefore does not support multiple simultaneous commands to the same device using libusb1 and not official Google product.
 - adb_shell: originated from python-adb; implements ADB shell and FileSync functionality
 - ppadb: pure python implementation of adb client which interfaces with the adb server on PC
 - mtkclient: unofficial MTK reverse engineering and flash tool

### Electronics

Design:
 - pinout: method to create pin-out diagrams for electronic hardware with SVG diagram creation
 - nmigen: toolbox for building complex digital hardware alternative to Verilog, VHDL

Hardware Interface:
 - coolterm: module to automate coolterm - a serial monitor app
 - pyserial: python library for interacting with serial port over a variety of different devices: old-style serial ports, Bluetooth dongles, infra-red ports etc
 - PyUSB: access USB devices; relies on a native system library
 - USPP: access serial portsv which only works in Windows for now

Graphics:
 - lvgl: Light and Versatile Graphics Library for microcontrollers with micropython bindings

### Web Programming

Webscripting:
 - Brython: run python in place of javascript in the frontend

HTML / Web page generation:
 - jinja2: templating engine
 - nikola: static site generator
 - pelican: static site generator
 - flask-flatpages: markdown supported static website creation https://www.jamesharding.ca/posts/simple-static-markdown-blog-in-flask/
 - pygments: python sytax highlighter for webpages
 - fastpages: github pages like static site generator from many different document formats
 - esparto: Create webpages to display data and outputs using bootstrap and jinja2

Webservice API:
 - https://public-apis.io/
 - https://github.com/public-apis/public-apis
 - clarifai: computer vision AI platform 5k free calls/mo
 - clearview.ai: computer vision API
 - openvisionapi: open source computer vision API
 - wolframalpha: solving math, natural language, 3D plots etc.
 - wikidata: Archive of structured data from wikipedia
 - dbpedia: Knowledge graph of various data sources

Webservice API libraries:
 - tweepy: Twitter streaming API library
 - twitter-scraper: Twitter frontend (JavaScript) has it's own API, reverse–engineered. No API rate limits. No restrictions. Extremely fast
 - facebook-scraper: similar to twitter-scraper to scrape data without API
 - python-telegram-bot: telegram bot wrapper
 - Telethon: Telegram bot library
 - InstaPy: Instagram selenium bot
 - pytrends: unofficial google trends api scraped from trends site
 - google-api-python-client: google api client
 - google-workspace: unofficial high level Python API wrapper for some of the productivity based Google APIs, that is focused on simplicity
 - newspaper3k: data from 1000's of newspapers with metadata
 - pygooglenews: A python wrapper of the Google News RSS feed
 - wikipedia: wikipedia API
 - wikipedia_ql: Query language for efficient data extraction from Wikipedia

Authentication:
 - easyauth: Create a centralized Authentication and Authorization token server. Works with FastAPI well.

Endpoint Frameworks:
 - Flask: micro-web framework, that helps to build an APIs and supports unit testing;
 - FastAPI: light and fast built on top of starlette, pydantic and Uvicorn
 - CherryPy: minimalist, manipulable, light with lot of plugins
 - Bottle: lightweight and self contained micro framework with webserver and no additional dependencies
 - Web2py: light with no dependencies, fully-featured IDE, full stack, old fashioned
 - Tornado: also an asynchronous networking library allows for large and scaling solution
 - Quart: combination of asyncio and flask
 - Pyramid: scalable and OO
 - Falcon: minimalist web API framework which is very fast used for large scale encourages REST
 - Enferno: A Python framework based on Flask microframework, with batteries included, and best practices in mind
 - instant-api: Instantly create an HTTP API with automatic type conversions, JSON RPC, and a Swagger UI with all the boring stuff done for you
 - hug: api/cli/local function; connected to a whole web framework, but gets a lot right

Django: web framework for building a complex, data-driven websites
 - cookiecutter-django: framework for jumpstarting production-ready Django projects quickly
 - django-rest-framework: powerful and flexible toolkit for building Web APIs using REST
 - graphene-django: for creating GraphQL API
 - django-pymemcache: Django cache backend that uses Pinterest's pymemcache library as the backend
 - django-filter: filter result data
 - kolo: See everything happening in your running Django app without leaving VSCode

WSGI servers:
 - Gunicorn

ASGI server:
 - Uvicorn: ASGI server
 - Starlette: toolbox of higher-level components such as requests and responses that you can use to abstract away some of the details of ASGI

## Basic Science

Mathematics:
 - stdlib> decimal: decimal data type whose results match calculations done by hand and have configurable precision
 - stdlib> fractions: conversion of real numbers to fractions and wise versa with high precision
 - sympy: symbolic fuctions which be used for solving math expressions such as intergals, limits
 - theano: define, optimize, and efficiently evaluate mathematical expressions involving multi-dimensional arrays, built on top of NumPy and allows use of GPU for fast calculations
 - handcalcs: convert or render mathematicals equations in python directly to mathtext / latex

Statistics:
 - stdlib> statistics: statistical functions
 - fitter: provides a simple class to identify the distribution from which a data samples is generated from
 - lmfit: provides a high-level interface to non-linear optimization and curve fitting
 - glum: generalized linear models common methods like least-squares regression, Poisson regression and logistic regression as special cases based on sklearn with similar API
 - pingouin: provides more uniform and user-friendly functions than SciPy and Statsmodels
 - PyMC3: statistical modeling tool for Bayesian statistical modeling & Probabilistic Machine Learning which focuses on advanced Markov chain Monte Carlo and variational fitting algorithms
 - ppscore: Predictive Power Score (PPS) replacement for corelation to detect relationships using decision trees ML model from sklearn internally
 - bayesian-histograms: for estimation of binary rare event rates, with fully automated bin pruning
 - DoWhy: An end-to-end library for causal inference

Time Series:
 - timesynth: Multipurpose Library for Synthetic Time Series Generation in Python
 - pmdarima: wraps statsmodels, contains auto.arima functionality like R and provides scikit-learn like API
     - statsmodels: for statistical models and unit tests
 - stumpy: scalable library that efficiently computes something called the matrix profile, which can be used for a variety of time series data mining tasks such as patterns / anomaly detection
 - dtw-python: Dynamic time warping to fit data to time series by finding minimum distance between the series
 - PyFlux: time series model library for Python
 - sktime: machine learning toolbox for time series forecasting
 - darts: easy manipulation and forecasting of time series from ARIMA to Prophet, Torch models
 - kats: one stop timeseries forecast and manipulation library from facebook
    - prophet: timeseries forecasting model from facebook
 - greykite: fast, intuitive, flexible forecasting model from linkedin
 - merlion: end-to-end machine learning framework that includes loading and transforming data, building and training models, post-processing model outputs, and evaluating model performance
 - auto_ts: Automatically build ARIMA, SARIMAX, VAR, FB Prophet, XGBoost and SKLearn Models on time series
 - nixtla: Automated time series processing and forecasting
 - etna: easy-to-use time series forecasting framework for preprocessing, feature generation and smart backtesting with unified interface
 - orbit: Bayesian time series modeling and inference with a familiar and intuitive initialize-fit-predict interface utilizing probabilistic programing languages under the hood
 - gluon-ts: Probabilistic Time Series Modeling in Python
 - tsfresh: Time Series Feature extraction based on scalable hypothesis tests automatically
 - pastas: simple framework for processing, simulating, and analyzing of hydrological time series
 - flow-forecast: Deep learning PyTorch library for time series forecasting, classification, and anomaly detection (originally for flood forecasting)

Natural / Applied Sciences:
 - pint: Python units library
 - forallpeople: Python SI units library: your 'daily driver' for calculations
 - scipy: module with many scientific fuctions and constants
 - biopython: package for bioinformatics
 - astropy: library for astronomy

Econometrics:
 - EconML: combine state-of-the-art machine learning techniques with econometrics to bring automation to complex causal inference problems (estimating heterogeneous treatment effects from observational data)

## Data Science

 - Pyodide: Python with the scientific stack, compiled to WebAssembly

Project Folder Structure Skeleton:
 - cookiecutter / ccds: folder structure for datascience
 - PyScaffold: tool for bootstrapping high quality Python packages, ready to be shared on PyPI and installable via pip
    - pyscaffoldext-dsproject: extension for datascience projects

Process / Best Practices:
 - recommenders: Best Practices on Recommendation Systems

Data Cleaning:
 - missingno: Missing data visualisation in pandas
 - dplython: dyplr R equivalent for summarizing
 - fuzzywuzzy: fuzzy data matching
 - pyjanitor: Clean APIs for data cleaning. Python implementation of R package Janitor
 - datacleaner: community edition of datacleaner application
 - dora: uses scikit-learn, pandas, and Matplotlib for exploratory analysis, or more specifically, for automating the most undesirable aspects of exploratory analysis
 - scrubadub: remove personally identifiable info from free text

Data Storage:
 - hub: Dataset Format for AI with slicing, version control, compression, distribution even on cloud, apply transformations using Ray
 - fds: fast data science is a transparent wrapper on dvc and git
    - dvc: Data version control. Git for data
 - pytables: Data storage for df from within pandas
 - pystore: Data storage for df from within pandas

Data Transformation / Piplines / ETL:
 - dagster: data orchestrator for machine learning, analytics, and ETL
 - Orchest: visual orchestration tool for ETL, parametrisation with jupyterlab interface
 - Prefect: workflow management system, designed for modern infrastructure for data science
 - hamilton: create dataframes from functions
 - dataprep: lets you prepare your data using a single library with a few lines of code

EDA libraries:
 - pandas-profiling: EDA support for pandas dataframe
 - pandera: data validation rules encoded in schema for quick validation
 - skimpy: light weight tool that provides summary statistics about variables in data frames within the console
 - Flenser: simple automated data exploration tool that runs tests on dataset and provides summary
 - data-describe: toolkit for Exploratory Data Analysis (EDA). It aims to accelerate data exploration and analysis by providing automated and opinionated analysis widgets
 - lux: API for Intelligent Visual Data Discovery based on Altair
 - sweetviz: target analysis, comparison, feature analysis, correlation, visualisation in two lines of code
 - edatk: Exploratory Data Analysis Toolkit (in development)

Pandas:
 - bamboolib: GUI for pandas
 - pandas-gui: GUI for pandas
 - dtale: Visualizer for pandas data structures
 - sidetable: Create Simple Summary Tables in Pandas
 - staircase: data analysis package based on mathematical step functions based on pandas

Pandas Alternatives:
 - datatable: h2oai's bigdata library based on extremely fast data.table from R
 - polars: fast, multi-threaded DataFrames library implemented in Rust using Apache Arrow as memory model
 - Vaex: lazy out-of-core dataframes with multi-threading
 - StaticFrame: a consistent interface for working with datafames alternative to pandas
 - RAPIDS: drop in replacement library for pandas to speed up data science analysis optimised CUDA (Nvidia) - better than pandas with GPU
 - Dask: build on top of pandas to parallelize it, slower will non parallel
 - Modin: Drop in replacement for pandas to speed up common timeconsuming task by parellelising code using Ray or Dask
 - Koalas: based on spark engine

Plotting Meta Package:
 - Holoviz: High-level tools to simplify visualization in Python

Plotting:
 https://pyviz.org/tools
 https://www.python-graph-gallery.com/
 - zengl: high-performance, simple rendering with OpenGL
 - bashplotlib: plot graphs in the console
 - bqplot: interactive 2-D visualization system for Jupyter, based on the constructs of the Grammar of Graphics
 - Plotnine: ggplot2 inspired plotting library
 - Altair: Vega based Plotly alternative
 - gleam: interactive web visualisations
 - Pygal: SVG Plots
 - Plotly: Web plots
 - Ggplot: based on R ggplot
 - pyecharts: echarts libary for python
 - chartify: charting package based on bokeh with consistent interface making it easy for data scientists
 - Pandas-Bokeh: Bokeh plotting backend for Pandas, GeoPandas and Pyspark DataFrames
 - CMasher: a collection of scientific colormaps and utility functions
 - pyUpSet: Creating UpSet plots in Python but old and poor documentation

Matplotlib:
 - https://matplotlib.org/mpl-third-party/
 - proplot: matplotlib wrapper for a consistent interface for all kinds of maps and quick settings
 - seaborn: declerative api for mathplotlib designed for dataframes
 - Dexplot: simple and intuitive user experience for mathplotlib
 - mplfinance: plotting financial data such as stocks
 - mpl_interactions: interactive Matplotlib plots with any backend
     - ipympl: plugin to enable mpl interactivity in Jupyter with ipywidgets
 - blume: replacement for the matplotlib table module
 - python-ternary: Ternary graph plotting library for matplotlib
 - mpl_sankey: simpler interface for basic sankey charts compared to matplotlib.sankey
 - highlight_text: functions to plot text with <highlighted substrings> in matplotlib
 - flexitext: draw text with multiple styles in Matplotlib like ggtext
 - adjustText: Automatically adjust labels to minimize overlap
 - descartes: Use Shapely or GeoJSON-like geometric objects as matplotlib paths and patches
 - upsetplot: Another implementation of UpSet plots
 - pywaffle: Waffle Charts and pictograms
 - ahlive: animate data
 - bar_chart_race: Bar chart race animation

Spatial / Geographical:
 Wheels for mapping libraries: https://www.lfd.uci.edu/~gohlke/pythonlibs/
 Binaries: https://download.osgeo.org/osgeo4w/
 - pyproj: Python interface to PROJ (cartographic projections and coordinate transformations library)
    - basemap: mpl_toolkits submodule for plotting on maps based on numpy and pyproj (PROJ.4 from OSGeo)
 - cartopy: geospatial data processing in order to produce maps and other geospatial data analyses (PROJ.4, GEOS)
 - pyshp: reading ESRI shapefiles in pure Python
    - geoplotlib: visualizing geographical data on OSM tiles based on numpy and pyglet OpenGL backend (stalled)
 - fiona: Fast reading of shapefiles based on GDAL/OGR
 - rasterio: reads and writes GeoTIFF and other raster GIS formats and provides a Python API based on Numpy N-dimensional arrays and GeoJSON using GDAL for conversion
 - contextily: retrieve tile maps from the internet and add as basemap to mpl figures or write tile maps to disk into geospatial raster files
 - shapely: manipulation and analysis of planar geometry objects
    - descartes: Use Shapely or GeoJSON-like geometric objects as matplotlib paths and patches
    - prettymaps: Draw Pretty Maps From OpenStreetMap Data built on matplotlib
    - cartopy: makes use of PROJ.4, NumPy and Shapely to provide a interface built on top of Matplotlib
        - geoplot: built on top of cartopy and mpl aim to be seaborn for cartopy
 - netCDF4: library to read netcdf geographic data format
 - xarray: Array manipulation library based for netCDF data models and Common Data Model (CDM)
 - iris: powerful, format-agnostic, community-driven Python package for analysing and visualising Earth science data
 - geopandas: High level library using numpy, pandas, cartopy, fiona etc to make maps
    - movingpandas: handling movement data based on Pandas, GeoPandas, and HoloViz
 - geemap: Google Earth Engine API
 - leafmap: geemap alternative based on folium and ipyleaflet
 - nominatim: API to search OSM data by name and address and to generate synthetic addresses of OSM points (reverse geocoding) without signup
 - xyzservices - repository of available XYZ services offering raster basemap tiles
 - pyrosm: parsing OpenStreetMap data
 - geopy: client for several popular geocoding web services
 - geocoder: Simple and consistent geocoding library
 - OSMnx: download geospatial data from OpenStreetMap and model, project, visualize, and analyze real-world street networks and any other geospatial geometrie built on top of NetworkX, GeoPandas and matplotlib
 - pygmt: python API for Generic Mapping Tools - processing geospatial and geophysical data and making publication quality maps and figures

Graphs:
 - NetworkX, igraph - Graph analysis
 - nxviz: Graph Visualiation
 - Pydot: graph plotting
    - Graphviz – underlying for pydot

Dashboards:
 - datapane: upload and share interactive plot made from any plotting library as reports
 - Dash: based on Plotly
 - Bowtie
 - Panel: built on top of bokeh
    - Bokeh: JS charting package

IPython / Jupyter / Notebooks:
 - codebraid: live code in Pandoc Markdown which can be executed and converted to any format; depends on Pandoc
 - jupyterlite: JupyterLab distribution that runs entirely in the browser based on Pyodide
 - IPython.core.display: support for various formats to be displayed in the output
 - ipycanvas: lightweight, fast and stable library exposing the browser's Canvas API to IPython
 - nblint: pylint for notebooks
 - nb_black: Black code formatting for notebooks
 - nbdime: provides tools for diffing and merging of Jupyter Notebooks
    - nbdiff: compare notebooks in a terminal-friendly way
    - nbmerge: three-way merge of notebooks with automatic conflict resolution
    - nbdiff-web: shows you a rich rendered diff of notebooks
    - nbmerge-web: gives you a web-based three-way merge tool for notebooks
    - nbshow: present a single notebook in a terminal-friendly way
 - nbterm: simple notebook for terminal
 - nbstripout: strip output from Jupyter and IPython notebooks
 - nbconvert: Convert Notebooks to other formats pdf, static presentations based on reveal.js (part of jupyter)
    - dejavu: create presentations with widgets which are non-interactive (included in >=nbconvert6.2)
 - rise: reveal.js based presentation for live notebooks with interactivity based on reveal.js for classic notebooks
 - voila: jupyter notebook dashboards based on ipywidgets
 - nbinteract: Convert notbooks with widgets to run on remote binder server with full interactivity
 - jupytext: code is saved in a specified format (py, md, Rst etc.) and is synced to ipynb on load
 - nbdev: allows you to develop a python library in Jupyter Notebooks with features such as debugging, refactoring, writing tests, create docs, publish packages etc.
 - jupyter-notify: notification when long running notebooks finish running
 - xeus-python: ipykernel alternative for jupyter
 - ipywidgets: adds interactivity to jupyter notebooks
    - ipympl:  enables the interactive features of matplotlib in the Jupyter notebook and in JupyterLab using Jupyter interactive widgets (%matplotlib widget)
 - ipydatagrid: Fast Datagrid widget with multiple features
 - papermill: parametrizing jupyter notebooks so the notebook can be run for different values and also build workflow based on results of the notebook
 - testbook: passess code from a notebook to a testing file to be used with any testing module
 - bqplot: interactive 2-D visualization system for Jupyter, based on the constructs of the Grammar of Graphics
 - powerbi-jupyter: IPyWidget that enables customers to use PowerBI embedding capabilities in a Jupyter notebook seamlessly
 - ipython-sql: load sql into IPython magic for IPython, hopefully evolving into full SQL client

### Finance:

Data:
 - yfinance: Yahoo finance API
 - yahooquery: Yahoo finance API unofficial
 - quantel: API for many international and NSE data
 - nsepy: API for nse including CLI depends on numpy and pandas

Charts:
 - mplfinance: matplotlib finance API for plotting stocks

Technical Analysis:
 - talib: Technical Analysis
 - pandas-ta: Technical Analysis Indicators - Pandas TA is an easy to usePandas Extension with 120+ Indicators
 - finta: Common financial technical indicators implemented in Pandas

Strategies:
 - Backtrader: Backtesting
 - backtesting.py
 - Zipline: Backtesting
 - orats: US options analysis API

Fundamental Analysis:
 - numpy-financial: collection of elementary financial functions for numpy which were removed from numpy
 - opstrat: option pricing and plotting
 - mibian: Options Pricing models

AI/ML:
 - mlfinlab: machine learning for finance

Portfolio Management / Testing:
 - Empyrial: Portfolio Management Framework for risk and performance analysis
 - quantstats: analytics for quants with stats, plots and reports
 - Qlib: AI-oriented quantitative investment platform for testing training executing tracking algos & strategies from Microsoft
 - Pyfolio: To check portfolio perf metrics

Personal Finance:
 - beancount: Personal account keeping in python rewrite of core to C++ in v3
    - bean-query: Querying beancount ledger with SQL like syntax
    - Fava: Flask based dashboard for beancount ledger

### AI / ML:

Machine Learning Tools:
 - mlfinlab: machine learning for finance
 - yellowbrick: suite of visual analysis and diagnostic tools designed to facilitate machine learning with scikit-learn
 - https://iancovert.com/blog/understanding-shap-sage/
 - https://www.aidancooper.co.uk/a-non-technical-guide-to-interpreting-shap-analyses/
 - SAGE:
 - SHAP: (SHapley Additive exPlanations) is a game theoretic approach to explain the output of any machine learning model by answering how much does each feature contribute to an individual prediction
    - Shapash: provides several types of visualization of ML models that display explicit labels that everyone can understand based on shap backend
 - eli5: used to inspect ML classifiers and explain their predictions, used to debug algorithms such as sklearn regressors and classifiers, XGBoost, CatBoost, Keras, etc
 - Fairlearn: assess a AI/ML systems fairness
 - alibi: machine learning model inspection and interpretation for classification and regression models
 - eli5: explainability and debugging of ML models
 - optuna: automatic hyperparameter optimization software framework, particularly designed for machine learning
 - hyperopt: Distributed Asynchronous Hyper-parameter Optimization with Bayesian optimization for speed up
 - Hummingbird: compile trained traditional ML models into tensor computations PyTorch
 - dirty_cat: facilitates machine-learning on non-curated categories: robust to morphological variants, such as typos

MLOps:
 - Feast: an operational data system for managing and serving machine learning features to models in production
 - modelkit: minimalist yet powerful MLOps library for Python, built for people who want to deploy ML models to production

Machine Learning Wrapper Libraries / AutoML:
 - pycaret: low-code machine learning library that automates workflows and hyperparameter tuning
 - jax: Composable transformations of Python+NumPy programs: differentiate, vectorize, JIT to GPU/TPU, and more
 - lore: ML pipeline framework by Instacart
 - shogun: machine learning toolbox written in C++ available for multiple languages
 - flaml: finds accurate machine learning models automatically, efficiently and economically. It frees users from selecting learners and hyperparameters for each learner.
 - Libra: automates the end-to-end machine learning process in just one line of code. It is built for both non-technical users and software professionals of all kinds.
 - LazyPredict: help build a lot of basic models without much code and helps understand which models works better without any parameter tuning
 - PyGAD: library for Building the Genetic Algorithm and Training Machine Learning Algoithms (Keras & PyTorch).
 - ludwig: toolbox that allows to train and evaluate deep learning models without the need to write code
 - metaflow: provides a unified API to the infrastructure stack that is required to execute data science projects
 - mljar-supervised: Automated Machine Learning Pipeline with Feature Engineering and Hyper-Parameters Tuning
 - imbalanced-learn: offers a number of re-sampling techniques commonly used in datasets showing strong between-class imbalance

Machine Learning Frameworks:
 - scikit-learn: algorithms of machine learning and data mining tasks
 - PyGBM: Gradient Boosting Decision Trees
 - XGBoost/LightGBM/CatBoost: optimised, scalable and fast implementations of gradient
 - GeoBoost: Lyft GBM library with customer splits features but slower
 - keras: makes deep learning easier to learn with a simpler api and clear error messages
    - TensorFlow - framework for deep neural networks by Google
 - PyTorch: Performs tensor computations with GPU acceleration, create dynamic computational graphs and automatically calculate gradients
 - fastai: simplified neural net training with best practices with out of the box support for many types of ML
 - H20: AI library

NLP:
 - textblob: simple NLP API on NLTK and pattern3
    - pattern3: web data mining library with web mining from google, twitter, wikipedia, web crawler, NLP, machine learning and network analysis for textual data
    - NLTK: Oldest NLP
 - SpaCy: New NLP
 - Gensim: robust semantic analysis, topic modeling and vector-space modelling
 - nlp: lightweight and extensible library to easily share and access datasets and evaluation metrics for Natural Language Processing (NLP) based on tensorflow dataset tfds
 - transformers: State-of-the-art Natural Language Processing including GPT2 huggingface

Image Processing / Character Recognition (OCR) / Image Recognition / Computer Vision:
 - scikit-image: collection of algorithms for image processing
 - pytesseract: Tesarract 4 python bindings
 - imageio: image manipulation library depends on numpy and pillow
    - pillow: maintained version of PIL, for working with images
 - imutils: image maniputlation utilities
 - opencv-contrib:
    - OpenCV-Python: Open computer vision library

Audio Processing / Speech Recognition:
 - pyttsx3: Offline tts modules bundled with sapi5, nsss, espeak engines
 - SpeechRecognition: Library for performing speech recognition, with support for several engines and APIs, online and offline
 - voice2json: speech recognition, transcription, intent recognition command line tools
 - Picovoice: voice recognition library to add Alexa like feature to python apps
 - openspeech: Open-Source Toolkit for End-to-End Speech Recognition leveraging PyTorch-Lightning and Hydra
 - speechbrain: PyTorch-based Speech Toolkit for speech recognition, speaker recognition, speech enhancement, multi-microphone signal processing etc
 - librosa: music and audio analysis

## Utilities

Time and date:
 - stdlib> datetime: working with date and time
 - stdlib> calender: generate calendars for any month
 - python-dateutil: working with timezones
 - pytz: alternative to python-dateutil (has different interface compared to dateutil so dateutil is preferred)
 - arrow: offers a sensible and human-friendly approach to creating, manipulating, formatting and converting dates, times and timestamps
 - pendulum: improves API consistency over arrow
 - dateparser: Natural language date parsing, supports multiple languages
 - convertdate: convert date between various calendar and holiday list
 - holidays: holiday list

Graphics:
 - stdlib> turtle: draw shapes with code
 - youtube-dl: download vidoes from multple sites
 - manim: create animations with python scripts

Audio:
 - pyFLAC: Real-time lossless audio compression in Python based on Soundfile which in turn is based on libsndfile, CFFI and numpy
 - Pedalboard: Spotify’s Audio Effects Library for Python

Convenience:
 - Tenacity: maintained fork of `retrying` which retries a fn with custom exception actions
 - humanize: create easily readable text conversion of large numbers

Uncategorised:
 - uuid: quick and easy way to generate Universally Unique IDs
 - polling2: library for polling any repetitive function
 - gdb: python module for GDB scripting
 - zipfly: writing large ZIP archives without memory inflation

## Apps
 - HTTPie: command-line HTTP client to make CLI interaction with web services as human-friendly as possible alternative to curl
 - ChatterBot: ML based python chatbot
 - JSMon: JavaScript Change Monitor for BugBounty
 - Ciphey: automated decryption tool. Input encrypted text, get the decrypted text back
 - byob: Python based botnet
 - xidel: command line web scraper analogous to CURL for HTTP
 - webify: Turn functions and commands into web services
 - ngrap: app tunneling https://ngrok.com/
 - jprq: ngrok alternative
 - netlify: ngrok alternative
 - glitch: integrated code and app hosting
 - pywhat: `what` wrapper to identify any data such as email, domains etc in pcap or text files
 - recoverypy: search and recover blocks in block devices transparent to overwritten files
 - novelWriter: Cross-Platform Editor Designed for Writing Novels Built With Python and Qt
 - REDLI: allows you to see the complete path a redirected URL goes through
 - mvt: mobile verification toolkit for forensic analysis of phones by Amnesty Security Labs
 - prometheus: home monitoring, alerting and time series database
