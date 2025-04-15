# Geosciences_sp25

Here is documented the data, code, and initial results for the final project of GLY 6932. 

# Overview 

The goal of this project was to investigate the frequency of occurences of different sizes of Earth impactors. We know that very large impacts are rare, 
and that small impacts are common - but to what extent? How frequently might we expect a considerable impact? 
I ended up fitting the data to a generalized Pareto distribution (GPD), which is good for modeling the 'tail' or 'extreme' events. This was based on a threshold 
of the 95th percentile of data points, which is a parameter of the distribution and can be varied for other applications. I compared these results with a simple 
Pareto distribution, and the GPD result had about half the error. This is the fit I used to determine the expected period between Chelyabinsk-like events, which 
is the largest impact in the dataset, and the highest energy impact in recent and well-documented history. Ironically, I had to remove the actual observation from 
the dataset because it was such an extreme outlier. I determined that we might expect to see such an event once in a ~300 year period. Since my set only spans about 
37 years, it was getting weighted too heavily. 

# Figures Produced 
<img src ="/images/GStat-sim_master_figure.png" align = "center">

# Datasets

The data used is from NASA’s Jet Propulsion Laboratory, Center for Near Earth Object Studies. 
Over 1,000 events have been documented since 1988, and can be accessed here: https://cneos.jpl.nasa.gov/fireballs/ .
The data can simply be downloaded as a csv file.
The primary measurement that is evaluated here is the "Calculated Total Impact Energy (kt)". 

# Package dependencies

* Numpy
* Pandas
* Scipy
* Sklearn

# Requirements for visualization

* Matplotlib

# Contributor
* Makayla Frisse
