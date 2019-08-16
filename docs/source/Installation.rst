
How to install Pyecog
==================================

While there is a package on pip, this has not been updated for a while, and will not work (probably). Please do not use it!

Also, please make sure to download the Development branch in the steps below.

Installation procedure with a conda environment (recommended)
---------------------------------------------------------------

1. Create a conda enviroment
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
First Install Anaconda (https://www.anaconda.com/distribution/#download-section). Choose the Python 3 version for your operating system (Linux, Windows, or OS X). You can also use the Python 2 version, but
be sure to use python=3.5 for the conda environment (next step).

Next make a new conda environment and install the dependencies for pyecog. To do this open a either the anaconda prompt if on windows or terminal if mac or linux and type or copy (triple click is helpful here).::

    conda create --name pyecog_env python=3.5 jupyter=1 scipy=0.18.1 numpy=1.11.2 scikit-learn=0.18.1 pandas=0.19.2 matplotlib=2 seaborn=0.7.1 h5py=2.8.0 xlrd=1 pyqt=5.6 numba=0.37.0

Follow the prompts in the terminal window, and when finished activate the environment you have just created. If on windows, type 'activate pyecog_env', or mac/linux 'source activate pyecog_env'::

    source activate pyecog_env  # or just "activate pyecog_env" if you are on windows

Then install pyqtgraph::

    pip install pyqtgraph==0.10

2. Download Pyecog from Github
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Click on the green "clone or download" button on the top right of the github project page: https://github.com/jcornford/pyecog/tree/Development.

Download the zip file and extract it somewhere on your computer.


3. Running the Graphical Interface
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Navigate to the folder where you have extracted Pyecog in anaconda prompt/ terminal - e.g cd ~/Desktop/pyecog-Development. The command 'cd' is for change directory.

Activate your python environment if needed. If on windows, type 'activate pyecog_env', or mac/linux 'source activate pyecog_env'::

    activate pyecog_env  # or  "source activate pyecog_env" if on a mac

Finally run the gui with::

    python start.py


Installing without a virtual python environment
------------------------------------------------
Instead of::

    conda create --name pyecog_env python=3.5 jupyter=1 scipy=0.18.1 numpy=1.11.2 scikit-learn=0.18.1 pandas=0.19.2 matplotlib=2 seaborn=0.7.1 h5py=2.8.0 xlrd=1 pyqt=5.6 numba=0.37.0

Replace with::

    conda install jupyter=1 scipy=0.18.1 numpy=1.11.2 scikit-learn=0.18.1 pandas=0.19.2 matplotlib=2 seaborn=0.7.1 h5py=2.8.0 xlrd=1 pyqt=5.6 numba=0.37.0

 And then do not activate an enviroment. Follow other steps as before.

