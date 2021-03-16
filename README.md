# Exmaples of REST_API of ODT Flow Explorer

[ODT Flow Explorer: Extract, Query, and Visualize Global Human Mobility](http://gis.cas.sc.edu/GeoAnalytics/od.html)


# Install keplergl Python library in Windows

-- install GDAL, Shapely, and Fiona

Go go this [site](https://www.lfd.uci.edu/~gohlke/pythonlibs) and download the version your need. Then install these .whl files using:

```python
pip install GDAL_your_version.whl
pip install Shapely_your_version.whl
pip install Fiona_your_version.whl
```

If keplergl map does not show up in your Jupyter Notebook, see through this [post](https://www.gitmemory.com/issue/keplergl/kepler.gl/583/516724808).
 
The solution is:

1) Copy files in folder `C:\Users\GPU\AppData\Roaming\Python\Python37\site-packages\keplergl\static`  to `C:\ProgramData\Anaconda3\share\jupyter\nbextensions\keplergl-jupyter`
2) Copy file `keplergl-jupyter.json` to `etc/jupyter/nbconfig/notebook.d`

Please replace the path accordingly.

You can use jupyter --paths to check where jupyter install extensions:

```
$ jupyter --paths
config:
    /Users/Olivier/.jupyter
    /usr/local/anaconda3/etc/jupyter
    /usr/local/etc/jupyter
    /etc/jupyter
data:
    /Users/Olivier/Library/Jupyter
    /usr/local/anaconda3/share/jupyter
    /usr/local/share/jupyter
    /usr/share/jupyter
runtime:
    /Users/Olivier/Library/Jupyter/runtime
The flag --sys-prefix means extension are installed in this data folder:
```
 
