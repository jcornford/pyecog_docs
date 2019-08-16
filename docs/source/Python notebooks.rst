==================================
Pyecog as a python module
==================================

Currently the smoothest way to use pyecog is to combine python code and the GUI. While it is possible to do
everything in the GUI, it is a little clunky and any uncaught error will currently crash the program.

It is suggested to use jupyter notebooks for ndf to h5 file conversion, feature extraction and the training & applying
of classifiers. Furthermore, by interacting with the files through python directly you do not restrict your
analysis to pre-coded routines.

Loading the pyecog module
~~~~~~~~~~~~~~~~~~~~~~~~~~

The easiest place to place and run this notebook is from the pyecog directory downloaded from github, e.g. "pyecog-Development" as the pyecog module will be found in this folder. However, if you want to run the notebook from else where on your computer you first need to make sure that python can find the pyecog module using sys.path.append(). To do this modify and copy the following code into a cell and run it (shift+enter).
::
    import sys
    pyecog_path = 'home/jonathan/git_repos/pyecog' # replace this with the pyecog location
    sys.path.append(pyecog_path)

If you are on windows you have to deal with the problem that backslashes in your paths are treated escape characters by python. Prefixing the string with 'r' prevents this.
::
    pyecog_path_windows = r'home\jonathan\git_repos\pyecog' # replace this with the pyecog location


Example Jupyter notebooks for classification workflow
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
.. toctree::
   :maxdepth: 1

   Notebook 1 Loading and converting Ndf files to h5 files.ipynb
   Notebook 2 Adding features to h5 files.ipynb
   Notebook 3 Making a library and train classifier.ipynb
   Notebook 4 Training a classifier on a library.ipynb
   Notebook 4 Applying classifier to h5 files.ipynb

Example Jupyter notebooks for more general analysis
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
.. toctree::
   :maxdepth: 1

   custom h5 analysis
