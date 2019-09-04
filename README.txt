This file describes the contents of this folder accompanying the submission of the manuscript entitled "QuCAT: Quantum Circuit Analyzer Tool" to the Computational physics communications journal.

Note this folder is adapted for the purposes of this peer-review from our GitHub repository https://github.com/qucat/qucat and our project website https://qucat.org/

Installation
============

QuCAT requires an installation of python 3, which we highly recommend downlading and installing through Anaconda at https://www.anaconda.com/distribution/
The Hamiltonian generation in QuCAT also requires QuTiP, which can be easily installed after one has obtained Anaconda by following these instructions: http://qutip.org/docs/latest/installation.html

After the two above requirements are satisfied, one can install QuCAT from this folder by opening a terminal and navigating to this folder, then running the command:

pip install .

An internet connection is required as this command will try and download and install additional dependencies of QuCAT.
A user can also install the latest version of QuCAT from the internet (without having this folder) through the command 

pip install qucat

Sample input and output of a comprehensive test run
===================================================

For a comprehensive test run of QuCAT, we recommend going through our "basics" tutorial.
This is a "jupyter notebook" containing python code which highlights the different features of the library.
The results of running the notebook can be viewed by opening the file ./docs/tutorials/basics.html, and the latest 
version can be found in the tutorials section of our website at https://qucat.org/tutorials/basics.html
Instructions for running this tutorial oneself are given below.

Running the comprehensive test run oneself
===========================================

One can simply copy and paste the different python commands visible in the notebook ./docs/tutorials/basics.html into a python file and execute the python file, 
or open the notebook file and run the commands from there.
The notebook file is located at .\tutorials\basics.ipynb and it can be opened by opening a terminal, navigating to the .\tutorials\ folder, running the command

jupyter notebook

then clicking on the basics notebook in the browser which consequently opens.

User manual
===========

The user manual can be navigated by opening the ./docs/index.html file. 
The documentation contains information about installation, a documented lists of functions, tutorials and more. 
An updated version can be found online at https://qucat.org/

Description of all files and folders
====================================

- test.py   A file testing all the basic functionalities of this package to the attention of a reviewer.

- .\docs\   Contains the html documentation of the package, one can read the documentation by opening ./docs/index.html. The documentation contains nformation about installation, a documented lists of functions, tutorials and more. An updated version can be found at https://qucat.org/

- .\docs_src\   Contains some tutorials in the form of jupyter notebooks, an updated can be found on our website at https://qucat.org/tutorials/tutorials.html

- .\src\    Contains the package source code
    - .\src\.graphics\      Contains the graphical elements used by the graphical user interface
    - .\src\_constants.py   Defines constants used in the package
    - .\src\_generate_graphics.py   Generates the contents of the .\src\.graphics\ folder
    - .\src\_gui.py         The source code of the graphical user interface
    - .\src\_utility.py     Utility functions used in all the libraries
    - .\src\core.py         The core library functions
    - .\src\plotting_settings.py    Contains the settings invoked when plotting the circuit or its normal modes.

- .\tests\      Scripts used to unittest most of the functionalities of QuCAT, in practice these are executed automatically (thanks to the continuous integration tool "Travis") each times changes are commited to our Github repository. The test currently cover 86 percent of the code of the .\src\ folder.

- .\LICENSE     Licensing information for the package
- .\setup.py    Setup filed used by the Python package installer


