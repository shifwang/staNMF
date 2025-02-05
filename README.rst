Amy Campbell, 2016
Yu Wang, 2018

staNMF
------
Python 3 implementation of `Siqi Wu et al.'s 2016 stability NMF (staNMF)
<http://doi.org/10.1073/pnas.1521171113>`_

Package Contents
----------------

=========
staNMF.py
=========
staNMF.py class includes the necessary methods to perform stability
NMF on a user-specified .csv datase (see sourcecode/staNMF_Example for precise
usage instructions)

=================
staNMF_Example.py
=================
Example of staNMF demonstrated on Wu et al.'s 2016
drosophila spatial expression data between K=15 and K=30; Generates
sample factorizations, calculates instability index, and plots instability
against K

================
staNMF_driver.py
================
Driver script to run staNMF in parallel; can be called from the command line
using:
python staNMF_driver.py <k1> <k2> <reps1> <reps2> <folder> <filename> <function>
(See docstring for more specific instructions) 

============================
data/WuExampleExpression.csv
============================
sample dataset (also available for download `here
<http://insitu.fruitfly.org/cgi-bin/ex/insitu.pl?t=html&p=downloads>`_)


Installation
-------------
$ pip install staNMF

*Please note that staNMF requires SPAMs package (version 2.5), which is
available from* `Julien Mairal et al.
<http://spams-devel.gforge.inria.fr/downloads.html>`_ , or from Anaconda
using:

$ conda install -c conda-forge python-spams=2.5


Acknowledgements
----------------
This work was supported by The Gordon and Betty Moore Foundation’s Data-Driven
Discovery Initiative (GBMF 4552 to C.S.G.) and a grant from the National
Institutes of Health (R01 CA200854)
