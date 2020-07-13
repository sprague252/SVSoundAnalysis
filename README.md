# ECU Summer Ventures Jupyter Notebooks for Sound Analysis in Python

## Introduction

This repository contains Jupyter notebooks that use *Python* to do basic sound analysis including importing WAV files, ploting waveforms, and computing and plotting power spectra and spectrograms.  There are two example Jupyter notebooks. One uses Matplotlib to produce static images, and the other uses Plotly to produce interactive images. The Matplotlib/static image notebook requires less memory and computer porcessing to produce images. Also, the static images can be readily imported into presentations and papers.  The interactive images require more computer resources to produce and save. They are good for exploring the details of a plot because the user can zoom and pan the plot without re-plotting. Plotly/interactive plots can be exported to Javascript-enabled HTML files that can be opened in most browsers or included in webpages, but exporting Plotly images to static files requires the Plotly-Orca library which is not readily installed on cloud servers like *Azure Notebooks*.

## Files

* Beats.wav - sound recording of beats produced by two tuning forks vibrating at different frequencies. Included as an example sound recording to analyze.

* OrganPipeOpenClosed.wav - sound recording of a tube (organ pipe) alternating between playing with both ends open and one end closed. There is also a voice speaking on the recording. Included as an example sound recording to analyze.

* README.md - This file.

* Sound Analysis-Interactive Figures.ipynb - Jupyter notebook that demonstrates sound analysis using Plotly to produce interactive figures.

* Sound Analysis-Static Figures.ipynb - Jupyter notebook that demonstrates sound analysis using Matplotlib to produce static figures.

* requirements.txt - List of additional packages to install when this project is imported into *Azure Notebooks*. Azure Notebooks reads this file and installs these packages automatically.

## Running Code

### Run on local computer

In order to run these Jupyter notebooks on a local computer, you must have a version of Python 3.6 or greater with Jupyter installed (recommendation: Anaconda Python) with these additional packages:

1. numpy
2. scipy
3. matplotlib
4. plotly
5. svsound - install this with `conda install -c sprague252 svsound` or with `pip install svsound`.

### Run on Azure Notebooks

Azure Notebooks is a cloud service that will run Jupyter notebooks without any need to install software on a local computer. Azure Notebooks is a free preview service that will be ending in September, but anyone with a Microsoft or ECU account can use it until then.

Press the button to import this project onto Azure Notebooks: [![Azure Notebooks](https://notebooks.azure.com/launch.png)](https://notebooks.azure.com/import/gh/sprague252/SVSoundAnalysis) Sign in with a Microsoft (or ECU) account. Follow the prompts to import the repository.  Click the run button on the upper right, and then open the notebooks `Sound Analysis-Static Figures.ipynb` and/or `Sound Analysis-Interactive Figures.ipynb`.