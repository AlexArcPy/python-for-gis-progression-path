# python-for-gis-progression-path
Progression path for a GIS analyst who wants to become proficient in using Python for GIS: from apprentice to guru

**This is a work in progress**

This is an attempt to provide a structured collection of resources that could help a GIS professional to learn how to use Python when working with spatial data management, mapping, and analysis. The resources are organized by progress category so basically everyone should be able to learn something new along the way.

The resources will include books, web pages and blog posts, online courses, videos, Q/A from GIS.SE, links to code snippets, and some bedtime readings. 

_The resources will focus mostly on learning about Python for users of Esri software though there will be some links that will apply even for open-source GIS professionals._

# Beginner

You should be able to write short simple scripts in pure Python with no connection to GIS. To learn the basics of Python, you can find a ton of resources online such as [CodeAcademy](https://www.codecademy.com/learn/python), [Learn Python the Hard Way](https://learnpythonthehardway.org/book/intro.html), and [Dive into Python](http://www.diveintopython3.net/installing-python.html).

If you don't want to learn Python this way and would rather like to catch up learning how Python can be used for GIS:
* Book [Python Scripting for ArcGIS](https://www.amazon.com/Python-Scripting-ArcGIS-Paul-Zandbergen/dp/1589483715) for Esri users. Going through this book is sufficient to learn everything you might ever neeed;
* Instructor-led course [Introduction to Geoprocessing Scripts Using Python](https://www.esri.com/training/catalog/57630435851d31e02a43f054/introduction-to-geoprocessing-scripts-using-python/);
* Book [Geoprocessing with Python](https://www.manning.com/books/geoprocessing-with-python) for open-source users.

At this point, you should be able:
- to write some simple scripts either using arcpy site-package or `ogr/gdal` libraries;
- to report information about your GIS assets (data format, geometry type, data schema, spatial reference);
- to write code for calling ArcGIS GP tools from Python code;
- to perform an operation on multiple datasets in batch mode using `arcpy` listing functions (eg. copy multiple shapefiles into a file geodatabase at once, re-project all  rasters in a folder);
- to read and update attributes & geometry of features using `arcpy.da` cursors;
- to create and operate `arcpy.Geometry()` objects (accessing both their properties and methods);
- to create an ArcGIS toolbox with a script tool executing a Python source file;
- to report information about map layers (eg. data sources, broken paths, definition queries) within a map document (.mxd) using `arcpy.mapping` module.




