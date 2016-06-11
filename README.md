# PCA Tutorial, using Python

This is a notebook that can help you teach yourself how to do principal components analysis using Python.

As example data, the notebook uses extracellular neuron spike waveforms, recorded from a silicon recording electrode in mouse visual cortex.  Data is sampled at around 30 kHz.  Each waveform is a vector of length nTimepts (nTimepts is about 50, total waveform duration is about 1.5 ms).

PCA finds new vectors that give the directions in a vector space (in this case the space of dimension nTimepoints, in which each waveform is a single point) that maximize the variation of the data points, subject to orthogonality constraints.  In short, the result of the PCA will be several clouds of points, where each cloud contains points with related waveform shapes.  Exploring the tutorial exercises will help you understand those PCA results.

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





