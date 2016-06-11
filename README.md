# Principal Components Analysis Tutorial, using Python

This tutorial can help you teach yourself how to do principal components analysis using Python.      *Quickstart*: click here to try it!  [![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/histed/PCATutorialPython)

As example data, we use extracellular neuron spike waveforms, recorded from a silicon recording electrode in mouse visual cortex.  Data is sampled at around 30 kHz.  Each waveform is a vector of length nTimepts (nTimepts is about 50, total waveform duration is about 1.5 ms).

PCA finds new vectors that give the directions in a vector space (in this case the space of dimension nTimepoints, in which each waveform is a single point) that maximize the variation of the data points, subject to orthogonality constraints.  In short, the result of the PCA will be several clouds of points, where each cloud contains points with related waveform shapes.  Exploring the tutorial exercises will help you understand those PCA results.

The tutorial uses the Jupyter notebook as a user interface.  It uses the nice [Seaborn](https://web.stanford.edu/~mwaskom/software/seaborn/) Python library to make the plots look good.  And it uses the standard scientific python tools numpy and matplotlib.

## Quick, online tutorial version

You can use the excellent [Binder](http://mybinder.org) tool to run this tutorial code completely with your browser.  Nothing needs to be installed on your computer.  Press this button: [![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/histed/PCATutorialPython)
(Thanks to Jeremy Freeman for the Binder tool.)


## Installing

First, [install Anaconda](https://docs.continuum.io/anaconda/install), a nicely packaged version of the Python scientific stack.
Then, to install all the required libraries and start the tutorial, run the following from a command line: (tested on Mac OS X only)
````
git clone https://github.com/histed/PCATutorialPython.git
cd PCATutorialPython
conda env create
source activate PCATutorialPython
````

## Contacts

* Bradley Akitake bakitake.nih@gmail.com
* Mark Histed mhisted@gmail.com

send questions to code@histedlab.org






### License 

This work is in the public domain.





