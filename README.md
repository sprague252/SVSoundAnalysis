# ECU Summer Ventures Jupyter Notebooks for Sound Analysis in Python

## Introduction

This repository contains Jupyter notebooks that use *Python* to do basic sound analysis including importing WAV files, ploting waveforms, and computing and plotting power spectra and spectrograms.  There are two example Jupyter notebooks. One uses *Matplotlib* to produce static images, and the other uses *Plotly* to produce interactive images. The *Matplotlib*/static image notebook requires less memory and computer porcessing to produce images. Also, the static images can be readily imported into presentations and papers.  The interactive images require more computer resources to produce and save. They are good for exploring the details of a plot because the user can zoom and pan the plot without re-plotting. *Plotly*/interactive plots can be exported to Javascript-enabled HTML files that can be opened in most browsers or included in webpages.


## Files

* Beats.wav - sound recording of beats produced by two tuning forks vibrating at different frequencies. Included as an example sound recording to analyze.

* OrganPipeOpenClosed.wav - sound recording of a tube (organ pipe) alternating between playing with both ends open and one end closed. There is also a voice speaking on the recording. Included as an example sound recording to analyze.

* README.md - This file.

* Sound Analysis-Interactive Figures.ipynb - Jupyter notebook that demonstrates sound analysis using Plotly to produce interactive figures.

* Sound Analysis-Static Figures.ipynb - Jupyter notebook that demonstrates sound analysis using Matplotlib to produce static figures.

* requirements.txt - List of additional packages to install when this project is imported into *Azure Notebooks*. Azure Notebooks reads this file and installs these packages automatically.

## Running Code

### Run on local computer

In order to run these Jupyter notebooks on a local computer, you must have a version of Python 3.6 or greater with Jupyter installed with these additional packages:

1. numpy
2. scipy
3. matplotlib
4. plotly
5. svsound - install this with `conda install -c sprague252 svsound` or with `pip install svsound`.

Clone this git repository from GitHub with the following command.
```
git clone https://github.com/sprague252/SVImageProcessing.git
```

Once you have everything configured, start Jupyter Notebook or Jupyter Lab and open either of the two notebooks described above. 

### Run on CoCalc

The files should be already installed in your [CoCalc](https://cocalc.com) Summer Ventures project. (Look in Handouts.) If not, you can open a Linux terminal and run the `git` command in the previous section to copy them. Once you have the files, open one of the two notebooks described above in CoCalc. Be sure to set the kernel to `Python 3 (system-wide)` because that contains all of the modules you will need.

### Run on Binder

Binder is a cloud service that allows users to run Jupyter notebooks from Github repositories (no account required). Binder will not save your files after you end your session, so be sure to download all of your results before closing.

Press this button to import this project onto Binder: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sprague252/SVSoundAnalysis/master)
