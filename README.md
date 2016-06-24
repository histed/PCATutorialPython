# Principal Components Analysis Tutorial, using Python

This tutorial can help you teach yourself how to do principal components analysis using Python.     *Quickstart*: Click here to try it online!  (Note: may take 30 sec to load, and this online version will not save changes; you must install - see below)  [![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/histed/PCATutorialPython)

As example data, we use extracellular neuron spike waveforms, recorded from a silicon recording electrode in mouse visual cortex.  Data is sampled at around 30 kHz.  Each waveform is a vector of length nTimepts (nTimepts is about 50, total waveform duration is about 1.5 ms).

PCA finds new vectors that give the directions in a vector space (in this case the space of dimension nTimepoints, in which each waveform is a single point) that maximize the variation of the data points, subject to orthogonality constraints.  In short, the result of the PCA will be several clouds of points, where each cloud contains points with related waveform shapes.  Exploring the tutorial exercises will help you understand those PCA results.

The tutorial uses the Jupyter notebook as a user interface.  It uses the nice [Seaborn](https://web.stanford.edu/~mwaskom/software/seaborn/) Python library to make the plots look good.  And it uses the standard scientific python tools numpy and matplotlib.

## Quick, online tutorial preview

You can use the excellent [Binder](http://mybinder.org) tool to run this tutorial code completely with your browser.  Nothing needs to be installed on your computer.  However, the online version will not save changes.  If you want to do the exercise, you must install. To try online, press this button: [![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/histed/PCATutorialPython)
(Thanks to Jeremy Freeman for the Binder tool.)


## Installing

Instructions for Mac OS X.

First, [install Anaconda](https://docs.continuum.io/anaconda), a nicely packaged version of the Python scientific stack.
- First, download the Python 3.5 command line installer.  Then run:
````
bash ~/Downloads/Anaconda3-4.0.0-MacOSX-x86_64.sh
````
- Approve the license
- Install to anaconda3 in your home directory: /Users/yourusername/anaconda3

Next, to install all the required libraries and start the tutorial, run the following from a command line after changing to your desired working directory:
````
source ~/anaconda3/bin/activate root
git clone https://github.com/histed/PCATutorialPython.git
cd PCATutorialPython
conda env create
source activate PCATutorialPython
````
To open the notebook:
````
jupyter notebook PCATutorialPython.ipynb
````

## Contacts

* Bradley Akitake bakitake.nih@gmail.com
* Mark Histed mhisted@gmail.com

send questions to code@histedlab.org






### License 

This work is in the public domain.





