# python-for-gis-progression-path

Progression path for a GIS analyst who wants to become proficient in using Python for GIS: from apprentice to guru

**This is a work in progress**

This is an attempt to provide a structured collection of resources that could help a GIS professional to learn how to use Python when working with spatial data management, mapping, and analysis. The resources are organized by progress category so basically everyone should be able to learn something new along the way.

The resources will include books, web pages and blog posts, online courses, videos, Q/A from GIS.SE, links to code snippets, and some bedtime readings.

_The resources will be applicable both for Esri software users as well as open-source GIS professionals._

---

# Beginner

You should be able to write short simple scripts in pure Python with no connection to GIS. To learn the basics of Python, you can find a ton of resources online such as [CodeAcademy](https://www.codecademy.com/learn/python), [Learn Python the Hard Way](https://learnpythonthehardway.org/book/intro.html), [Dive into Python](http://www.diveintopython3.net/installing-python.html), [A Whirlwind Tour of Python](http://www.oreilly.com/programming/free/a-whirlwind-tour-of-python.csp), and many other books from [Python.org](https://wiki.python.org/moin/IntroductoryBooks) and this [Free programming books](https://github.com/vhf/free-programming-books/blob/master/free-programming-books.md#python) GitHub repo.

## Resources

If you don't want to learn Python this way and would rather like to catch up learning how Python can be used for GIS:

### Books

* [Python Scripting for ArcGIS](https://www.amazon.com/Python-Scripting-ArcGIS-Paul-Zandbergen/dp/1589483715) for Esri users
* [Geoprocessing with Python](https://www.manning.com/books/geoprocessing-with-python) for open-source users

Going through these books _may_ be sufficient to learn everything you may ever need if you are an Esri or an open-source GIS user, respectively.

### Courses

* Esri instructor-led course [Introduction to Geoprocessing Scripts Using Python](https://www.esri.com/training/catalog/57630435851d31e02a43f054/introduction-to-geoprocessing-scripts-using-python/)
* Esri free web course [Python for Everyone](https://www.esri.com/training/catalog/57630436851d31e02a43f13c/python-for-everyone/)
* Esri web course [Basics of Python (for ArcGIS 10)](https://www.esri.com/training/catalog/57630430851d31e02a43ee14/basics-of-python-(for-arcgis-10)/)
* Penn State free web course [GIS Programming and Automation](https://www.e-education.psu.edu/geog485/node/104)

### Videos

Look for videos at Esri Video web page and search for `Python` and sort by most recent. An example of [URL](http://www.esri.com/videos/search?q=python#?sortby=recent&channels=esri,Events,ArcGIS,Industries,ArcGIS,esri).

* Esri video [Working with Feature Data Using ArcPy](http://www.esri.com/videos/watch?videoid=3448&isLegacy=true&title=working-with-feature-data-using-arcpy)
* Esri video [ArcMap and Python: Closing the VBA Gap](http://www.esri.com/videos/watch?videoid=1229&isLegacy=true&title=arcmap-and-python-closing-the-vba-gap)
* Esri video [Python: Getting Started 2014](http://www.esri.com/videos/watch?videoid=3879&channelid=LegacyVideo&isLegacy=true&title=python:-getting-started)
* Esri video [Python: Developing Geoprocessing Tools](http://www.esri.com/videos/watch?videoid=4304&channelid=LegacyVideo&isLegacy=true&title=python:-developing-geoprocessing-tools)
* Esri video [Python: Getting Started 2013](http://www.esri.com/videos/watch?videoid=2622&channelid=LegacyVideo&isLegacy=true&title=python---getting-started)

### Tutorials / web pages

* [arcpy tutorials](https://boxshapedworld.wordpress.com/tutorials/)
* Esri Blog post [Scheduling a Python script or model to run at a prescribed time](https://blogs.esri.com/esri/arcgis/2013/07/30/scheduling-a-scrip/)
* [PyQGIS Developer Cookbook](https://docs.qgis.org/testing/en/docs/pyqgis_developer_cookbook/)

### Collections of resources

* Esri blog [Seven easy ways to start learning Python and ArcPy](https://community.esri.com/groups/technical-support/blog/2014/03/26/7-easy-ways-learning-python-arcpy)
* GIS.SE [What are some resources for learning ArcPy?](http://gis.stackexchange.com/a/53826/14435)
* GIS.SE [Learning resources for PyQGIS?](https://gis.stackexchange.com/questions/250035/learning-resources-for-pyqgis)
* [Python for GIS tutorials](http://courses.washington.edu/geog465/Programming_Resources.html)
* [Python GDAL/OGR Cookbook!](https://pcjericks.github.io/py-gdalogr-cookbook/index.html)

## Skills

### GIS specific

At this point, you should be able to:

* write some simple scripts either using `arcpy` site-package or `ogr/gdal/pyqgis` libraries
* report information about your GIS assets (data format, geometry type, data schema, spatial reference)
* write code for calling ArcGIS geoprocessing tools (inspectig the `arcpy.Result` object returned) / `ogr` geometry methods / `PyQGIS` tools from Python code
* perform an operation on multiple datasets in batch mode using `arcpy`/`ogr` listing functions
* read and update attributes & geometry of features using `arcpy.da` cursors or `ogr` data source methods
* create and operate `arcpy.Geometry()` objects (accessing their properties and methods) or `ogr.Feature()`
* create an ArcGIS toolbox with a simple script tool executing a Python source file
* report information about map layers (eg. data sources, broken paths, definition queries) within an ArcMap map document (.mxd) using `arcpy.mapping` module or `pyqgis` module

### Python

At this point, you should be familiar with:

* variables of different data types (numeric, string, Boolean, date etc.)
* data structures of different types (list, tuple, dictionary, set)
* `for` and `while` loops, `if-elif-else` blocks
* import of external Python modules and packages (eg. `import os`)
* functions and how they work (eg. input arguments and `return` statement)
* reading/writing text files using the built-in `open` function
* reading/writing `.csv` files using the `csv` module and `unicodecsv` module

### Exercises

This section contains examples of tasks that you might need to write at some point of time. Implementing these tasks in Python code would be a good sign that you have mastered the basics of Python for GIS.

* get a list of field names of Date type in a file geodatabase feature class
* copy multiple shapefiles into a file geodatabase at once
* re-project all rasters in a folder copying the results into a new folder
* update data sources for layers in a map document and save a new map document
* write to a `.txt` or a `.csv` file information about your GIS assets

---

# Intermediate

## Resources

* Learn about [various Python IDEs](https://wiki.python.org/moin/IntegratedDevelopmentEnvironments) and find out which one you like most. Many start with free [PyScripter](https://sourceforge.net/projects/pyscripter/) and then move to something else:
  * SO question [What IDE to use for Python?](http://stackoverflow.com/questions/81584/what-ide-to-use-for-python)
  * Check PyCharm, WingIDE, Eclipse PyDev, Visual Studio Code, Python Tools for Visual Studio, or rich text editors such as [Sublime with Python support](https://www.fullstackpython.com/sublime-text.html)
  * Check Esri blog post [Choosing the right Python Integrated Development Environment](https://blogs.esri.com/esri/arcgis/2013/06/24/choosing-the-right-python-integrated-development-environment/)

Now, for getting started with Python development, [Visual Studio Code with Python](https://code.visualstudio.com/docs/languages/python) extension(s) is arguably the best choice. It's completely free, you can install it on any of your physical or virtual machines and it has great support for Python development. Choosing between commercial IDEs, Wing IDE or PyCharm would be a great choice.

* Learn about [VCS](https://en.wikipedia.org/wiki/Version_control) such as `Git` for managing the source code. [BitBucket](https://bitbucket.org/product) by Atlassian and [GitLab](https://about.gitlab.com/gitlab-com/) provides free private repositories and [GitHub](https://github.com/) provides free public repositories (you need to pay to create private ones).
  * Find out whether there is a VCS solution deployed in-house within your organization, such as [Microsoft TFS](https://www.visualstudio.com/tfs/), which you could use to check in the code
  * Should you like to dive deeper into `Git`, read the [Git Pro book](https://git-scm.com/book/en/v2) for free online

* Watch Python courses on training sites such as Pluralsight [Python Fundamentals](https://app.pluralsight.com/library/courses/python-fundamentals/table-of-contents, Enthought [Python Foundation Series](https://www.enthought.com/services/training/python-training-on-demand/) or [Safari Books online](https://www.safaribooksonline.com/)
* Watch Esri video [Python: Useful Libraries for the GIS Professional](http://www.esri.com/videos/watch?videoid=2938&isLegacy=true&title=python-useful-libraries-for-the-gis-professional)

* Learn about [type hinting in Python](https://docs.python.org/3/library/typing.html). There is an [excellent blog post on how type hints are used in PyCharm](https://www.jetbrains.com/help/pycharm/type-hinting-in-pycharm.html) and a [help page from Wing IDE people](https://wingware.com/doc/edit/helping-wing-analyze-code). Find out  whether your Python IDE supports static code analysis and start using the type hints (with support both for Python 2.7 and 3.5+).
  * Learn about [MyPy static type checker](http://mypy-lang.org/) and support for type hints with the [`typing`](https://docs.python.org/3/library/typing.html) module in Python 3.6

* Learn how run other Python programs or executable files from your program using `subprocess` module. This is handy when you need to run an `.exe` program in the middle of your Python program. This is often the case when you use `arcpy` / `ogr` code in the beginning of the script, but then need to run ArcObjects console app / compiled C++ app to get something done before you can proceed further.

### Tutorials / web pages

* Esri blog [Generating a choice list from a field](https://blogs.esri.com/esri/arcgis/2011/08/25/generating-a-choice-list-from-a-field/) for a custom script tool
* [Python and GIS blog 1](https://pymorton.wordpress.com/) and [Python and GIS blog 2](https://pythongisandstuff.wordpress.com/)
* Convert ArcGIS script toolbox (.tbx) to Python toolbox (.pyt) with [tbxtopyt](https://github.com/jasonbot/tbxtopyt)
* Esri blog [How to Debug Python Toolboxes in 3 Easy Steps](https://blogs.esri.com/esri/arcgis/2012/12/14/how-to-debug-python-toolboxes-in-3-easy-steps/)
* Esri blog [Field mapping and Python scripting](https://blogs.esri.com/esri/arcgis/2012/08/30/field-mapping-and-python-scripting/)
* Esri [ArcPy team blog](https://arcpy.wordpress.com/)
* Convenience functions for `arcpy` in repo [arcapi](https://github.com/NERC-CEH/arcapi)
* Sample ArcGIS toolbox [SampleArcPyMappingScriptTools_10_v1](http://www.arcgis.com/home/item.html?id=18c19ec00acb4d568c27bc20a72bfdc8) for working with `arcpy.mapping` (20+ tools)
* Learn how to use [pip](http://stackoverflow.com/questions/4750806/how-do-i-install-pip-on-windows) for managing Python packages
* Learn [`virtualenv`](https://virtualenv.pypa.io/en/stable/) and [`venv`](https://docs.python.org/3.6/library/venv.html) for managing Python 2  for Python 3 environments, respectively
* Learn `tox` and `retox` to run your tests/programs on multiple Python installations (can be handy when building script tools to be used both in ArcGIS Desktop with Python 2.7 and ArcGIS Pro with Python 3.x or QGIS with Python 2.7 and QGIS with Python 3.x)
* Learn [R-ArcGIS bridge](https://github.com/R-ArcGIS/r-bridge-install) to combine Python and R code

## Skills

### GIS specific

At this point, you should be able to:

* automate map production using `arcpy.mapping` with data-driven pages or `pyqgis`
* manage `.pdf` files (eg. re-ordering, merging, splitting) using `arcpy` or pure Python packages such as `pypdf2`
* export ArcMap map document layout to various file formats such as `.png` and `.pdf`
* update text elements content in layout of an ArcMap map document
* executing SQL queries from Python using `arcpy.ArcSDESQLExecute()` or `GDALDataset::ExecuteSQL()`
* use `FieldInfo`, `FieldMap`, and `FieldMappings` classes from `arcpy` or `ogr.FieldDefn()` to manage data schema changes
* customize custom ArcGIS script tool behavior using `ToolValidator` class or build simple QGIS plugins
* start using Python toolboxes and Python add-ins in ArcGIS when it makes sense
* debug `arcpy`-driven code with the help of geoprocessing messages
* writing smaller unit tests for GIS workflows
* handling `JSON` data in Python and `arcpy` and `GeoJSON` for `ogr`
* read Excel files using `xlrd` Python package
* generate simple Excel files from datasets with Python and [`xlsxwriter`](https://github.com/jmcnamara/XlsxWriter) package or [`xlwd`](https://github.com/python-excel/xlwt)
* using `arcpy.da.Walk()` and `os.walk()` to traverse folders with GIS datasets recursively

### Python

At this point, you should be familiar with:

* installing Python packages using `pip`
* PYTHONPATH environment variable and Python environment isolation
* Python 3 to be able to write code that will be ported later to ArcGIS Pro / QGIS 3.x
* Python [PEP-8](https://www.python.org/dev/peps/pep-0008/) style guide
* `collections` module data structures such as `defaultdict`, `namedtuple`, `Counter`
* list, dictionary comprehensions, and set comprehensions + set theory operations
* enumerating sequences using the built-in `enumerate` function
* writing own functions and handling the arguments with `*args` and `**kwargs`
* [lambda/anonymous](https://en.wikipedia.org/wiki/Anonymous_function) and [convenience](https://en.wikipedia.org/wiki/Convenience_function) functions
* accessing DBMS databases using Python
* working with disk-based databases such as `SQLite` from Python
* using non-Latin characters in the source file, handling Unicode, encoding shebang
* Python exceptions and `try/except` block
* Python `traceback` module
* tuple unpacking with function calls
* sending emails with Python
* accessing ftp sites with Python using `ftplib` module
* running Python files with the `cmd` and a task scheduler
* zipping folders and files with Python and reading/unpacking archive files (using `zipfile` module for `.zip` files and `tarfile` for `.tar` and `.tar.gz` files)
* sending SMS using Python and `Twilio`
* logging your Python programs (using `logging` module) - handy to use instead of `print` statements

---

# Advanced

## Resources

### GIS specific

* Learn how to use ArcObjects from Python:
  * GIS.SE [Accessing ArcObjects from Python?](http://gis.stackexchange.com/a/110/14435)
  * GIS.SE [Guidelines for using ArcObjects from Python](http://gis.stackexchange.com/questions/129456/guidelines-for-using-arcobjects-from-python)
  * Esri video [Extending Python Using C++ and ArcObjects](http://www.esri.com/videos/watch?videoid=1242&isLegacy=true&title=extending-python-using-c_plus__plus_-and-arcobjects)
  * Esri [recorded live-training seminar on ArcObjects](https://www.youtube.com/watch?v=AtwD02wyP3A)
  * Esri Help page [Learning ArcObjects](http://resources.arcgis.com/en/help/arcobjects-net/conceptualhelp/#/Learning_ArcObjects/0001000000p1000000/) will help you determine which ArcObjects will provide the functionality required by your customization
  * Esri Help page [Reading OMDs](http://resources.arcgis.com/en/help/arcobjects-net/conceptualhelp/#/Reading_OMDs/000100000306000000/) provides a description of the diagram notation used on the ArcObjects object model diagrams (OMDs)
  * Blog post [Accessing ArcObjects in Python](https://tereshenkov.wordpress.com/2016/01/16/accessing-arcobjects-in-python/)
  * [GitHub repo](https://github.com/hellocomrade/ArcObject) with tutorial on ArcObjects

* Learn how to access ArcGIS Pro .NET libraries from Python:
  * Learn the basics of C# or VB.NET
  * Learn to use the [`pythonnet`](https://pypi.python.org/pypi/pythonnet/2.1.0) package
  * Learn to build a class library to access its methods from Python using `clr`
  * Learn how to build a console app that would embed Pro libraries in [Pro .NET SDK Help](https://github.com/Esri/arcgis-pro-sdk/wiki/proconcepts-CoreHost)

* Learn about other GIS packages:
  * Go through a comprehensive list of [Essential Python Geospatial Libraries](http://carsonfarmer.com/2013/07/essential-python-geo-libraries/) (also available on [this GitHub page](https://github.com/SpatialPython/spatial_python/blob/master/packages.md))
  * Watch the series of recorded workshops on using open source GIS packages: [Geospatial data in Python: Database, Desktop, and the Web](http://pyvideo.org/speaker/carson-farmer.html)
  * Watch the series of various talks on using open source GIS packages: [Geospatial Python talks](http://pyvideo.org/search.html?q=geospatial)

* Learn about how to build desktop GUI applications using Tkinter, WxPython, PyQt, PySide, or Kivy and then embed them into ArcGIS or just let them be aware of spatial datasets:
  * [Python Add-Ins and Tkinter](http://anothergisblog.blogspot.se/2013/07/python-add-ins-and-tkinter.html)
  * Esri blog post [Using Python and QML to build native apps](https://blogs.esri.com/esri/arcgis/2015/11/16/using-python-and-qml-to-build-native-apps/)
  * [GitHub repo](https://github.com/ldanzinger/PyOtherSideForArcGIS) with samples for ArcGIS, Qt and Python integration
  * Watch Esri video [Developing Custom Tools with PyQt](http://www.esri.com/videos/watch?videoid=4549&isLegacy=true&title=developing-custom-tools-with-pyqt)
  * Go through examples of PyQt applications on the [Riverbank GitHub page](https://github.com/baoboa/pyqt5/tree/master/examples)
  * Explore the workflow of [building a custom QGIS plugin with PyQt](https://docs.qgis.org/2.0/en/docs/pyqgis_developer_cookbook/plugins.html)
  * Explore PyQt5 desktop application for executing SQL queries against Esri file geodatabases [GDBee](https://github.com/AlexArcPy/GDBee)

* Learn about [computational geometry](https://en.wikipedia.org/wiki/Computational_geometry) and find out how it can help you in your work. Maybe you could use a tool that is not present in your desktop GIS or you are looking for something that performs faster. There are two main computational geometry libraries and both were written in C:
  * [qhull](http://www.qhull.org/). Its Python wrapper is accessed via [`scipy.spatial`](https://docs.scipy.org/doc/scipy/reference/tutorial/spatial.html) module, an exceptional tool for anyone who deals with geometrical data.
  * [CGAL](https://www.cgal.org/index.html). Its [Python bindings](https://pypi.python.org/pypi/cgal-bindings) are generated with `SWIG`. The `CGAL` is somewhat difficult to install and compile, but does provide much richer functionality.
  * Watch [Computational Geometry in Python - PyCon 2016](https://www.youtube.com/watch?v=nb3GRgtjlTw) and [Python Powered Computational Geometry](http://pyvideo.org/pycon-au-2012/python-powered-computational-geometry.html) to learn more about `qhull` and `CGAL`, respectively.

* Learn about using Python with [FME Desktop](https://www.safe.com/fme/fme-desktop/):
  * Find out [how to run an FME workbench from Python](https://knowledge.safe.com/articles/1158/run-an-fme-workspace-from-python-using-fmeworkspac.html)
  * Find out how to call Python code from within an FME workbench using [PythonCaller transformer](https://docs.safe.com/fme/2017.1/html/FME_Desktop_Documentation/FME_Transformers/Transformers/pythoncaller.htm)
  * Find out how to process data without using any FME workbench with the help of [FME Objects Python API](https://docs.safe.com/fme/html/FME_Objects_Python_API/index.html)

* Learn the ArcGIS REST API:
  * Learn [`requests`](http://docs.python-requests.org/en/master/) module
  * ArcGIS toolbox [ArcGIS Server Administration Toolkit - 10.1+](http://www.arcgis.com/home/item.html?id=12dde73e0e784e47818162b4d41ee340)
  * Learn [ArcGIS Python API](https://developers.arcgis.com/python/) to manage ArcGIS Online / Portal organizations and ArcGIS Server resources

* Learn about managing and processing larger spatial datasets as performance will matter:
  * Learn profiling techniques to find out what code takes most time to execute (`cProfile`)
  * Learn benchmarking to compare execution time for functions that do the same thing using different tools (eg. looking for the fastest way to count points in polygons)
  * Read Esri blog [Accessing Multidimensional Scientific Data using Python](https://blogs.esri.com/esri/arcgis/2015/06/10/accessing-multidimensional-scientific-data-using-python/)
  * Learn how to use `multiprocessing` module with ArcGIS at Esri blog post [Multiprocessing with ArcGIS – Approaches and Considerations (Part 1)](https://blogs.esri.com/esri/arcgis/2012/09/26/distributed-processing-with-arcgis-part-1/)
  * Read Esri blog [Be successful overlaying large, complex datasets in Geoprocessing](https://blogs.esri.com/esri/arcgis/2012/06/15/be-successful-overlaying-large-complex-datasets-in-geoprocessing/)

* Learn about using Python for Big Data management and analysis
  * Learn about [`PySpark`](https://spark.apache.org/docs/2.3.0/api/python/pyspark.html) that will let you use Spark in Python as well as [various geospatial libraries](https://gist.github.com/4rzael/bbd543af0cb2ee087771f42c5aefdad7) that will let you do geospatial analysis using Spark: [`magellan`](https://github.com/harsha2010/magellan), [`spatialspark`](https://github.com/syoummer/SpatialSpark), and [`GeoSpark`](https://github.com/DataSystemsLab/GeoSpark/)
  * Watch a video showcasing use of Spark for large data analysis: [Large Scale Geospatial Analytics with Python, Spark, and Impala](https://youtu.be/L_uJvLKHgEs)
  * Read an article showcasing use of `Hadoop` and `Presto` for large data analysis at Uber: [Query the planet: Geospatial big data analytics at Uber](https://www.oreilly.com/ideas/query-the-planet-geospatial-big-data-analytics-at-uber)
  * Learn about [Presto geospatial functions](https://prestodb.io/docs/current/functions/geospatial.html) and [Presto Python client](https://github.com/prestodb/presto-python-client)
  * Learn about [Omnisci geospatial Map-d core](https://github.com/omnisci/mapd-core) and its [Python JayDeBeApi](https://www.omnisci.com/docs/latest/6_jaydebeapi.html)
  * Learn about [Geomesa](https://www.geomesa.org/) and its [integration with the Spark Python API for accessing data in GeoMesa data stores](https://www.geomesa.org/documentation/user/spark/pyspark.html)
  * Become familiar with [Esri Geometry API for Java](https://github.com/Esri/geometry-api-java) as it is used by many Java-based Big Data platforms that provide some kind of geospatial support

* Learn about [Esri File Geodatabase C++ API](https://github.com/Esri/file-geodatabase-api) with .NET bindings to be able to work with file geodatabases programmatically using C++ or .NET 
  * Learn how to use `ESRI File Geodatabase (OpenFileGDB)` and `ESRI File Geodatabase (FileGDB)` GDAL drivers to connect to Esri file geodatabase programmatically or using open-source tools
  * Explore an example of using `GDALDataset::ExecuteSQL()` in a PyQT desktop SQL editor [`GDBee`](https://github.com/AlexArcPy/GDBee)

### Python

* Learn how Python is used in the enterprise watching the [Enterprise Software with Python](https://player.oreilly.com/videos/9781491943755) O'reilly video course

* Learn [IPython](https://ipython.org/) and the concept of reproducible research:
  * Learn how to use [Jupyter notebook](http://jupyter.org/)
  * Learn how to combine [Python and R code](https://www.continuum.io/blog/developer/jupyter-and-conda-r) in the same Jupyter notebook

* Learn about using Python for web development:
  * Learn [`flask`](http://flask.pocoo.org/) and [`django`](https://www.djangoproject.com/). Start with `flask` and only then move to `django`
  * Learn [`geodjango`](https://docs.djangoproject.com/en/1.10/ref/contrib/gis/) to serve spatial datasets on the web. Read through slides [ArcGIS JavaScript Plus Django Equals Dynamic Web App](http://proceedings.esri.com/library/userconf/proc15/papers/794_139.pdf)

* Watch [Python – Beyond the Basics](https://app.pluralsight.com/library/courses/python-beyond-basics/table-of-contents) on Pluralsight
* Learn about [`nlpk`](http://www.nltk.org/) Python package to work with human language data (eg. parsing address data)
* Learn about [`regex`](https://docs.python.org/2/howto/regex.html) Python package to work with regular expressions in Python (eg. finding addresses in a specific format)
* Learn about [`difflib`](https://docs.python.org/3.5/library/difflib.html) and [`Levenshtein C extension`](https://rawgit.com/ztane/python-Levenshtein/master/docs/Levenshtein.html) to do fuzzy string matching (eg. finding the closest address string in the registry for an input address)
* Learn [`Selenium`](https://github.com/SeleniumHQ/Selenium) Python package to be able to automate web app testing. Read the docs for Python bindings [here](http://www.seleniumhq.org/docs/03_webdriver.jsp#introducing-the-selenium-webdriver-api-by-example)

* Learn about numerical computing and data science:
  * Install [`Anaconda`](https://www.continuum.io/downloads) and learn about `conda`. This is helpful as [Python in ArcGIS Pro](https://geonet.esri.com/docs/DOC-8359) is implemented using a [conda](http://conda.pydata.org/docs/test-drive.html) environment
  * Install [Enthought Canopy](https://www.enthought.com/products/canopy/) scientific Python distribution and learn what tools it has
  * Learn numerics, science, and data with Python with [scipy-lectures](http://www.scipy-lectures.org/)
  * Learn what [`scipy.spatial`](https://docs.scipy.org/doc/scipy/reference/spatial.html) can do for your GIS work
  * Read [Python for Data Analysis](http://shop.oreilly.com/product/0636920023784.do) and [Python for Computational Science and Engineering](https://www.southampton.ac.uk/~fangohr/training/python/pdfs/Python-for-Computational-Science-and-Engineering.pdf) (free book)

* Learn about connecting to various DBMS from Python:
  * For Microsoft SQL Server - `pymssql`
  * For Oracle - `cx_Oracle`
  * For PostgreSQL - `psycopg2` or `sqlalchemy` 

* Learn about using machine learning with Python:
  * Start using [scikit-learn](http://scikit-learn.org/) for various GIS-related operations such as data classification and regression as well as [scikit-image](http://scikit-image.org/) for image processing (e.g., satellite imagery recognition)

* Learn about using computer vision (CV) with Python to do image processing:
  * Learn how to use the [`Pillow`](https://pillow.readthedocs.io/en/5.1.x/), [`OpenCV`](https://docs.opencv.org/3.0-beta/doc/py_tutorials/py_tutorials.html), and [`SimpleCV`](http://simplecv.org/) libraries. Start with `SimpleCV` first

* Learn about creating and parsing HTML:
  * Parse and construct HTML pages with Python using [`BeautifulSoup`](https://launchpad.net/beautifulsoup). Having this skill would be handy when a web page should be searched for some information and loaded into a GIS dataset or when you are building HTML reports
  * Learn how the [`registrant`](https://github.com/AlexArcPy/registrant) package reports information about the Esri geodatabase contents
  * Learn about web scraping using [`Scrapy`](https://scrapy.org/)

* Learn about creating and parsing XML:
  * Parse existing `.xml` files using built-in `xml.etree.ElementTree` class and 3rd party package [`lxml`](https://lxml.de/)

* Learn about source code testing, linting, and refactoring:
  * Learn `unittest` built-in module and more advanced [`pytest`](https://docs.pytest.org/en/latest/) framework
  * Learn [`coverage.py`](https://coverage.readthedocs.io/en/coverage-4.4.1/) module to create code coverage reports
  * Learn [`Hypothesis`](https://hypothesis.readthedocs.io/en/latest/) for writing more powerful unit tests
  * Learn Python linters such as `pylint`, `flake8`, and `pyflakes8` to keep the code tidy
  * Learn about Python style guides such as [Google style guide](https://github.com/google/styleguide/blob/gh-pages/pyguide.md). This will be particular useful when you start working in a team
  * Learn about most comprehensive Python linter [`wemake-python-styleguide`
](https://github.com/wemake-services/wemake-python-styleguide). It is just a `flake8` plugin; however, it combines violations from a lot of other `flake8` plugins
  * Learn Python formatters such `yapf` and `autopep8` to automatically reformat the source code to conform to a style. It is best to run `autopep8` with aggressive option enabled to reformat the code and then run `yapf` on the result code
  * Learn [SonarPython](https://rules.sonarsource.com/python) static code analyzer to find code smells and refactoring options. Many of the rules from `SonarPython` are implemented in `wemake-python-styleguide`
  * Learn about Python interface files ([PEP-484](https://www.python.org/dev/peps/pep-0484/)) and how to use them to [help your Python IDE to do static code analysis](https://www.jetbrains.com/help/pycharm/type-hinting-in-product.html#pep484) and provide better intellisense

* Start looking for doing certain things outside of GIS applications using pure Python, for instance, using `pandas`

* Learn best practices for organizing configuration and settings for a larger workflow where you need to keep the config values separately from the business logic (eg. using `json`, `ConfigParser` or using OOP constructors)

* Learn about extending Python with C or C++:
  * Learn how to [create a C++ extension for Python](https://docs.microsoft.com/en-us/visualstudio/python/cpp-and-python) (`.pyd` compiled file that can be imported as a regular module into Python module)
  * Go through the [Interfacing with other languages](https://training.enthought.com/course/INTERFACING) course from Enthought to start building Python native modules
  * Learn and compare various [alternatives for wrapping C++ code for Python](http://intermediate-and-advanced-software-carpentry.readthedocs.io/en/latest/c++-wrapping.html) such as using [`Boost`](https://www.boost.org/), [`SWIG`](http://www.swig.org/), native [Python C API](https://docs.python.org/2/c-api/index.html), and [`pybind11`](https://github.com/pybind/pybind11). `pybind11` is the most user-friendly one

## Skills

### GIS specific

At this point, you should be able to:

* execute ArcObjects code from Python using `comtypes` library
* export the data from tables and feature classes into Excel with custom formatting using `xlsxwriter`
* generate `.pdf` files from scratch that would contain map images, custom charts, and tables using `reportlab`
* split, merge, crop, and transform `.pdf` documents using `pypdf2`
* generate `.pdf` report files using ArcGIS report templates (`.rlf`) and `arcpy`
* generate graphs using `arcpy.Graph`, `arcpy.GraphTemplate` with graph template files (`.tee`), and Make Graph GP tool
* perform graph theory operations on linear datasets using `networkx` (eg. point-to-point routing)
* plot geodata with `Matplotlib` (both vector and raster)
* use `numpy` and `pandas` for manipulating spatial dataset attribute table
* use `requests` and/or `arcrest` package to access ArcGIS Server site, ArcGIS Online / Portal organizations through the ArcGIS REST API
* call FME workbenches from Python
* access readers and writers in FME with `fmeobjects`
* read, modify, and write a georeferenced image
* generate useful information about a point dataset (most isolated points, a pair of two furthest points, etc)

### Python

At this point, you should be familiar with:

* building desktop GUI applications using PyQt, PySide, or Kivy (eg. visualize a shapefile's features in an application window)
* contributing to open-source projects such as `arcrest` or `geopandas` reporting bugs or pulling in new functionality
* creating new `conda` environments and installing various packages into specific environments
* refactoring wrapping the code into functions, modules, and packages
* OOP basics and creating own classes
* compile a simple Python extension module (`.pyd`) and write a `.pyi` interface file to provide the intellisense for your Python IDE

### Exercises

This section contains the examples of tasks that you might need to write at some point of time. Implementing these tasks in Python code would be a good sign that you have mastered the advanced concepts of Python for GIS.

* hide/show map grid of data frame in a map layout before exporting the map in a map document using `arcpy` package and ArcObjects
* update label's text of a scale bar in a map layout using pure ArcObjects
* generate a service area (drive-time) polygon for an arbitrary point on a street network stored as a shapefile using `networkx`
* find out the fastest spatial join - ArcGIS Spatial Join GP tool, `rtree` in PostGIS, SQL Server `STContains`, or `shapely` Python package
* create a new .csv file from an existing one by filtering certain rows using `pandas`
* classify point dataset features into clusters using `scikit-learn` to mimic some of the ArcGIS Spatial Statistics tools
* write a program that will calculate the area of a lake automatically recognized from a satellite imagery
* build with the help of `PyQt` a GUI application for executing SQL queries against file geodatabases
