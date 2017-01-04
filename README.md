# python-for-gis-progression-path
Progression path for a GIS analyst who wants to become proficient in using Python for GIS: from apprentice to guru

**This is a work in progress**

This is an attempt to provide a structured collection of resources that could help a GIS professional to learn how to use Python when working with spatial data management, mapping, and analysis. The resources are organized by progress category so basically everyone should be able to learn something new along the way.

The resources will include books, web pages and blog posts, online courses, videos, Q/A from GIS.SE, links to code snippets, and some bedtime readings. 

_The resources will focus mostly on learning about Python for users of Esri software though there will be some links that will apply even for open-source GIS professionals._

# Beginner

You should be able to write short simple scripts in pure Python with no connection to GIS. To learn the basics of Python, you can find a ton of resources online such as [CodeAcademy](https://www.codecademy.com/learn/python), [Learn Python the Hard Way](https://learnpythonthehardway.org/book/intro.html), [Dive into Python](http://www.diveintopython3.net/installing-python.html), [A Whirlwind Tour of Python](http://www.oreilly.com/programming/free/a-whirlwind-tour-of-python.csp), and many other books from [Python.org](https://wiki.python.org/moin/IntroductoryBooks).

## Resources
If you don't want to learn Python this way and would rather like to catch up learning how Python can be used for GIS:
* Book [Python Scripting for ArcGIS](https://www.amazon.com/Python-Scripting-ArcGIS-Paul-Zandbergen/dp/1589483715) for Esri users. Going through this book is sufficient to learn everything you might ever need;
* Book [Geoprocessing with Python](https://www.manning.com/books/geoprocessing-with-python) for open-source users;
* Esri instructor-led course [Introduction to Geoprocessing Scripts Using Python](https://www.esri.com/training/catalog/57630435851d31e02a43f054/introduction-to-geoprocessing-scripts-using-python/);


## Skills

### GIS specific
At this point, you should be able to:
- write some simple scripts either using `arcpy` site-package or `ogr/gdal` libraries;
- report information about your GIS assets (data format, geometry type, data schema, spatial reference);
- write code for calling ArcGIS GP tools from Python code and inspect the `Result` object returned;
- perform an operation on multiple datasets in batch mode using `arcpy` listing functions;
- read and update attributes & geometry of features using `arcpy.da` cursors;
- create and operate `arcpy.Geometry()` objects (accessing both their properties and methods);
- create an ArcGIS toolbox with a simple script tool executing a Python source file;
- report information about map layers (eg. data sources, broken paths, definition queries) within an ArcMap map document (.mxd) using `arcpy.mapping` module.

### Python
At this point, you should be familiar with:
- variables of different data types (numeric, string, date etc.);
- data structures of different types (list, tuple, dictionary, set);
- `for` and `while` loops, `if-elif-else` blocks;
- import of external Python modules and packages (eg. `import os`);
- functions and how they work (eg. input arguments and `return` statement);
- reading/writing of text files using the `os` module;

### Exercises
This section contains the examples of tasks that you might need to write at some point of time. Implementing these tasks in Python code would be a good sign that you have mastered the basics of Python for ArcGIS.
- get a list field names of Date type in a file geodatabase feature class;
- copy multiple shapefiles into a file geodatabase at once;
- re-project all rasters in a folder;
- update data sources for layers in a map document and save a new map document;
- write to a .txt or a .csv file information about your GIS assets;


# Intermediate

## Resources
* Learn about [VCS](https://en.wikipedia.org/wiki/Version_control) such as Git for managing the source code. [BitBucket](https://bitbucket.org/product) by Atlassian and [GitLab](https://about.gitlab.com/gitlab-com/) provides free private repositories and [GitHub](https://github.com/) provides free public repositories (you need to pay to create private ones).
 - Find out whether there is a VCS solution deployed in-house within your organization, such as [Microsoft TFS](https://www.visualstudio.com/tfs/), which you could use to check in the code;
 
* Watch [Python Fundamentals](https://app.pluralsight.com/library/courses/python-fundamentals/table-of-contents) on Pluralsight;


## Skills
### GIS specific
- to automate map production using `arcpy.mapping` with data-driven pages;
- to manage .pdf files (eg. re-ordering, merging, splitting) using `arcpy`;
- to export ArcMap map document to various file formats such as .png and .pdf;
- update text elements content in layout of ArcMap map document;
- executing DBMS spatial functions from Python and using `arcpy.ArcSDESQLExecute()`;
- to use `FieldInfo`, `FieldMap`, and `FieldMappings` from `arcpy` to manage data schema
- customize custom ArcGIS script tool behavior using `ToolValidator` class;
- start using Python toolboxes and Python add-ins in ArcGIS when it makes sense;
- debug `arcpy`-driven code using geoprocessing messages
- writing unit tests for GIS workflows;
- handling JSON in Python and `arcpy`;
- generate simple Excel files from geodatasets with Python and `xlsxwriter` package;

### Python
At this point, you should be familiar with:
- Python 3 to able to write code that will be ported later to ArcGIS Pro;
- [Python style guide](https://www.python.org/dev/peps/pep-0008/);
- `collections` module data structures such as `defaultdict`, `namedtuple`, `Counter`
- list and dictionary comprehensions;
- set comprehensions and set theory operations;
- enumerating sequences using built-in `enumerate` function';
- writing own functions and handling the arguments;
- lambda functions;
- convenience functions such as those in [arcapi](https://github.com/NERC-CEH/arcapi);
- accessing databases using Python;
- working with disk-based database SQLite from Python;
- using non-Latin characters in the source file and handling Unicode;
- Python exceptions and `try/except` block;
- Python `traceback` module;
- tuple unpacking with function calls;
- send emails with Python;
- access ftp sites with Python;
- run Python files with the cmd;
- zip folders and files with Python;


# Advanced

## Resources
* Learn about how to use ArcObjects from Python:
 - [Accessing ArcObjects from Python?](http://gis.stackexchange.com/a/110/14435)
* Learn about other GIS packages. Go through a comprehensive list of [Essential Python Geospatial Libraries](http://carsonfarmer.com/2013/07/essential-python-geo-libraries/) (also available on [this GitHub page](https://github.com/SpatialPython/spatial_python/blob/master/packages.md). 
 - watch the series of recorded workshops on using open source GIS packages: [Geospatial data in Python: Database, Desktop, and the Web](http://pyvideo.org/speaker/carson-farmer.html)
 
* Learn about how to build desktop GUI applications using PyQt, PySide, or Kivy and then embed them into ArcGIS or just let them be aware of spatial datasets. 
 - Watch Esri video [Developing Custom Tools with PyQt](http://www.esri.com/videos/watch?videoid=4549&isLegacy=true&title=developing-custom-tools-with-pyqt).
* Learn about using Python for web development:
 - learn [`flask`](http://flask.pocoo.org/) and [`django`](https://www.djangoproject.com/). Start with flask and only then move to Django.
 - learn [`geodjango`](https://docs.djangoproject.com/en/1.10/ref/contrib/gis/) to serve spatial datasets on the web. Read through pdf [ArcGIS JavaScript Plus Django Equals Dynamic Web App](http://proceedings.esri.com/library/userconf/proc15/papers/794_139.pdf);

* Watch [Python – Beyond the Basics](https://app.pluralsight.com/library/courses/python-beyond-basics/table-of-contents) on Pluralsight; 
* Learn about [`nlpk`](http://www.nltk.org/) Python package to work with human language data (eg. parsing address data);
* Learn about [`regex`](https://docs.python.org/2/howto/regex.html) Python package to work with regular expressions in Python (eg. finding addresses in a specific format);

* Install `Anaconda`(https://www.continuum.io/downloads) and learn about `conda`. This is helpful as [Python in ArcGIS Pro](https://geonet.esri.com/docs/DOC-8359) is implemented using a [conda](http://conda.pydata.org/docs/test-drive.html) env. 

* Learn about managing and processing larger spatial datasets as performance will matter.
 - learn profiling techniques to find out what code takes most time to execute;
 - learn benchmarking to compare execution time for functions that do the same thing using different tools (eg. looking for the fastest way to count points in polygons);

* Start looking for doing certain things outside of ArcGIS such using `pandas` (eg. create a new csv file from an existing one by filtering certain rows without converting the csv file into a geodatabase table);

* Learn best practices for organizing configuration and settings for a larger workflow where you need to keep the config values apart from the business logic (eg. using JSON or ConfigParser or init() );

## Skills

### GIS specific
- execute ArcObjects code from Python using `comtypes` library;
- export the data from tables and feature classes into Excel with custom formatting using `xlsxwriter`;
- generate .pdf files from scratch that would contain map images, custom charts, and tables using `reportlab`; 
- generate .pdf report files using ArcGIS report templates (.rlf) and `arcpy`;
- generate graphs using `arcpy.Graph`, `arcpy.GraphTemplate` with graph template files (.tee), and Make Graph GP tool;
- perform graph theory operations on linear datasets using `networkx` (eg. point-to-point routing);
- plot geodata with `Matplotlib` (both vector and raster);
- use `numpy` and `pandas` for manipulating spatial dataset attribute table;
- use pure Python and `arcrest` package to access ArcGIS Server site, ArcGIS Online / Portal organizations through ArcGIS REST API;
- call FME workbenches from Python;
- access readers and writers in FME with `fmeobjects`;


### Python
- build desktop GUI applications using PyQt, PySide, or Kivy (eg. visualize a shapefile features in a window);
- contribute to open-source projects such as `arcrest` or `geopandas` reporting bugs or new functionality;
- create new conda environments and install various packages into specific environments;
- refactor existing code to use dictionaries for lookups instead of multiple `if-elif`;
- OOP basics and creating own classes;

### Exercises
This section contains the examples of tasks that you might need to write at some point of time. Implementing these tasks in Python code would be a good sign that you have mastered the advanced concepts of Python for ArcGIS.
- hide/show map grid of data frame in a map layout before exporting the map in a map document using `arcpy` package and ArcObjects;
- update label's text of a scale bar in a map layout using pure ArcObjects;
- generate a service area (drive-time) polygon for an arbitrary point on a street network stored as a shapefile;
- find out the fastest spatial join - ArcGIS Spatial Join GP tool, `rtree` in PostGIS, SQL Server `STContains`, or `shapely` Python package;
