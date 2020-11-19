# Change-Point-Detection-Model
Change Point Detection on Wind Turbine Gearbox Sensors
# Objective
The objective of the project is to build a Change Point Detection model to detect change points in variance on wind turbine gearboxes.
# Method
The notebook incorporates rpy2 to import R libraries to perform the change point detection analysis.  The "Mood" algrithm is used on the dataset of a wind turbine to detect changes in variance.  Two aggregations are added to evaluate possible clearer change points.  To adjust for autocorrelation, the log differences are applied to the data before application of the change point detection.  Then to visualize real changes, Exponential Weighted Moving Averages of the squared log differences is plotted on the change points.  
# Results
Plotting the change points on the EWMA of the squared residuals showed a successful model with the least Average Detection Delay on the unaggregated data.  There was little benefit to aggregating the data as it increased the average detection delay with little benefit of clearer results.  
