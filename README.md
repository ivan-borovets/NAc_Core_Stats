# NAc_Core_Stats

This repository contains R script for analyzing data from the neuroscience experiment and plotting its results. 

After downloading the necessary libraries and pre-processing the data, preliminary mixed linear models were built. Diagnostics of the resulting models showed the possible presence of a non-linear relationship between the dependent and independent variables. The dependent variables were generally distributed with positive skewness, so three types of models were built, potentially normalizing the distribution of the residuals of the resulting regression models: with logarithmic transformation of the dependent variable and using square and cubic roots.

A diagnostic of the resulting models for all transformed dependent variables showed that the cubic root transformation is the best in both graphical and synthetic metrics. The distribution of residuals in the resulting models allows us to conclude their applicability in general.

Constructed models are placed in the "models" list. Their summaries are in the "results" list. The above list also contains the results of the contrast analysis we were interested in.

Lastly, the plotting of results was added. Before starting the "Plotting" chunk, make sure that you have selected the correct working directory. Significant differences in the resulting graphs are marked automatically.
