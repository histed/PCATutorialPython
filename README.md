# Principal Components Analysis Tutorial, using Python

This tutorial can help you teach yourself how to do principal components analysis using Python.     *Quickstart*: Click button to try online version!   [![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/histed/PCATutorialPython)  (Note: may take 30 sec to load.  Online version will not save changes; you must install locally.) 

As example data, we use extracellular neuron spike waveforms, recorded from a silicon recording electrode in mouse visual cortex.  Data is sampled at around 30 kHz.  Each waveform is a vector of length nTimepts (nTimepts is about 50, total waveform duration is about 1.5 ms).

PCA finds new vectors that give the directions in a vector space (in this case the space of dimension nTimepoints, in which each waveform is a single point) that maximize the variation of the data points, subject to orthogonality constraints.  In short, the result of the PCA will be several clouds of points, where each cloud contains points with related waveform shapes.  Exploring the tutorial exercises will help you understand those PCA results.

The tutorial uses the Jupyter notebook as a user interface.  It uses the nice [Seaborn](https://web.stanford.edu/~mwaskom/software/seaborn/) Python library to make the plots look good.  And it uses the standard scientific python tools numpy and matplotlib.

## Quick, online tutorial preview

You can use the excellent [Binder](http://mybinder.org) tool to run this tutorial code completely with your browser.  Nothing needs to be installed on your computer.  However, the online version will not save changes.  If you want to do the exercise, you must install. To try online, press this button: [![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/histed/PCATutorialPython)
(Thanks to Jeremy Freeman for the Binder tool.)


## Installing locally

Instructions are for Mac OS X.

[Anaconda](https://docs.continuum.io/anaconda) is a nicely packaged version of the Python scientific stack.
Follow [these directions to install Anaconda](https://docs.continuum.io/anaconda/install#anaconda-for-os-x-graphical-install).  Use the Python 3 Mac OS X 64-bit graphical installer.  You must select 'Install for me only'.

You may need to install Apple's Developer tools to use git.  To check, open a terminal window and type 'git'.  If a dialog prompts you to install the Developer Tools, do that next.

The tutorial uses Anaconda to install extra required python components.  To install them and start the tutorial, run the following from a Terminal prompt:
````
mkdir ~/Repositories  # change this if you want to put the code in a different location
cd ~/Repositories   # change this if you want to put the code in a different location
source ~/anaconda/bin/activate root
git clone https://github.com/histed/PCATutorialPython.git
cd PCATutorialPython
conda env create
source activate PCATutorialPython
````
Then, open the notebook, by typing in the same terminal window:
````
jupyter notebook PCATutorialPython.ipynb
````

The Jupyter notebook will pop up in a browser window.  If you don't see anything, check any open browsers.

## Contacts

* Bradley Akitake bakitake.nih@gmail.com
* Mark Histed mhisted@gmail.com

send questions to code@histedlab.org






### License 

This work is in the public domain.





