# Code and data for: *Brain structure and activity predicting cognitive maturation in adolescence*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Generic badge](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.10494534-orange.svg)](https://doi.org/10.5281/zenodo.14832030)

## Introduction

This repository contains the code and data used in [Zhu et. al. 2024](https://www.biorxiv.org/content/10.1101/2024.08.23.608315v2.abstract) 'Brain structure and activity predicting cognitive maturation in adolescence.' 


Abstract of the paper:
>Cognitive abilities of primates, including humans, continue to improve through adolescence 1,2. While a range of changes in brain structure and connectivity have been documented 3,4, how they affect neuronal activity that ultimately determines performance of cognitive functions remains unknown. Here, we conducted a multilevel longitudinal study of monkey adolescent neurocognitive development. The developmental trajectory of neural activity in the prefrontal cortex accounted remarkably well for working memory improvements. While complex aspects of activity changed progressively during adolescence, such as the rotation of stimulus representation in multidimensional neuronal space, which has been implicated in cognitive flexibility, even simpler attributes, such as the baseline firing rate in the period preceding a stimulus appearance had predictive power over behavior. Unexpectedly, decreases in brain volume and thickness, which are widely thought to underlie cognitive changes in humans 5 did not predict well the trajectory of neural activity or cognitive performance changes. Whole brain cortical volume in particular, exhibited an increase and reached a local maximum in late adolescence, at a time of rapid behavioral improvement. Maturation of long-distance white matter tracts linking the frontal lobe with areas of the association cortex and subcortical regions best predicted changes in neuronal activity and behavior. Our results provide evidence that optimization of neural activity depending on widely distributed circuitry effects cognitive development in adolescence.

## Dependencies
This code relies on MATLAB(R2023b) and R version 4.2.2.

For MATLAB code, Statistics and Machine Learning Toolbox and Curve Fitting Toolbox are needed.

For R code, the following packages are needed:

dplyr

ggplot2

gratia

gridExtra

lubridate

mgcv

purrr

stringr

tidyr

xtable


## Reproducing the analyses

### Raw data processing
Scripts under the following folders are used to read raw data in .mat format from folder [data_raw](data_raw) to generate plots or plot data for subsequent use:

[behavior](behavior)

[firingmetrics](firingmetrics)

[dimensionality](dimensionality)

Read comments in each Matlab scripts for more info.

### GAM fitting and plotting
R notebooks in the folder [GAM](GAM) are used to read data in .csv format from folder [data](GAM/data) to fit GAM models and plot developmental trajectories in the paper.

Read comments in each R notebook for more info.

Before use, change the path to where the data is located.

Please make sure to thoroughly read the comments in the code to understand the functionality of each part. If you encounter any problems, please contact author [Junda Zhu](mailto:junda.zhu@vanderbilt.edu).

**This repository is actively maintained and the published version will be on [Zenodo](https://doi.org/10.5281/zenodo.14832030).**

## Contributors
* [Junda Zhu](mailto:jzhu.neuro@gmail.com)
* [Christos Constantinidis](mailto:christos.constantinidis.1@vanderbilt.edu) (Principal Investigator)

>Citation: to be updated...


## Funding

This work was supported by NIH grants R01 MH117996 and R01 MH116675.

## License 

MIT License

Copyright (c) 2024 Constantinidis Lab at Vanderbilt Univeristy

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
