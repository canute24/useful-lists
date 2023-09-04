# Useful Python Modules

As Python usage across different applications increases and huge number of modules with a similar objective but different ideology / features are introduced, a list of propular / useful modules for quick reference helps a lot.

The main categorisation is between python apps in the traiditonal sense vs the more recent but rapidly growing data science ecosystem. While the common sections seperated out.

Other Similar Collations
 - https://github.com/vinta/awesome-python/
 - https://github.com/ml-tooling/best-of-web-python
 - https://github.com/florimondmanca/awesome-asgi
 - https://www.libhunt.com/
 - https://libraries.io/
 - http://svaksha.github.io/pythonidae/

Cheatsheets:
 - https://nedbatchelder.com/text/which-py.html
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
 - stdlib> tempfile: os specific temp paths
 - stdlib> glob: glob operator for files as python list
   - glob2: capture patterns and supports recursive wildcards
 - stdlib> webbrowser: Convenient Web-browser controller
 - stdlib> mmap: map disk to memory to read large files without completely loading them to RAM
 - atomicwrites: write to filesystem atomically
 - platformdirs: determining appropriate platform-specific dirs
 - watchdog: python API and commandline to monitor file system events and perform custom actions
 - fileless-elf-exec: Execute ELF files without dropping them on disk directly from memory
 - sh: full-fledged subprocess replacement that allows you to call any program as if it were a function
 - WinSys: Python tools for the Windows Administrator
 - pyperclip: clipboard access
 - win32clipboard: part of win32api
 - pywin32: provides access to many of the Windows APIs from Python
   - win32com: Windows COM object and client
   - win32api: Windows system calls
 - py-filelock: platform independent file lock that supports the with-statement
 - setproctitle: allows a process to change its title (as displayed by system tools such as ps, top after forking

Unique ID:
 - uuid: quick and easy way to generate Universally Unique IDs
 - ulid: create lexically dated unique identifiers with metadata support and variable string lengths among others
 - nanoid: unique ids which are smaller than uuid and very fast with character set customisation support

Interoperability:
 - reticulate: tools for interoperability between Python and R in R
 - rpy/rpy2: calling R from python
 - compatlib: Python utilities for writing cross-version compatible libraries
 - pybind11: C++/python bindings with full C++ coverage
 - nanobind: same as above with limited C++ coverage to make it faster
 - gopy: compiles and generates a CPython extension module from a Go package which can then be used in Python
 - pyopy: interesting matlab/octave libraries in python requires octave/python

Text Processing:
 - stdlib> string: convenience functions for text such as templates strings
 - stdlib> re: regex library
 - stdlib> difflib: library for comparison and identify difference between patterns with many helpful methods
 - stdlib> tomlib: TOML parser (=>3.11)
 - stdlib> codecs: library for transcoding various formats
   - codext: codecs extension featuring CLI tools for encoding/decoding anything including languages, hash, encryption, morse code and more
 - stream_unzip: steam data from zip files instead of reading / loading the entire file
 - chardet: for detecting character set for a file
 - unidecode: convert unicode strings to ASCII for backward compatibility with legacy systems
 - emoji: Unicode emoji conversion
 - emot: library to convert emojis to text with meaning
 - humre: human readable regexes
 - textract: Text extraction from variety of document and images
 - texthero: Text preprocessing, representation and visualization
 - flashtext: Fast full word replacement
 - parse: Parse strings using a specification based on the Python format() syntax
 - numerizer: convert spelled numbers to real numbers
 - humanize: create easily readable text conversion of large numbers
 - cogapp: lets you use pieces of Python code as generators in your source files to generate whatever text you need
 - english-words: collections of english word categorised with filter methods
 - quarto: A scientific and technical publishing system built on Pandoc using markdown
   - pandoc: commandline tool to convert documents from many different formats
 - python-markdown: python implementation of John Grubers markdown
 - docx2txt: extract text from MSWord docx format
 - catdoc: extract text from MSWord doc format
 - python-docx: create and edit MSWord documents

JSON / HOCON:
 - pyhocon: Human-Optimized Config Object Notation (HOCON / JSON superset) parser / converter into JSON, YAML
 - orjson: rust implementated fast, more correct JSON library than stdlib json lib which can serialize dataclass, datetime, numpy, and UUID instances natively
 - ujson: Extremely fast json library written in C
 - ijson: iterative JSON parser with standard Python iterator interfaces
 - json-traverse: simple JSON parser
 - JmesPath: declarative access to json elements
 - jsonpath-ng: traverse JSON elements in `.` (dot) notation (JSON notation) link in javascript
 - jpath: access lists and dicts with `.` (dot) notation like JSON with wildcard, slicing and conditionals support
 - nvelope: Define your JSON schema as Python dataclasses with custom checks and defined conversions from JSON to dict
 - jsonschema: JSON Schema validation
 - python-benedict: drop in replacement for dict with support for keylists and keypaths in dicts

XML:
 - stdlib> xml.etree.ElementTree: parse XML files
 - lxml.etree: fast and wide std support (XPath, XMLSchema, XSLT)
   - html_text: extract text from HTML
     - trafilatura: lib and cmd app to extract text from a variety of sources
 - untangle: simple library to access XML in a pythonic way depends on xml.sax and is designed for samll files; implemented in pure python
 - xmltodict: convert xml to python dict and vice versa
 - reader: retrieve, store, and manage web feeds through a high-level API, without having to deal with feed-related details
 - feedparser: parse Atom and RSS feeds
 - Python-OOXML: working with Office Open XML files >=MSOffice2013 formats

YAML:
 - PyYAML: YAML parser
 - strictyaml: Type-safe YAML parser and validator with schema for type checking and creating YAML from dicts and lists
 - yamale: schema and validator for YAML

Serialisation:
 - stdlib> pickle / cpickle: for serializing objects for storage
 - msgspec: lightweight and fast serialization and validation library, with builtin support for JSON, MessagePack, YAML, and TOML
 - cloudpickle: serialize constructs not supported by the pickle especially useful for cluster computing where code is shipped over the network to execute on remote hosts, possibly close to the data such as lambda functions along with functions and classes defined interactively
 - pyserde: inspired by serde-rs can serialize data types and objects along with typing options like Union

Data validation:
 - msgspec: lightweight and fast serialization and validation library, with builtin support for JSON, MessagePack, YAML, and TOML
 - msgpack: efficient binary serialization format for data exchange like JSON but faster and smaller
 - cerberus: powerful yet simple and lightweight data validation functionality out of the box and is designed to be easily extensible, allowing for custom validation
 - pydantic: data parsing and validation using python type hints making it easier to write classes
   - pydbantic: single model for shaping, creating, accessing, storing data within a Database
 - datashape: language defining a data description protocol
 - marshmellow: ORM/ODM/framework agonostic library for converting complex datatypes such as objects to and from Python datatypes
 - great_expectations: data validation framework
 - pandera: statistical data validation for pandas
 - pydeequ: scala based data validator with dynamic checks and anomaly detection
 - validators: simple data validation library for different data types

Datafiles / Tabular Data:
 - dataconverters: Unified python library and command line interface to convert data from one format to another (especially tabular data)
 - tablib: format agonistic tabular dataset library supporting json, csv, xls, yaml etc
 - datamatrix: light-weight library for working with tabular data  with spreadsheet-like structure that consists of named columns and numbered rows
 - rows: work with anytype of tabular data
 - csvkit: Library for working with csv files
 - comma: csv Library for Humans; python object like indexing and manipulation
   - clevercsv: drop-in replacement for the Python csv package with improved dialect detection for messy CSV files and a handy command line tool that can standardize a messy file or generate Python code to import it
 - lazycsv: a memory-efficient csv parser implemented in C
 - csvcubed: convert any data to open consistently formatted CSV-W data files
 - gptables: Good Practice Tables for converting any dataframe to GPTables
 - pyarrow: arrow bindings for python
   - fastparquet: read and write parquet file

Documentation:
 - docutils: convert rst to any other rich text markup
   - sphinx: Docs generator
 - mkdocs: static site generator for documentation
   - mkdocstrings: Automatic documentation from sources, for MkDocs
 - pycco: port of Docco which generates simple docs from code
 - rst2pdf: creates PDF documents from your ReStructured Text markup

PDFs:
 - pText: pure python pdf manipulation as a JSON like structure support read and editing
 - fpdf2: minimalist PDF creation library successor to PyFPDF
 - Pypdf2: for working with pdf’s
 - ReportLab: for creating PDFs programmatically
 - PDFx: extract data, links and metadata from pdfs as CLI or library
 - PyPDFParser: Visualize and extract structured data from PDF files
 - pdfminer: for mining pdf files
 - camelot: Extract tables from text based PDF files
 - pymupdf: high speed and feature right text and image extraction/conversion based on MuPDF library with Tesseract integration for OCR
 - tabula-py: based on tabula-java can directly extract tables to pandas

Spreadsheets:
 - openpyxl: for working with Excel 2010 format (.xlsx) excel files
 - xlsxwriter: module for creating Excel 2010 (.xlsx) files, in particular, charts
 - pyxlsb: read Excel files in the (.xlsb) format
 - xlrd: For reading older Excel (.xls) documents
 - xlwt: For writing older Excel (.xls) documents
 - formulas: interpreter for parsing and calculating Excel formulae
 - xlwings: Works with new Excel formats and has macro capabilities but depends on excel
 - PyXLL: use python instead of macros in Excel making python accessible from excel (commercial)
 - gspread: API for Google Sheets like pygsheets, ezsheets

Presentations:
 - python-pptx: create and edit Microsoft Powerpoint documents
 - gslides: Creating charts in Google slides

SQL / Databases:
 - stdlib> shelve: pickle wrapper for storing key value pairs similar to dbm
 - tinyDB: simple pure python database with a clean API that just works without lots of configuration
   - tinyflux: tinyDB for timeseries applications
 - pickledb: lightweight and simple key-value store based on simplejson inspired by Redis
 - diskcache: disk and file backed cache library with high performance based on sqlite
 - sqlitedict: persistent dict, backed by sqlite3 and pickle (for serialisation), multithread-safe
 - sqlite-utils: library and command line tool with convenience fns for working with sqlite db
 - sqlcommenter: add meta info to your SQL queries as comments which can be useful for debugging
 - Alembic: for database migration
 - peewee: a tiny ORM with limited features
 - SQLAlchemy: Most popular ORM for python
   - sqlmodel: SQL databases in Python, designed for simplicity, compatibility, and robustness based on Pydantic and SQLAlchemy made by FastAPI authour
   - ibis: Expressive analytics in Python at any scale which writes sql statements in the background to interaction with databases locally and over the web based on sqlalchemy
 - zodb: Python object-oriented database based on BTrees optimised for object traversal rather than search
 - piccolo: fast, user friendly ORM and query builder which supports asyncio
 - preql: interpreted relational query language that complies python to sql written in python
 - psycopg2: the most popular PostgreSQL database adapter for the Python
 - vinum: use SQL on python datatypes in-memory for data analytics using Postgress's pglast parser
 - duckdb: run SQL queries on many data files including on pandas dataframes
 - FugueSQL: run SQL queries on pandas, spark and dash within notebook cells
 - SQLFluff: dialect-flexible and configurable SQL linter written in python
 - SQLLineage: shows source and target tables for any SQL query for complex queries
 - CogDB: persistent graph database implemented purely in Python

Data Ecosystem:
 - dbt: data transformation within the warehouse using sofware best practices such as CI/CD, version control etc
 - blaze: set of libraries that help users store, describe, query and process data

### Network / Communication:

HTTP / TCP / UDP / Websocket:
 - pyfilesystem: filesytem abstraction works with zip, ftp, cloud, memory, etc.
 - fsspec: provides an abstract filesystem with a consistent API for various network services e.g., S3, GCP
 - mureq: Single-file alternative to python-requests with lower memory but no connection pooling
 - requests: easy to use http client based on urllib3
   - requests-cache: Caching for requests library
 - mechanize: a browser that implements the urllib2.OpenerDirector interface with state, including navigation history, HTML form state, cookies, etc based on perl's WWW::Mechanize
 - packet-sniffer: pure-Python network packet sniffer based on PF_PACKET (Linux only)
 - httpx: next generation HTTP client based on requests with async, HTTP/2 support, connection & response pooling etc
 - aiohttp: asynchronous http client
 - python-webrtc: Python extension that provides bindings to WebRTC M92

Web Scraping:
 https://pixelscan.net/
 https://httpbin.org/headers
 http://webnumbr.com/
 https://jsonplaceholder.typicode.com/
 - BeautifulSoup: parser for xml / html
 - parsel: extract and remove data from HTML and XML using XPath and CSS selectors, optionally combined with regular expressions
 - elemental: makes Selenium automation faster and easier by adding automatic waits and common missing usecases from selenium
   - Selenium – Browser automation
 - selenium-wire: give access to underlying requests made by the browser
 - mitmproxy: interactive, SSL/TLS-capable intercepting proxy with a console interface for HTTP and Websockets
   - mitmproxy2swagger: Automagically reverse-engineer REST APIs via capturing traffic
 - playwright: puppeteer devs new project after moving to microsoft for browser control similar API as puppeteer runs on NodeJS backend
 - pyppeteer: Headless chrome/chromium automation library (unofficial port of puppeteer)
 - scrapy: web crawler
 - pyspider: web crawler
 - cloudproxy: Provision proxy servers across different cloud / datacenter provider ips

Email:
 - stdlib> email: For managing email messages. With this we will setup the email message itself, including subject, body, and attachments.
 - stdlib> smtplib: Handles the SMTP connection
 - stdlib> IMAPlib: working with IMAP connections
 - redbox/redmail: easier email management and sending library

### GUI / Interface

Indicators:
 - progress / fastprogress / alive-progress / tqdm: progress bars

GUI:
 - win10toast: Notifications in windows or win10toast-click for clickable version
 - gooey: Turn (almost) any Python command line program into a full GUI application with one line based on wxpython
 - PyWebIO: simple web app interface / GUI generation in python script
 - pyvibe: create web pages or web apps from python using web components from tailwind
 - pywebview: GUI for python apps in JS, HTML and CSS
   - neutron: create webbased frontend in python to run in pywebview
 - reflex: full-stack framework that makes it easy to build and deploy web apps
 - pyrustic: framwwork for making GUI's uses tk
 - PySimpleGUI: Simple python GUI framework using tkinter, Qt, Remi or WxPython
 - PyMsgBox: simple, cross-platform, pure Python module for messageboxes
 - qtwin11: Windows 11 theme for Qt
 - edifice: makes it simple to build a fully reactive UI based on Javascript libraries such as React
 - re-wx: library for building modern declarative desktop applications in WX
 - Kivy: cross-platform framework for development of applications that make use of innovative, multi-touch user interfaces
 - Toga: Python native, OS native, cross platform GUI toolkit part of BeeWare suite
 - atlas-python: Atlas toolkit is the easiest way to add a web-based graphical user interface
 - streamlit: create beautiful, performant apps in a few hours in pure Python
 - nicegui: streamlit type simple UI with minimal config
 - gradio: deploy ML models, fns, API with UI
 - voila: GUI's from jupyter notebook based on ipywidgets
 - mercury: easily convert Python notebook to web app and share with others
 - bloxs: Display your data in an attractive way in your notebook works well with mercury
 - litemark: Lightweight Markdown dialect for Python desktop apps
 - CustomTkinter: based on Tkinter, provides new, modern and fully customizable widgets with consistent views across platforms
 - tkinterdnd2: tkinter with native drag and drop support

Terminal-UI:
 - stdlib> textwrap: display easily formatted text in console
 - curses: used to create text user interface is restricted to Unix-like systems
 - windows-curses: curses compatible module for windows
 - WConio: is a wrapper for Turbo-C’s CONIO.H, used to create text user interfaces
 - WConio2: pure python implementation of WConio
 - rich: for rendering rich text and beautiful formatting to the terminal with rich text REPL
 - survey: simple library for creating interactive prompts with simple functions and minimal dependencies
 - nurses_2: widget and async-centric terminal graphics library
 - colorama: colouring command-line text
 - tabulate: pretty print tabular data
 - prettytable: pretty print tabular data
 - py_cui: Tk like API for creating CUI/TUI interfaces with widgets, inspired by gocui
 - textual: CUI/TUI interface with widgets based on Rich module for formatting
 - blessed: TUI interface similar to textual
 - pytermgui: simple yet powerful TUI framework for your Python (3.7+) applications
 - bashplotlib: plot graphs in the console
 - plotext: plotting in terminal with matplotlib like interface
 - tplot: A library for creating text-based graphs in the terminal.

CLI:
 - stdlib> argparse: powerful but verbose, preferred over getopt/optparse which are soft deprecated
 - cliche: Build a simple command-line interface from your functions using a decorator while keeping it usage for other scripts
 - click: you need a lot of decorators to construct a CLI, and not obvious how to use it
   - typer: CLI based on type hints similar to FastAPI by FastAPI authour
   - trogon: automatic TUI based on Click CLI with just 2 lines of code based on Textual
 - python-fire: low set up, but traces all the time / design lacking, does not show default values and types by Google
 - cleo: requires too much code/objects to construct
 - docopt: Command-line interface description language

Cryptography / Hashing / Password:
 - stdlib> getpass: portable password input without echoing
 - stdlib> crypt: provides functions that could be used for password hashing dependending on your system and aren’t as strong as passlib
 - stdlib> hashlib: provides functions for file hashing
 - stdlib> secrets:
 - SecretStorage: provides a way for securely storing passwords and other secrets using D-Bus SecretService API supported by GNOME Keyring, KSecretsService and KeePassXC
 - passlib: widely used and tested hashing library with strong encryption
 - bcrypt: bcrypt hasing algo. Password storage requires multiple passes
 - hmac: used to verify integrity and authenticity of message and doesn’t have the properties required for password hashing
 - keyring: by default uses your user account login password for encryption, so it gets automatically unlocked when you login and you therefore don’t have worry about extra password
 - pycryptodome/pycryptodomex: self-contained low-level cryptographic primitives
 - itsdangerous: safely pass data to untrusted environments and back with crypto sign, timestamp and compression features

## General Programming

OS:
 - pyRTOS: RTOS written in Python
 - xonsh: shell and command prompt
 - pythonnet: python.net gives nearly seamless integration with .NET Framework, .NET Core and Mono

REPL:
 - jupyter-console: ipython like REPL for other kernels like C and Java
 - bpython: python repl with undo, autoformatting, autocomplete, highlighting in terminal
 - ptpython: REPL build on top of the prompt_toolkit library
 - prompt_toolkit: build powerful interactive command line applications in Python

Compilers / Decompilers:
 - dis: disassembiling CPython bytecode
 - numexpr: extension library for scipy which can further speed up Numpy and Pandas
 - numba: similar to numexpr
 - lpython: retargettable compiler with backends such as LLVM, C, C++, WASM, Julia and x86 with interoperability with CPython and faster than numba
 - shedskin: fastest restricted python to C++ compiler
 - pycom: Python compiler, down to native code, using C++
 - mypyc: compiles Python modules to C extensions using standard Python type hints to generate fast code
 - hpy: new API for extending Python in C with zero overhead, faster, universal binaries, nicer API and more
 - pypy: python JIT compiler
 - pyston-lite: JIT with upto 30% improvement on server benchmarks and more for simpler programs can be manually enabled using pyston_lite.enable() instead of installing pyston_lite_autoload which injects everytime unless DISABLE_PYSTON=1 is set
 - pyjion: JIT which convert code to native CIL and runs with .NET 5 CLR from Microsoft
 - cinder: python JIT complier from Instagram
 - skybison: ground up high performance version of python from Instagram
 - nutika: transpiler which converts python code to C++ to an executable
 - codon: python compiler using LLVM with speed comparable to C
 - Rusthon: multi-language tranpiler written in python
 - pythonjs: python to JS tranpiler offering upto 20X speeup on typed code
 - taichi: parallel programming language for high-performance numerical computations embedded in Python, and its just-in-time compiler offloads compute-intensive tasks to multi-core CPUs and massively parallel GPUs

Python Grammar:
 - __future__: import features implemented in newer versions of python
 - stdlib> atexit: register function to run at sys.exit() to cleanly terminate
 - operator: python operators and convenience functions such as itemgetter, attrgetter, methodcaller for sorting with key and filtering data
 - collections: additional data types and utiliy functions for container data types
 - itertools/functools - tools for using iterators and functions as functional progamming
   - more_itertools: extends itertools with more routines for operating on iterables
 - toolz (itertoolz/functoolz/distoolz) - supplementary to above which implements some missing functionality
 - functools.singledispatch (>=3.8)/singledispatchmethod(<3.8): generic function consisting of multiple functions implementing the same operation for different data types determining which implementation to run based on the type of a "single" argument
 - multipledispatch: full featured multiple dispatch
 - runtype: Utilities for simplyfying run-time type validation and multiple dispatch
 - operator: contains a large number of efficient functions corresponding to Python operators
 - ast: sytax parsing and manipulation for linting, patching, refactoring
 - astunparse: unparse changes done using `ast` module to convert to python code
 - python-goto: enable goto by rewriting the bytecode
 - copy: with copy and deepcopy methods for making copies of python objects

Environments / Dependency Management:
 - stdlib> importlib: working with modules and package resource tool (install importlib_resouces py < 3.7)
 - pyenv: shell script to manage multiple installations of python
 - virtualenvwrapper: wrapper for virtualenv tool
   - Virtualenv: parent of stdlib> venv with some additional features not available in venv
 declarative_config.html#example-setup-config
 - pydeps: read code and draw a dependency graph
 - pipdeptree: command line utility for displaying the installed python packages in form of a dependency tree
 - pipx: install end user apps in a seperate isolated virtual env available globally
 - pip-tools: version pinning and hashes to mitigate supply chain attacks
 - pip-audit: scan environments for packages with known vulnerabilities
 - pipenv: dependency management for packages and projects intergrating virtual enviornments with pip

Python Packaging / Modules:
 - twine: utility for publishing packages to PyPI and other repositories. It provides build system independent uploads of source and binary distribution artifacts for both new and existing projects
 - poetry: simplifies dependeny management for projects and packages
 - flit: tool to simplify package creation and publishing to PyPI
 - hatch: project management including enviornment management, version management and publishing to pypi
 - build: simple, correct Python build frontend maintained by PyPA

Distribution:
 - py2exe: create exe's for supported versions of python - doesn't require extraction
 - briefcase: tool for converting a Python project into a standalone native application
 - pyoxidizer: similar to py2exe runs by extracting to memory. Rust app so requires rust
 - pyinstaller: extracts to temp and runs, requires virtualenv
 - pyinstxtractor: Python script to extract the contents of a PyInstaller generated Windows executable file

Build / CI/CD tools:
 - Deprecated setup.py: https://pypa-build.readthedocs.io/en/stable/
 - setup.cfg: https://setuptools.pypa.io/en/latest/userguide/
 - pyproject.toml: https://drivendata.co/blog/python-packaging-2023
 - invoke: task execution tool and libary similar to make
 - pydoit: doit comes from the idea of bringing the power of build-tools to execute any kind of task
 - pypyr: task-runner cli & api for automation pipelines combining different scripts in different languages and apps
 - tox: task automation tool which can make venvs to run builds, tests, docs, publishing etc a complete CI/CD workflow which can also execute make commands but configuration is done in .ini file
 - nox: command-line tool that automates testing in multiple Python environments, similar to tox. Unlike tox, Nox uses a standard Python file for configuration
 - pre-commit: framework for managing and maintaining multi-language pre-commit hooks
 - pants: Pants 2 is a fast, scalable, user-friendly build system for codebases of all sizes. It's currently focused on Python, Shell, Docker, and Go.
 - bump2version: maintained fork of bumpversion tool to simplify releasing software by updating all version strings in your source code by the correct increment
 - semantic-release: automatically updates the changelog, increments the version according to a standard called Semantic Versioning, and publishes the project to PyPI
   - commitizen: guides you through the steps needed to automatically create a commit message in the format of a Conventional Commit which semantic release uses to increment the version automatically

Obfuscator / Code compactors:
 - python-minifier: Transform Python source code into it's most compact representation

Formatting / Styling:
 - teyit: Formatter for your Python unit tests specifically unittest
 - black: automatic code formatter
 - yapf: highly configurable code formatter from Google that can use multiple code styles
 - autopep8: built on pycodestyle for autoformatting code (run with double --aggressive switches)
   - pycodestyle: formally called pep8
 - pydocstyle: check doc string formatting
 - pydocstringformatter: check doc string formatting
 - ssort: Tool for sorting top level statements such as classes moved to top
 - isort: automatic import formatter
   - seed-isort-config: statically populate the known_third_party part of the .isort.cfg
 - reorder_python_imports: rewrites source to reorder python imports with the aim of simplyfying merges by putting one import per line
 - table-format: formats list of lists as a fixed width table
 - pyupgrade: tool (and pre-commit hook) to automatically upgrade syntax for newer versions of python inc fstrings
 - setup-py-upgrade: upgrade a setup.py to declarative metadata
 - flynt: command line tool to automatically convert old "%-formatted" and .format() strings into f-strings'

Refactoring:
 - Bowler: refactoring tool for manipulating Python at the syntax tree level
 - rope: refactoring library which is light on dependencies like npm which is required for PyRight/PyLance
 - vulture: find dead/unused code
 - refurb: tool for refurbishing and modernizing Python codebases suggesting code improvements

Linting:
 - ruff: extremely fast linter written in Rust
 - pylama: wrapper for multiple linters/checkers used for code audit
 - pylint: superset of flake8
   - flake8: check for errors and style wrapper on pyflakes and few other tools
     - bugbear: flake8 plugin which catches additional bugs and runs on multiple cores
     - autoflake: removes unused imports of stdlib and unused variables reported by pyflakes
       - pyflakes: A simple program which checks Python source files for error
     - mccabe: code complexity checker
     - pycodestyle: formally called pep8
   - pyreverse: intergrated into pylint to allow generating class diagrams from code
 - pygrep: Find python identifiers in code files where they are imported
 - slotscheck: Find mistakes in your __slots__ definitions
 - Pyroma: packing linter point out issues related to packaging your code for distribution on PyPI with properly formatted descriptions, versions, and meta data fields
 - bandit: find common security issues in Python code
 - radon: remove dead code based on mccabe
 - vulture: remove dead code
 - eradicate: remove dead code

Type Checking (static):
 - stdlib> typing: type hinting and annotations with modern IDE's
 - typing_extensions: Enable use of new type system features on older Python versions
 - pyannotate: insert annotations into your source code based on call arguments and return types observed at runtime
 - autotyping: tool to add type hints for various cases
 - MonkeyType: collects runtime types of function arguments and return values, and can automatically generate stub files or even add draft type annotations directly to your code by Instagram
 - pytype: checks and infers types without requiring type annotations
 - mypy: optional static type checker
 - pytype: checks and infers types for your Python code - without requiring type annotations also support cross function inference which is not available with mypy and also allows runtime lenience compared to mypy(windows support pending) (Google)
 - pyre: static type checker (Facebook)
 - pyright: static type checker (Microsoft) has external dependencies
 - pylyzer: static code analyzer & language server which is 100x faster than others. It  uses the type checker of the Erg programming language internally.
 - attrs: creating dataclasses with less boilerplate based on type hints on which stdlib dataclasses is based on

Dynamic Type Checking:
 - enforce
 - typeguard
 - typo
 - ducktype
 - strictconf
 - pytypes

Logging:
 - structlog: structured logging library
 - loguru: easily configurable logging library with debugging info in log
 - picologging: drop-in replacement for stdlib>logging high-performance (4-10x) logging library for Python

Debugging:
 - stdlib> print statement: f"{hello=}" # >=python3.8
 - konsole: Readable, pleasing console output with colours and easy setup built on logging library
 - objexplore: terminal UI to inspect and explore Python objects
 - objprint: print Python objects in human readable format
 - invectio: gather symbols provided or library calls and attribute usage based on static analysis of sources of Python applications
 - icecream: pretty print and easily managable print function for debugging
 - watchpoints: prints watched variables whenever its value changes and can even trigger pdb
 - PySnooper: poor mans debugger, prints every variable change
 - pdbpp: debugger based on pdb with many convenient features
 - pudb: text GUI debugger
 - ipdb: IPython debugger
 - debugpy: implementation of the Debug Adapter Protocol for Python by Microsoft
 - border_patrol: logs all imports and versions
 - pycrunch-trace: debugging and time travel from pytrace.com
 - jurigged: hotpatching code while script is being run when files is modified and saved
 - pyrasite: Inject code into running Python processes
 - pystack: Inspired by pyrasite, pstack, allows stack analysis for python running/crashed process by Bloomberg
 - cyberbrain: Backtraces variable change, See every state of program execution, including variables' values

Traceback:
 - stdlib> sys.settrace and sys.setprofile
 - friendly_traceback: clearer traceback messages
 - traceback_with_variables: Adds variables to python traceback, colouring or to file log
 - rich.traceback: formatted traceback module in rich
 - IPython.core.ultratb: traceback module used by IPython
 - stackprinter: ultratb like tracebacks
 - frosch: runtime error debugger with formatted last line with variable list

Profiling:
 - stdlib> time python <script_name.py>
 - stdlib> python -m timeit -s <setup_code> <script_name.py> # setup_code will not be included in benchmark
 - stdlib> python -X importtime -S <script_name.py> # -S This will “disable the import of the module site and the site-dependent manipulations of sys.path that it entails” hence non-stdlib imports may fail
 - stdlib> tracemalloc: tracks every individual memory blocks allocated by the Python interpreter (30% perf hit)
 - stdlib> resource: provides basic controls for resources that a program allocates (point in time reporting needs more code for running another monitoring thread for profiling multiple points but imprecise if sampling duration is too long)
 - stdlib> pstats: cProfiler data analysis class with analysis methods
 - stdlib> cProfile: function profiler part of stdlib
 - hyperfine: not a module but can be good to get objective benchmarks for python apps or any other program
 - pyperf: similar syntax to timeit but with much better features subcommands for analysing results defacto std for benchmarks used by PSF
 - line_profiler: profile the time each individual line takes to execute
 - memory_profiler: monitoring memory consumption in a process or you can use it for a line-by-line analysis of the memory consumption. psutil (optional requirement) significantly improves its performance
 - memray: live memory profiler similar to top
 - profilehooks: multiple profiling options
 - QuickPotato: create automated tests for profiling performance
 - pyinstrument: online profiler
 - VizTracer: traces concurrent python programs and also helps in debugging
 - palanteer: High performance visual profiler, debugger, tests enabler for C++ and Python
 - scalene: a high-performance, high-precision CPU, GPU, and memory profiler and find bottlenecks in data too
 - jetfuel: performance profiler that only profiles required sections, makes results easy to aggregate and search through
 - reloadium: hot reloading and profiling of functions for web frameworks, data analytics and other libraries

Caching:
 - functools> @lru_cache: caching recent calculations
 - functools> @cache: lru_cache enhancement (>=python3.9.2)
 - functools> @cached_property: prevent recalculation of a class method if same args are provided (>=python3.8)
 - pylibmc: Python client for memcached written in C

RPA:
 - mouse: monitor and control mouse
 - keyboard: monitor and control keyboard, with features such as callback, hotkeys, macro recording and playback etc.
 - rpa: RPA package for python
 - pynput: Monitor and control input devices like KB and Mouse used for interceptors and keyloggers
 - pyautogui: GUI automation
 - pywinauto: set of python modules to automate the GUI on Windows and Linux
 - mouseinfo: display XY position and RGB color information for the pixel currently under the mouse
 - pygetwindow: cross-platform module for obtaining GUI information on application's windows
 - robotframework: RPA language implemented in python

Configuration Management:
 - python-decouple: full featured config module initially designed for django compatible with ini and env with auto type casting, default config, config overiding etc
 - stdlib> configparser: for working with ini files
 - configupdater: complements configparser with ability to selectively update .ini files
 - environs: enviornment variable loading and easy parsing
 - python-dotenv: Reads the key-value pair from .env file and adds them to environment variable. It is great for managing app settings during development and in production using 12-factor principles
 - Dynaconf: can read most config formats
 - Hydra: dynamically create hierarchial config and overide with command line options and save each session into a custom config

Testing:
 - stdlib> unittest: First unit testing framework of the std library
 - stdlib> doctest: test generation based on output from shell interpreter
 - Coverage.py: tool that check testing code coverage of source
 - slipcover: Near Zero-Overhead Python Code Coverage Tracking
 - nose: Extends unit testing for other packages
 - pytest: easy to write small tests, parametric tests, scales to support complex functional testing for applications and libraries
   - pytest-rich: Leverage rich for richer test session output
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
 - pydags: creation and running of lightweight DAG-based workloads locally based on Redis and GraphiViz alternate to technologies like Airflow, Kubeflow, and Luigi are more heavyweight, enterprise-level workflow manager

Task Queue / Message Queue / Scheduling:
 - dramatiq: background task processing library for Python with a focus on simplicity, reliability and performance
 - celery: Task queues used as a mechanism to distribute work across threads or machines
 - pika: pure-Python implementation of the AMQP 0-9-1 protocol including RabbitMQ’s extensions
 - huey: little task queue based on redis, sqlite, file-system, or in-memory storage
 - APScheduler: very advanced scheduler
 - sched: simple scheduler
 - python-crontab: uses os specific scheduler in the background
 - schedule: declarative scheduler similar to crontab, easier syntax
 - rocketry: modern, simple, clean and extensive scheduling framework for Python applications

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
 - pathos: framework for heterogeneous computing
   - p_tqdm: distributed computing wrapper based on pathos
   - klepto: extends lru_cache with different algorithms (MRU, LFU) and long term storage

### Android / Mobile phone

 - python-adb: pure-python implementation of the ADB and Fastboot protocols, without using daemon between the client and the device, and therefore does not support multiple simultaneous commands to the same device using libusb1 and not official Google product.
 - adb_shell: originated from python-adb; implements ADB shell and FileSync functionality
 - ppadb: pure python implementation of adb client which interfaces with the adb server on PC
 - mtkclient: unofficial MTK reverse engineering and flash tool
 - flet: Build flutter apps in python and deploy to any platform

### Electronics

Design:
 - pinout: method to create pin-out diagrams for electronic hardware with SVG diagram creation
 - nmigen: toolbox for building complex digital hardware alternative to Verilog, VHDL

Hardware Interface:
 - coolterm: module to automate coolterm - a serial monitor app
 - pyserial: python library for interacting with serial port over a variety of different devices: old-style serial ports, Bluetooth dongles, infra-red ports etc
 - PyUSB: access USB devices; relies on a native system library
 - USPP: access serial portsv which only works in Windows for now

Micropython:
 - micropython: python for microcontrollers
 - pycopy: minimalist and memory-efficient Python dialect which works on microcontrollers but in beta
 - belay: enables the rapid development of projects that interact witg a micropython-compatible board from a PC running python through some connection
 - microdot: minimalist web framework inspired by flask which can run on low end systems including micropython

Graphics:
 - lvgl: Light and Versatile Graphics Library for microcontrollers with micropython bindings

### Web Programming

Webscripting:
 - Brython: run python in place of javascript in the frontend
 - pyscript: python replacement for javascript based on pyodide and WASM
 - pythonmonkey: Mozilla Spidermonkey JS engine embedded python VM

HTML / Web page generation:
 - mako: templating engine
 - jinja2: templating engine
 - genshi: templating engine for HTML, XML and plain text
 - nikola: static site generator
 - pelican: static site generator
 - flask-flatpages: markdown supported static website creation https://www.jamesharding.ca/posts/simple-static-markdown-blog-in-flask/
 - pygments: python sytax highlighter for webpages
 - fastpages: github pages like static site generator from many different document formats
 - esparto: Create webpages to display data and outputs using bootstrap and jinja2
 - lektor: python based flat file CMS
 - reactpy: react web framework only using python

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
 - snscrape: scraper for social networking services (SNS). It scrapes things like user profiles, hashtags, or searches and returns the discovered items
 - apify-sdk-python: access apify store with pre-made automation scripts for extracting data from the web
 - twitter-scraper: Twitter frontend (JavaScript) has it's own API, reverse–engineered. No API rate limits. No restrictions. Extremely fast
 - facebook-scraper: similar to twitter-scraper to scrape data without API
 - mastodon.py: wrapper for mastodon API
 - toot: CLI and TUI tool for posting text and media to the timeline, searching, following, muting and blocking accounts and other actions with Mastodon instances from the command line
 - python-telegram-bot: telegram bot wrapper
 - Telethon: Telegram bot library
 - InstaPy: Instagram selenium bot
 - pytrends: unofficial google trends api scraped from trends site
 - google-api-python-client: google api client
 - google-auth-httplib2 / google-auth-oauthlib: required for authentication
 - google-workspace: unofficial high level Python API wrapper for some of the productivity based Google APIs, that is focused on simplicity
 - simple-youtube-api: Youtube API wrapper for python, making it easier to search and upload your videos and requires google API keys
 - newspaper3k: data from 1000's of newspapers with metadata
 - pygooglenews: A python wrapper of the Google News RSS feed
 - wikipedia: wikipedia API
 - wikipedia_ql: Query language for efficient data extraction from Wikipedia
 - wikitextparser: simple to use WikiText parsing library for MediaWiki to extract and/or manipulate templates, template parameters, parser functions, tables, external links, wikilinks, lists, etc. found in wikitexts
 - authentik: One stop SSO token management service and library

Authentication:
 - easyauth: Create a centralized Authentication and Authorization token server. Works with FastAPI well.

Endpoint Frameworks:
 - pyramid: scalable and OO webframework fit between full featured and micro frameworks with extensions
 - flask: micro-web framework, that helps to build an APIs and supports unit testing
 - microdot: minimalist web framework inspired by flask which can run on low end systems including micropython
 - quart: ASGI based re-implementation of flask which is eventually planned to be merged with flask
 - fastAPI: light and fast built on top of starlette, pydantic and Uvicorn
 - CherryPy: minimalist, manipulable, light with lot of plugins
 - Bottle: lightweight and self contained micro framework with webserver and no additional dependencies
 - Web2py: light with no dependencies, fully-featured IDE, full stack, old fashioned
 - Tornado: also an asynchronous networking library allows for large and scaling solution
 - Quart: combination of asyncio and flask
 - Falcon: minimalist web API framework which is very fast used for large scale encourages REST
 - Enferno: A Python framework based on Flask microframework, with batteries included, and best practices in mind
 - instant-api: Instantly create an HTTP API with automatic type conversions, JSON RPC, and a Swagger UI with all the boring stuff done for you
 - hug: api/cli/local function; connected to a whole web framework, but gets a lot right
 - lumi: nano framework to convert your python functions into a REST API with minimal setup
 - frappe: low code web framework in Python and Javascript and MariaDB built for ERPNext

Web Frameworks:
 - pyhat: Python-htmx-ASGI-Tailwind for creating websites with less JS and more python
 - justpy:  object-oriented, component based, high-level Python Web Framework that requires no front-end programming. All design elements can be styled in Python but more low level than nicegui

Django: web framework for building a complex, data-driven websites
 - cookiecutter-django: framework for jumpstarting production-ready Django projects quickly
 - django-upgrade: automatically upgrade your Django projects to a specific version of Django
 - whitenoise: Radically simplified static file serving for Python web apps
 - django-rest-framework: powerful and flexible toolkit for building Web APIs using REST
 - django-ninja: FastAPI-inspired web framework for building APIs from Django views and Python 3.6+ type hints
 - graphene-django: for creating GraphQL API
 - django-crispy-forms: provides a tag and filter that lets you quickly render forms in a div format while providing an enormous amount of capability to configure and control the rendered HTML
 - django-pymemcache: Django cache backend that uses Pinterest's pymemcache library as the backend
 - django-filter:  filter down a queryset based on a model’s fields, displaying the form to let them do this
 - wagtail: content management system focused on flexibility and user experience
 - django-fsm: friendly finite state machine support
 - slippers: includes additional template tags and filters, but its headline feature is reusable components
 - kolo: See everything happening in your running Django app without leaving VSCode
 - django-admin-honeypot: fake Django admin login screen page
 - django-defender: blocks people from brute forcing login attempts
 - django-health-check: runs a full check on the deployment, using a number of plugins to check
 - django-q: multiprocessing distributed task queue for Django
 - django-debug-toolbar
 - django-browser-reload: Automatically reload your browser in development
 - nango: Streamlining Django forms to provide all the wins of single-page-applications without the pain
 - django-distill: Minimal configuration static site generator for Django
 - nplusone: catches performance issue that occurs when your code makes more database queries than it should
 - django-zen-queries: limits which code can make db queries

WSGI servers:
 - Gunicorn
 - fastwsgi: Ultra Fast WSGI Server for Python

ASGI server:
 - Uvicorn: ASGI server
 - Starlette: toolbox of higher-level components such as requests and responses that you can use to abstract away some of the details of ASGI

## Basic Science

Mathematics:
 - stdlib> decimal: decimal data type whose results match calculations done by hand and have configurable precision
 - stdlib> fractions: conversion of real numbers to fractions and wise versa with high precision
 - sympy: symbolic fuctions which be used for solving math expressions such as intergals, limits
 - fastnumpyio: Fast replacement for numpy.load and numpy.save
 - openblas: highly optimized library for linear algebra calculation forms basis of numpy and pandas
 - theano: define, optimize, and efficiently evaluate mathematical expressions involving multi-dimensional arrays, built on top of NumPy and allows use of GPU for fast calculations
 - latexify_py: package that generates LaTeX math description from Python functions
 - handcalcs: convert or render mathematicals equations in python directly to mathtext / latex
 - Aesara: define, optimize, and efficiently evaluate mathematical expressions involving multi-dimensional arrays
 - ortools: Google OR Tools for linear programming, contraint programming and other AI methods with a consistent API
 - cvxpy: convex optimization problems based on open source solvers OSQP, SCS, and ECOS
 - kiwisolver: efficient C++ implementation of the Cassowary constraint solving algorithm for LPP
 - pycosat: provides efficient Python bindings to picosat SAT solver on the C level
 - mpmath: real and complex floating-point arithmetic with arbitrary precision

Statistics:
 - stdlib> statistics: statistical functions
 - fitter: provides a simple class to identify the distribution from which a data samples is generated from
 - lmfit: provides a high-level interface to non-linear optimization and curve fitting
 - glum: generalized linear models common methods like least-squares regression, Poisson regression and logistic regression as special cases based on sklearn with similar API
 - pingouin: provides more uniform and user-friendly functions than SciPy and Statsmodels
 - PyMC3: statistical modeling tool for Bayesian statistical modeling & Probabilistic Machine Learning which focuses on advanced Markov chain Monte Carlo and variational fitting algorithms
 - PyRCA: A Python Machine Learning Library for Root Cause Analysis
 - ppscore: Predictive Power Score (PPS) replacement for corelation to detect relationships using decision trees ML model from sklearn internally
 - bayesian-histograms: for estimation of binary rare event rates, with fully automated bin pruning
 - DoWhy: An end-to-end library for causal inference
 - PyStan is a Python interface to Stan, a state-of-the-art platform for statistical modeling and high-performance statistical computation using Bayesian inference

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
 - nixtla/statsforecast: Automated time series processing and forecasting
 - etna: easy-to-use time series forecasting framework for preprocessing, feature generation and smart backtesting with unified interface
 - orbit: Bayesian time series modeling and inference with a familiar and intuitive initialize-fit-predict interface utilizing probabilistic programing languages under the hood
 - gluon-ts: Probabilistic Time Series Modeling in Python
 - tsfresh: Time Series feature extraction based on scalable hypothesis tests automatically
 - pastas: simple framework for processing, simulating, and analyzing of hydrological time series
 - flow-forecast: Deep learning PyTorch library for time series forecasting, classification, and anomaly detection (originally for flood forecasting)
 - cesium: timeseries feature extraction and ML libary for forecasting

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
 - fastapi-mvc: generate FastAPI projects based on MVC architectural pattern, WSGI + ASGI. Includes tests, GitHub actions, utilities, Helm, and more
 - cookiecutter-django: framework for jumpstarting production-ready Django projects quickly

Process / Best Practices:
 - recommenders: Best Practices on Recommendation Systems
 - Production Data Science: workflow for collaborative data science aimed at production

Data Cleaning:
 - missingno: Missing data visualisation in pandas
 - dplython: dyplr R equivalent for summarizing
 - fuzzywuzzy: fuzzy data matching
 - python-string-similarity: different string similarity and distance measures
 - textdistance: compare distance between two or more sequences with many algorithms
 - pyjanitor: Clean APIs for data cleaning. Python implementation of R package Janitor
 - datacleaner: community edition of datacleaner application
 - dora: uses scikit-learn, pandas, and Matplotlib for exploratory analysis, or more specifically, for automating the most undesirable aspects of exploratory analysis
 - scrubadub: remove personally identifiable info from free text
 - cleanco: clean organization names from abbreviations and terms
 - email-validator: library to perform syntax as well as domain DNS checks on email addresseses

Data Storage:
 - hub: Dataset Format for AI with slicing, version control, compression, distribution even on cloud, apply transformations using Ray
 - fds: fast data science is a transparent wrapper on dvc and git
   - dvc: Data version control. Git for data
 - pytables: Data storage for df from within pandas
 - pystore: Data storage for df from within pandas
 - docArray: nested, unstructured data in transit which allows deep-learning engineers to efficiently process, embed, search, recommend, store, and transfer the data with a Pythonic API

Data Transformation / Piplines / ETL:
 - dagster: data orchestrator for machine learning, analytics, and ETL with a partition concept
 - orchest: visual orchestration tool for ETL, parametrisation with jupyterlab interface
 - prefect: workflow management system, designed for modern infrastructure for data science
 - sf-hamilton: create dataframes from functions
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
 - pygwalker: Turn your pandas dataframe into a Tableau-style User Interface for visual analysis
 - bamboolib: GUI for pandas
 - mitoinstaller/mitosheet: spreadsheet frontend in notebooks with excel formula support that generates equivalent code based on plotly
 - pandas-gui: GUI for pandas
 - dtale: Visualizer for pandas data structures
 - sidetable: Create Simple Summary Tables in Pandas
 - staircase: data analysis package based on mathematical step functions based on pandas
 - pandas-datareader: Up-to-date remote data access for pandas. Works for multiple versions of pandas.

Pandas Alternatives:
 - fugue: convert code from pandas, SQL, dask, spark, ray in a unified interface to parallelize code
 - datatable: h2oai's bigdata library based on extremely fast data.table from R
 - polars: fast, multi-threaded DataFrames library implemented in Rust using Apache Arrow as memory model
 - Vaex: lazy out-of-core dataframes with multi-threading
 - StaticFrame: df based on immutable np array feature with fast no-copy operations with low overhead w.r.t pandas
 - RAPIDS: drop in pandas replacement to speed up analysis on optimised CUDA (Nvidia) - better than pandas with GPU
 - Dask: build on top of pandas to parallelize it, slower will non parallel
 - Modin: drop in pandas replacement to speed up common timeconsuming tasks by parellelising code using Ray or Dask
 - Koalas: based on spark engine

Plotting Meta Package:
 - Holoviz: High-level tools to simplify visualization in Python

Plotting:
 https://pyviz.org/tools
 https://www.python-graph-gallery.com/
 - zengl: high-performance, simple rendering with OpenGL
 - bashplotlib: plot graphs in the console
 - bqplot: interactive 2-D visualization system for Jupyter, based on the constructs of the Grammar of Graphics
 - lets-plot: ggplot inspired grammer of graphics with dynamic graphs
 - plotnine: ggplot2 inspired plotting library
 - altair: Vega based Plotly alternative
 - observableplot: concise API for exploratory data visualisation
 - gleam: interactive web visualisations
 - pygal: SVG Plots
 - plotly: Web plots
 - ggplot: based on R ggplot
 - pyecharts: wrapper for Apache echarts libary with high quality js charts
 - chartify: charting package based on bokeh with consistent interface making it easy for data scientists
 - Pandas-Bokeh: Bokeh plotting backend for Pandas, GeoPandas and Pyspark DataFrames
 - CMasher: a collection of scientific colormaps and utility functions
 - pyUpSet: Creating UpSet plots in Python but old and poor documentation
 - pyqtgraph:  graphics and GUI library for use in mathematics / scientific / engineering applications written entirely in python and pyqt/pyside for fast updating graphs which matplotlib can't do
 - netgraph: Publication-quality network visualisations

Matplotlib:
 - https://matplotlib.org/mpl-third-party/
 - proplot: matplotlib wrapper for a consistent interface for all kinds of maps and quick settings
 - seaborn: declerative api for mathplotlib designed for dataframes
 - Dexplot: simple and intuitive user experience for mathplotlib
 - mplfinance: plotting financial data such as stocks
 - mplcursors: provides interactive data selection cursors for Matplotlib. It is inspired from mpldatacursor, with a much simplified API
 - mplcursor alternative implemented in pure python: https://gist.github.com/AmirMardan/44152b7ff947a429c364c958e384e6a4
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

Creative Programming:
 - stdlib> turtle: draw shapes with code
 - manim: create animations with python scripts
 - joy: tiny creative coding library in Python
 - samila: Generative Art Generator

Spatial / Geographical:
 Wheels for mapping libraries: https://www.lfd.uci.edu/~gohlke/pythonlibs/
 Binaries: https://download.osgeo.org/osgeo4w/
 - PySAL: Library of Spatial Analytical Methods
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
 - spherely: manipulation and analysis of geometric objects on the sphere analogous to shapely
 - netCDF4: library to read netcdf geographic data format
 - xarray: Array manipulation library based for netCDF data models and Common Data Model (CDM)
 - iris: powerful, format-agnostic, community-driven Python package for analysing and visualising Earth science data
 - pyogrio: Vectorized spatial vector file format I/O for reading and writing GeoDataFrames to and from using GDAL/OGR very fast 5-20x
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
 - lat_lon_parser: parsing lat-long coordinates in "various" formats and converting e.g.: degrees to DMS

Graphs / DAG:
 - graph-tool, igraph, networkit, snap: C libraries for Graph analysis with python bindings
 - networkx: creation, manipulation, and study of the structure, dynamics, and functions of complex networks
 - netgraph: Publication-quality network visualisations
 - graphviz: thin wrapper over GraphViz open source graph plotting tools
 - pygraphviz: full blown python interface (create, edit, read, write, and draw) to Graphviz with similar API to networkx connected though SWIG
 - graphviz-python: official GraphViz python interface
 - pydot: pure python interface to Dot language for file manipulation, plotting requires GraphViz
 - nxviz: declarative graph Visualiation library for networkx graph objects

Dashboards:
 - datapane: upload and share interactive plot made from any plotting library as reports
 - Dash: based on Plotly
 - Bowtie
 - Panel: built on top of bokeh
   - Bokeh: JS charting package
 - ipyflex: A WYSIWYG layout editor for Jupyter widgets

IPython / Jupyter / Notebooks:
 - myst: live code in markdown for jupyter notebooks with widgets
 - codebraid: live code in Pandoc Markdown which can be executed and converted to any format; depends on Pandoc
 - markdown-code-runner: similar to codebraid above
 - jupyterlite: JupyterLab distribution that runs entirely in the browser based on Pyodide
 - IPython.core.display: support for various formats to be displayed in the output
 - ipycanvas: lightweight, fast and stable library exposing the browser's Canvas API to IPython
 - jupyterlab-code-formatter: plugin to facilitate invocation of code formatters such as black and isort
 - nb_black: Black code formatting for notebooks
 - nblint: pylint for notebooks
 - nbdime: provides tools for diffing and merging of Jupyter Notebooks
   - nbdiff: compare notebooks in a terminal-friendly way
   - nbmerge: three-way merge of notebooks with automatic conflict resolution
   - nbdiff-web: shows you a rich rendered diff of notebooks
   - nbmerge-web: gives you a web-based three-way merge tool for notebooks
   - nbshow: present a single notebook in a terminal-friendly way
 - execnb: jupyter notebook execution and output capture through code and CLI, without needing jupyter
 - euporie: jupyter notebooks in terminal
 - nbterm: simple notebook for terminal
 - nbpreview: terminal viewer for Jupyter notebooks. It's like cat for ipynb files
 - nbstripout: strip output from Jupyter and IPython notebooks
 - nbconvert: Convert Notebooks to other formats pdf, static presentations based on reveal.js (part of jupyter)
 - nbinteract: Convert notbooks with widgets to run on remote binder server with full interactivity
 - nbdev: meta package for debugging, refactoring, testing, create docs, publish packages etc in Notebooks
   - dejavu: create presentations with widgets which are non-interactive (included in >=nbconvert6.2)
 - jupytext: code is saved in a specified format (py, md, Rst etc.) and is synced to ipynb on load
 - jupytercad: collaboratively work on freecad designs
 - jupyter-book: create publication quality books in Jupyter especially with mathematical notation
 - jupyter-notify: notification when long running notebooks finish running
 - rise: reveal.js based presentation for live notebooks with interactivity based on reveal.js for classic notebooks
 - ipyvizzu: is the Jupyter Notebook integration of Vizzu - animated graphs for storyboarding
 - ipyflex: A WYSIWYG layout editor for Jupyter widgets
 - voila: jupyter notebook dashboards based on ipywidgets
 - xeus-python: ipykernel alternative for jupyter
 - ipyflow: ipython kernel with reactivity, execution suggestions, syntax extensions, and more
 - ipywidgets: adds interactivity to jupyter notebooks
   - ipympl:  enables the interactive features of matplotlib in the Jupyter notebook and in JupyterLab using Jupyter interactive widgets (%matplotlib widget)
 - ipydatagrid: Fast Datagrid widget with multiple features
 - papermill: parametrizing jupyter notebooks so the notebook can be run for different values and also build workflow based on results of the notebook
 - linearpy: simiarl to papermill that can use notebooks in production pipelines
 - testbook: passess code from a notebook to a testing file to be used with any testing module
 - pytest-jupyter: pytest plugin for Jupyter
 - whyprofiler: CPU profiler for Jupyter notebook that not only identifies hotspots but can suggest faster alternatives
 - bqplot: interactive 2-D visualization system for Jupyter, based on the constructs of the Grammar of Graphics
 - powerbi-jupyter: IPyWidget that enables customers to use PowerBI embedding capabilities in a Jupyter notebook seamlessly
 - ipython-sql: load sql into IPython magic for IPython, hopefully evolving into full SQL client
 - anywidget: compatibility layer around Jupyter Widgets to allow widgets to run in any enviornment by leveraging brower JS engine simplyfying development and packaging of widgets
   - ipyreact: React widget in python built on top of AnyWidget

### Finance:

Data:
 - findatapy: common API to download market data from many sources including Quandl, Bloomberg, Yahoo, Google, customer API's via config files etc.
 - yfinance: Yahoo finance API
 - yahooquery: Yahoo finance API unofficial
 - quantel: API for many international and NSE data
 - nsepy: API for nse including CLI depends on numpy and pandas

Charts:
 - mplfinance: matplotlib finance API for plotting stocks

Technical Analysis:
 - talib: Technical Analysis
 - talipp: Technical Analysis library for O(1) iterative
 - pandas-ta: Technical Analysis Indicators - Pandas TA is an easy to usePandas Extension with 120+ Indicators
 - finta: Common financial technical indicators implemented in Pandas

Strategies:
 - Backtrader: Backtesting
 - backtesting.py
 - Zipline: Backtesting, accquired by Robinhood
 - orats: US options analysis API
 - qf-Lib: provides an advanced event driven backtester and a set of high quality tools for quantitative finance by CERN
 - autotrader: development platform for automated trading systems - from backtesting to optimisation to livetrading
 - Vectorbt: helps find your trading edge, using the fastest engine for backtesting, algorithmic trading, and research
 - OctoBot: cryptocurrency trading bot for TA, arbitrage and social trading with an advanced web interface
 - Gemini: cryptocurrency backtesting engine that focuses on simplicity
 - Quantdom: backtesting framework that let's you focus on modeling financial strategies, portfolio management, and analyzing backtests
 - pybroker: algo trading with ML

Fundamental Analysis:
 - numpy-financial: collection of elementary financial functions for numpy which were removed from numpy
 - opstrat: option pricing and plotting
 - mibian: Options Pricing models
 - py_vollib: library for calculating option prices, implied volatility and greeks
 - quantsbin: pricing and plotting of vanilla option prices, greeks and various other analysis

AI/ML:
 - mlfinlab: machine learning for finance

Portfolio Management / Testing:
 - Empyrial: Portfolio Management Framework for risk and performance analysis
 - quantstats: analytics for quants with stats, plots and reports
 - Qlib: AI-oriented quantitative investment platform for testing training executing tracking algos & strategies by Microsoft
 - Pyfolio: To check portfolio perf metrics
 - financepy: pricing and risk-management of Financial Derivatives, including fixed-income, equity, FX and credit derivatives

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
 - sage: for calculating global feature importance using Shapley values
 - shap: (SHapley Additive exPlanations) is a game theoretic approach to explain the output of any machine learning model by answering how much does each feature contribute to an individual prediction. They are a combination of Shapley values and LIME since Shapley values are time consuming to calculate, whereas SHAP is fast due to approximations and hence is used more widely.
   - Shapash: provides several types of visualization of ML models that display explicit labels that everyone can understand based on shap backend
 - NannyML: estimates performance with an algorithm called Confidence-based Performance estimation (CBPE) and  captures the impact of data drift on performance
 - eli5: used to inspect ML classifiers and explain their predictions, used to debug algorithms such as sklearn regressors and classifiers, XGBoost, CatBoost, Keras, etc
 - deepchecks: build test suites for ML models & data for performance, distribution, methodology, explainability checks
 - Fairlearn: assess a AI/ML systems fairness
 - alibi: machine learning model inspection and interpretation for classification and regression models
 - eli5: explainability and debugging of ML models
 - optuna: automatic hyperparameter optimization software framework, particularly designed for machine learning
 - hyperopt: Distributed Asynchronous Hyper-parameter Optimization with Bayesian optimization for speed up
 - Hummingbird: compile trained traditional ML models into tensor computations PyTorch
 - dirty_cat: facilitates machine-learning on non-curated categories: robust to morphological variants, such as typos
 - PostgresML: end-to-end machine learning system which enables you to train models and make online predictions using only SQL
 - PyMDE: compute vector embeddings of items, such as images, biological cells, nodes in a network, or any other type of abstract object generalizing well-known methods like PCA, spectral embedding, multi-dimensional scaling for use in machine learning
 - lilac: extract structured dimentions out of free text such as sentiment, addresses, languages etc

MLOps:
 - Feast: an operational data system for managing and serving machine learning features to models in production
 - modelkit: minimalist yet powerful MLOps library for Python, built for people who want to deploy ML models to production
 - mlflow: open source platform to manage the ML lifecycle, including experimentation, reproducibility, deployment, and a central model registry
 - evidently: tools to evaluate, test and monitor machine learning models
 - whitebox: open source E2E ML monitoring platform with edge capabilities that plays nicely with kubernetes
 - whylogs: model monitoring and analysis from logs with visualisation

Machine Learning Wrapper Libraries / AutoML:
 - blockly: googles visual AI/ML editor for python and ML
 - auto-sklearn: AutoML version of sklearn
 - auto-keras: AutoML version of keras
 - tpot: Tree-Based Pipeline Optimization Tool (TPOT) was one of the very first AutoML methods and open-source software packages developed for the data science community
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
 - balance: package to deal with imbalanced classed in ML by Facebook

Machine Learning Frameworks:
 - scikit-learn: algorithms of machine learning and data mining tasks
   - imbalanced-learn: relying on scikit-learn (imported as sklearn) and provides tools when dealing with classification with imbalanced classes
 - PyGBM: Gradient Boosting Decision Trees
 - XGBoost/LightGBM/CatBoost: optimised, scalable and fast implementations of gradient
 - lleaves: LLVM-based compiler for LightGBM decision trees which converts trained LightGBM models to optimized machine code, speeding-up prediction by ≥10
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
 - simple_elmo: Simple ELMO model
 - gensim: robust semantic analysis, topic modeling and vector-space modelling
 - nlp: lightweight and extensible library to easily share and access datasets and evaluation metrics for Natural Language Processing (NLP) based on tensorflow dataset tfds
 - wordcloud: create wordclouds
 - easynlp: NLP library based on PyTorch from Alibaba
 - transformers: State-of-the-art pretrained models from huggingface integration with your workflow
 - txtai: AI-powered semantic search based on latest techniques as opposed to keyword based libraries
 - tweet-preprocessor: preprocessor for NLP on tweets with identification of emojis, hashtags, links etc

Image Processing / Character Recognition (OCR) / Computer Vision:
 - scikit-image: collection of algorithms for image processing
 - pytesseract: Tesarract 4 python bindings
 - imageio: image manipulation library depends on numpy and pillow (minimum) and ffmpeg (optional)
   - pillow: maintained version of PIL, for working with images
 - imutils: image maniputlation utilities
 - opencv-contrib:
   - OpenCV-Python: Open computer vision library
 - SimpleCV: framework with simple API for building computer vision applications
 - mahotas: computer vision and image processing library with over 100 functions and counting
 - simpleitk: library for Insight Toolkit developed for biomedical sciences
 - pgmagick: API for graphicsmagick a imagemagick fork
 - pycairo: API for Cairo vector library
 - docquery: library and command-line tool that makes it easy to analyze semi-structured and unstructured documents (PDFs, scanned images, etc.) using large language models (LLMs)

Audio Processing / Speech Recognition:
 - pyttsx3: Offline tts modules bundled with sapi5, nsss, espeak engines
 - SpeechRecognition: Library for performing speech recognition, with support for several engines and APIs, online and offline
 - voice2json: speech recognition, transcription, intent recognition command line tools
 - Picovoice: voice recognition library to add Alexa like feature to python apps based on pvrecorder
   - pvrecorder: Python SDK which captures audio suitable for speech recognition, meaning the audio captured is already 16 kHz and 16-bit
 - openspeech: Open-Source Toolkit for End-to-End Speech Recognition leveraging PyTorch-Lightning and Hydra
 - speechbrain: PyTorch-based Speech Toolkit for speech recognition, speaker recognition, speech enhancement, multi-microphone signal processing etc
 - librosa: music and audio analysis
 - textlesslib: for Textless Spoken Language Processing by Facebook

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

Web:
 - youtube-dl: download vidoes from multple sites
 - pytube: download videos from youtube
 - unzip-http: extract files from remote .zip files without downloading entire archive

Image:
 - segno: faster and more feature rich QR Code generator

Image as code:
 - roadmapper: roadmap as code

Audio:
 - pyFLAC: Real-time lossless audio compression in Python based on Soundfile which in turn is based on libsndfile, CFFI and numpy
 - Pedalboard: Spotify’s Audio Effects Library for Python
 - python-vlc: play media using VLC from python
 - pyaudio: bindings for PortAudio v19, the cross-platform audio I/O library, allows computer mic to work with python

Video:
 - deffcode: OpenCV like API for FFmpeg

Convenience:
 - Tenacity: maintained fork of `retrying` which retries a fn with custom exception actions
 - polling2: library for polling any repetitive function
 - circuitbreaker: implementation of "Circuit Breaker" Pattern (https://martinfowler.com/bliki/CircuitBreaker.html)
 - mdiff: calculate diffs by character and display in terminal or gui

Uncategorised:
 - gdb: python module for GDB scripting
 - zipfly: writing large ZIP archives without memory inflation

Data:
 - namematch: Tool for probabilistically linking the records of individual entities (e.g. people) within and across datasets

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
 - mkposters: Make cheatsheet like posters from data in Markdown files
 - miller: process flat file data from commandline
 - cleanvision: image identification and tagging ML library
 - vidrsyncer: Synchronize calendars and contacts with WebDAV
 - tinyvector: tiny, customisable vector embedding database based on flask+numpy/rust with SQLite backend 500 lines of code scales to 100 million+ dimentions
 - 
