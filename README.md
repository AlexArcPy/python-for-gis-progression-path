# python-for-gis-progression-path
Progression path for a GIS analyst who wants to become proficient in using Python for GIS: from apprentice to guru

**This is a work in progress**

This is an attempt to provide a structured collection of resources that could help a GIS professional to learn how to use Python when working with spatial data management, mapping, and analysis. The resources are organized by progress category so basically everyone should be able to learn something new along the way.

The resources will include books, web pages and blog posts, online courses, videos, Q/A from GIS.SE, links to code snippets, and some bedtime readings. 

_The resources will focus mostly on learning about Python for users of Esri software though there will be some links that will apply even for open-source GIS professionals._

---

# Beginner

You should be able to write short simple scripts in pure Python with no connection to GIS. To learn the basics of Python, you can find a ton of resources online such as [CodeAcademy](https://www.codecademy.com/learn/python), [Learn Python the Hard Way](https://learnpythonthehardway.org/book/intro.html), [Dive into Python](http://www.diveintopython3.net/installing-python.html), [A Whirlwind Tour of Python](http://www.oreilly.com/programming/free/a-whirlwind-tour-of-python.csp), and many other books from [Python.org](https://wiki.python.org/moin/IntroductoryBooks) and this [Free programming books](https://github.com/vhf/free-programming-books/blob/master/free-programming-books.md#python) GitHub repo.

## Resources
If you don't want to learn Python this way and would rather like to catch up learning how Python can be used for GIS:
#### Books
* [Python Scripting for ArcGIS](https://www.amazon.com/Python-Scripting-ArcGIS-Paul-Zandbergen/dp/1589483715) for Esri users. Going through this book _might_ be sufficient to learn everything you might ever need
* [Geoprocessing with Python](https://www.manning.com/books/geoprocessing-with-python) for open-source users

#### Courses:
* Esri instructor-led course [Introduction to Geoprocessing Scripts Using Python](https://www.esri.com/training/catalog/57630435851d31e02a43f054/introduction-to-geoprocessing-scripts-using-python/)
* Esri free web course [Python for Everyone](https://www.esri.com/training/catalog/57630436851d31e02a43f13c/python-for-everyone/)
* Esri web course [Basics of Python (for ArcGIS 10)](https://www.esri.com/training/catalog/57630430851d31e02a43ee14/basics-of-python-(for-arcgis-10)/)
* Penn State free web course [GIS Programming and Automation](https://www.e-education.psu.edu/geog485/node/104)

#### Videos:

Look for videos at Esri Video web page and search for `Python` and sort by most recent. An example of [URL](http://www.esri.com/videos/search?q=python#?sortby=recent&channels=esri,Events,ArcGIS,Industries,ArcGIS,esri).

* Esri video [Working with Feature Data Using ArcPy](http://www.esri.com/videos/watch?videoid=3448&isLegacy=true&title=working-with-feature-data-using-arcpy)
* Esri video [ArcMap and Python: Closing the VBA Gap](http://www.esri.com/videos/watch?videoid=1229&isLegacy=true&title=arcmap-and-python-closing-the-vba-gap)
* Esri video [Python: Getting Started 2014](http://www.esri.com/videos/watch?videoid=3879&channelid=LegacyVideo&isLegacy=true&title=python:-getting-started)
* Esri video [Python: Developing Geoprocessing Tools](http://www.esri.com/videos/watch?videoid=4304&channelid=LegacyVideo&isLegacy=true&title=python:-developing-geoprocessing-tools)
* Esri video [Python: Getting Started 2013](http://www.esri.com/videos/watch?videoid=2622&channelid=LegacyVideo&isLegacy=true&title=python---getting-started)

#### Tutorials / web pages:
* [arcpy tutorials](https://boxshapedworld.wordpress.com/tutorials/)
* Esri Blog post [Scheduling a Python script or model to run at a prescribed time](https://blogs.esri.com/esri/arcgis/2013/07/30/scheduling-a-scrip/)

#### Collections of resources:
* Esri blog [Seven easy ways to start learning Python and ArcPy](https://blogs.esri.com/esri/supportcenter/2014/03/26/8-easy-ways-learning-python-arcpy/)
* GIS.SE [What are some resources for learning ArcPy?](http://gis.stackexchange.com/a/53826/14435)
* [Python for GIS tutorials](http://courses.washington.edu/geog465/Programming_Resources.html)

## Skills

### GIS specific
At this point, you should be able to:
- write some simple scripts either using `arcpy` site-package or `ogr/gdal` libraries
- report information about your GIS assets (data format, geometry type, data schema, spatial reference)
- write code for calling ArcGIS GP tools from Python code and inspect the `Result` object returned
- perform an operation on multiple datasets in batch mode using `arcpy` listing functions
- read and update attributes & geometry of features using `arcpy.da` cursors
- create and operate `arcpy.Geometry()` objects (accessing both their properties and methods)
- create an ArcGIS toolbox with a simple script tool executing a Python source file
- report information about map layers (eg. data sources, broken paths, definition queries) within an ArcMap map document (.mxd) using `arcpy.mapping` module

### Python
At this point, you should be familiar with:
- variables of different data types (numeric, string, date etc.)
- data structures of different types (list, tuple, dictionary, set)
- `for` and `while` loops, `if-elif-else` blocks
- import of external Python modules and packages (eg. `import os`)
- functions and how they work (eg. input arguments and `return` statement)
- reading/writing of text files using the `os` module

### Exercises
This section contains the examples of tasks that you might need to write at some point of time. Implementing these tasks in Python code would be a good sign that you have mastered the basics of Python for ArcGIS.
- get a list field names of Date type in a file geodatabase feature class
- copy multiple shapefiles into a file geodatabase at once
- re-project all rasters in a folder
- update data sources for layers in a map document and save a new map document
- write to a .txt or a .csv file information about your GIS assets

---

# Intermediate

## Resources
* Learn about [various Python IDEs](https://wiki.python.org/moin/IntegratedDevelopmentEnvironments) and find out which one you like most. Many start with [PyScripter](https://sourceforge.net/projects/pyscripter/) (free) and then move to something else:
 - SO question [What IDE to use for Python?](http://stackoverflow.com/questions/81584/what-ide-to-use-for-python)
 - Check PyCharm, WingIDE, Eclipse PyDev, Visual Studio Code, Python Tools for Visual Studio
 - Check Esri blog post [Choosing the right Python Integrated Development Environment](https://blogs.esri.com/esri/arcgis/2013/06/24/choosing-the-right-python-integrated-development-environment/)
 
* Learn about [VCS](https://en.wikipedia.org/wiki/Version_control) such as `Git` for managing the source code. [BitBucket](https://bitbucket.org/product) by Atlassian and [GitLab](https://about.gitlab.com/gitlab-com/) provides free private repositories and [GitHub](https://github.com/) provides free public repositories (you need to pay to create private ones).
 - Find out whether there is a VCS solution deployed in-house within your organization, such as [Microsoft TFS](https://www.visualstudio.com/tfs/), which you could use to check in the code
 
* Watch [Python Fundamentals](https://app.pluralsight.com/library/courses/python-fundamentals/table-of-contents) on Pluralsight
* Watch Esri video [Python: Useful Libraries for the GIS Professional](http://www.esri.com/videos/watch?videoid=2938&isLegacy=true&title=python-useful-libraries-for-the-gis-professional)

#### Tutorials / web pages
* Esri blog [Generating a choice list from a field](https://blogs.esri.com/esri/arcgis/2011/08/25/generating-a-choice-list-from-a-field/) for a custom script tool
* Esri blog [How to Debug Python Toolboxes in 3 Easy Steps](https://blogs.esri.com/esri/arcgis/2012/12/14/how-to-debug-python-toolboxes-in-3-easy-steps/)
* Esri blog [Field mapping and Python scripting](https://blogs.esri.com/esri/arcgis/2012/08/30/field-mapping-and-python-scripting/)
* Esri [ArcPy team blog](https://arcpy.wordpress.com/)
* [Python and GIS blog](https://pythongisandstuff.wordpress.com/)
* Convenience functions for arcpy in repo [arcapi](https://github.com/NERC-CEH/arcapi)
* Sample ArcGIS toolbox [SampleArcPyMappingScriptTools_10_v1](http://www.arcgis.com/home/item.html?id=18c19ec00acb4d568c27bc20a72bfdc8) for working with `arcpy.mapping` (20+ tools)
* Learn how to use [pip](http://stackoverflow.com/questions/4750806/how-do-i-install-pip-on-windows) for managing Python packages
* Learn [`virtualenv`](https://virtualenv.pypa.io/en/stable/) for managing Python environments
* Learn [R-ArcGIS bridge](https://github.com/R-ArcGIS/r-bridge-install) to combine Python code and R code

## Skills

### GIS specific
At this point, you should be able to:
- automate map production using `arcpy.mapping` with data-driven pages
- manage .pdf files (eg. re-ordering, merging, splitting) using `arcpy`
- export ArcMap map documents to various file formats such as .png and .pdf
- update text elements content in layout of ArcMap map document
- executing DBMS spatial functions from Python and using `arcpy.ArcSDESQLExecute()`
- use `FieldInfo`, `FieldMap`, and `FieldMappings` classes from `arcpy` to manage data schema
- customize custom ArcGIS script tool behavior using `ToolValidator` class
- start using Python toolboxes and Python add-ins in ArcGIS when it makes sense
- debug `arcpy`-driven code with the help of geoprocessing messages
- writing smaller unit tests for GIS workflows
- handling `JSON` in Python and `arcpy`
- generate simple Excel files from datasets with Python and `xlsxwriter` package

### Python
At this point, you should be familiar with:
- installing Python packages using pip
- Python 3 to be able to write code that will be ported later to ArcGIS Pro
- Python PEP-8 style guide
- `collections` module data structures such as `defaultdict`, `namedtuple`, `Counter`
- list and dictionary comprehensions
- set comprehensions and set theory operations
- enumerating sequences using built-in `enumerate` function'
- writing own functions and handling the arguments
- lambda functions
- convenience functions
- accessing databases using Python
- working with disk-based database SQLite from Python
- using non-Latin characters in the source file and handling Unicode
- Python exceptions and `try/except` block
- Python `traceback` module
- tuple unpacking with function calls
- sending emails with Python
- accessing ftp sites with Python
- running Python files with the cmd and task scheduler
- zipping folders and files with Python and reading archive files
- sending SMS using Python and `Twilio`

---

# Advanced

## Resources

### GIS specific
* Learn how to use ArcObjects from Python:
 - GIS.SE [Accessing ArcObjects from Python?](http://gis.stackexchange.com/a/110/14435)
 - GIS.SE [Guidelines for using ArcObjects from Python](http://gis.stackexchange.com/questions/129456/guidelines-for-using-arcobjects-from-python)
 - Esri video [Extending Python Using C++ and ArcObjects](http://www.esri.com/videos/watch?videoid=1242&isLegacy=true&title=extending-python-using-c_plus__plus_-and-arcobjects)
 - Esri [recorded live-training seminar on ArcObjects](https://www.youtube.com/watch?v=AtwD02wyP3A)
 - Esri Help page [Learning ArcObjects] (http://resources.arcgis.com/en/help/arcobjects-net/conceptualhelp/#/Learning_ArcObjects/0001000000p1000000/) will help you determine which ArcObjects will provide the functionality required by your customization
 - Esri Help page [Reading OMDs](http://resources.arcgis.com/en/help/arcobjects-net/conceptualhelp/#/Reading_OMDs/000100000306000000/) provides a description of the diagram notation used on the ArcObjects object model diagrams (OMDs)
 - Blog post [Accessing ArcObjects in Python](https://tereshenkov.wordpress.com/2016/01/16/accessing-arcobjects-in-python/)

* Learn about other GIS packages. 
 - Go through a comprehensive list of [Essential Python Geospatial Libraries](http://carsonfarmer.com/2013/07/essential-python-geo-libraries/) (also available on [this GitHub page](https://github.com/SpatialPython/spatial_python/blob/master/packages.md)) 
 - Watch the series of recorded workshops on using open source GIS packages: [Geospatial data in Python: Database, Desktop, and the Web](http://pyvideo.org/speaker/carson-farmer.html)
 
* Learn about how to build desktop GUI applications using Tkinter, WxPython, PyQt, PySide, or Kivy and then embed them into ArcGIS or just let them be aware of spatial datasets:
 - [Python Add-Ins and Tkinter](http://anothergisblog.blogspot.se/2013/07/python-add-ins-and-tkinter.html)
 - Esri blog post [Using Python and QML to build native apps](https://blogs.esri.com/esri/arcgis/2015/11/16/using-python-and-qml-to-build-native-apps/)
 - [GitHub repo](https://github.com/ldanzinger/PyOtherSideForArcGIS) with samples for ArcGIS, Qt and Python integration 
 - Watch Esri video [Developing Custom Tools with PyQt](http://www.esri.com/videos/watch?videoid=4549&isLegacy=true&title=developing-custom-tools-with-pyqt)

* Esri blog [Accessing Multidimensional Scientific Data using Python](https://blogs.esri.com/esri/arcgis/2015/06/10/accessing-multidimensional-scientific-data-using-python/)
* [Python and GIS blog](https://pymorton.wordpress.com/)
* Convert ArcGIS script toolbox (.tbx) to Python toolbox (.pyt) with [tbxtopyt](https://github.com/jasonbot/tbxtopyt)

### Python

* Learn [IPython](https://ipython.org/) and the concept of reproducible research:
 - Learn how to use [Jupyter notebook](http://jupyter.org/)
 - Learn how to combine [Python and R code](https://www.continuum.io/blog/developer/jupyter-and-conda-r) in the same Jupyter notebook

* Learn about using Python for web development:
 - learn [`flask`](http://flask.pocoo.org/) and [`django`](https://www.djangoproject.com/). Start with flask and only then move to Django
 - learn [`geodjango`](https://docs.djangoproject.com/en/1.10/ref/contrib/gis/) to serve spatial datasets on the web. Read through pdf [ArcGIS JavaScript Plus Django Equals Dynamic Web App](http://proceedings.esri.com/library/userconf/proc15/papers/794_139.pdf)

* Watch [Python – Beyond the Basics](https://app.pluralsight.com/library/courses/python-beyond-basics/table-of-contents) on Pluralsight 
* Learn about [`nlpk`](http://www.nltk.org/) Python package to work with human language data (eg. parsing address data)
* Learn about [`regex`](https://docs.python.org/2/howto/regex.html) Python package to work with regular expressions in Python (eg. finding addresses in a specific format)
* Learn [`Selenium`](https://github.com/SeleniumHQ/Selenium) Python package to be able to automate web app testing. Read the docs for Python [here](http://www.seleniumhq.org/docs/03_webdriver.jsp#introducing-the-selenium-webdriver-api-by-example)

* Learn about numerical computing and data science:
 - Install `Anaconda`(https://www.continuum.io/downloads) and learn about `conda`. This is helpful as [Python in ArcGIS Pro](https://geonet.esri.com/docs/DOC-8359) is implemented using a [conda](http://conda.pydata.org/docs/test-drive.html) env
 - Learn numerics, science, and data with Python with [scipy-lectures](http://www.scipy-lectures.org/)
 - Learn what [`scipy.spatial`](https://docs.scipy.org/doc/scipy/reference/spatial.html) can do for your GIS work
 - Read [Python for Data Analysis](http://shop.oreilly.com/product/0636920023784.do) and [Python for Computational Science and Engineering](https://www.southampton.ac.uk/~fangohr/training/python/pdfs/Python-for-Computational-Science-and-Engineering.pdf) (free book)

* Learn about managing and processing larger spatial datasets as performance will matter.
 - learn profiling techniques to find out what code takes most time to execute
 - learn benchmarking to compare execution time for functions that do the same thing using different tools (eg. looking for the fastest way to count points in polygons)
 - learn how to use `multiprocessing` module with ArcGIS at Esri blog post [Multiprocessing with ArcGIS – Approaches and Considerations (Part 1)](https://blogs.esri.com/esri/arcgis/2012/09/26/distributed-processing-with-arcgis-part-1/)
 - Esri blog [Be successful overlaying large, complex datasets in Geoprocessing](https://blogs.esri.com/esri/arcgis/2012/06/15/be-successful-overlaying-large-complex-datasets-in-geoprocessing/)

* Start looking for doing certain things outside of ArcGIS such using `pandas`
* Learn best practices for organizing configuration and settings for a larger workflow where you need to keep the config values apart from the business logic (eg. using JSON or ConfigParser or init() )
* Learn ArcGIS REST API
 - Learn [`requests`](http://docs.python-requests.org/en/master/) module
 - ArcGIS toolbox [ArcGIS Server Administration Toolkit - 10.1+](http://www.arcgis.com/home/item.html?id=12dde73e0e784e47818162b4d41ee340)
 - Learn [ArcGIS Python API](https://developers.arcgis.com/python/) to manage ArcGIS Online / Portal organization

## Skills

### GIS specific
At this point, you should be able to:
- execute ArcObjects code from Python using `comtypes` library
- export the data from tables and feature classes into Excel with custom formatting using `xlsxwriter`
- generate .pdf files from scratch that would contain map images, custom charts, and tables using `reportlab` 
- generate .pdf report files using ArcGIS report templates (.rlf) and `arcpy`
- generate graphs using `arcpy.Graph`, `arcpy.GraphTemplate` with graph template files (.tee), and Make Graph GP tool
- perform graph theory operations on linear datasets using `networkx` (eg. point-to-point routing)
- plot geodata with `Matplotlib` (both vector and raster)
- use `numpy` and `pandas` for manipulating spatial dataset attribute table
- use `requests` and/or `arcrest` package to access ArcGIS Server site, ArcGIS Online / Portal organizations through ArcGIS REST API
- call FME workbenches from Python
- access readers and writers in FME with `fmeobjects`

### Python
At this point, you should be familiar with:
- building desktop GUI applications using PyQt, PySide, or Kivy (eg. visualize a shapefile features in a window)
- contributing to open-source projects such as `arcrest` or `geopandas` reporting bugs or new functionality
- creating new conda environments and installing various packages into specific environments
- refactoring wrapping the code into functions, modules, and packages
- OOP basics and creating own classes

### Exercises
This section contains the examples of tasks that you might need to write at some point of time. Implementing these tasks in Python code would be a good sign that you have mastered the advanced concepts of Python for ArcGIS.
- hide/show map grid of data frame in a map layout before exporting the map in a map document using `arcpy` package and ArcObjects
- update label's text of a scale bar in a map layout using pure ArcObjects
- generate a service area (drive-time) polygon for an arbitrary point on a street network stored as a shapefile using `networkx`
- find out the fastest spatial join - ArcGIS Spatial Join GP tool, `rtree` in PostGIS, SQL Server `STContains`, or `shapely` Python package
- create a new csv file from an existing one by filtering certain rows using `pandas`
