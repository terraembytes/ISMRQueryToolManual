# Plot

* * *

This function makes it possible to analyze time series of monitoring attributes, with the time attribute being represented along the x-axis.

* * *

After entering the initial parameters, the user can set some specific filters for plotting.

 - *The tool auto suggest labels and output parameters for plottings, but the user can change the filters manually. There are also some specific parameters for analysis.*

![Inputs](images/plot/inputs.PNG)

* * *

## **X-Axis/Label**
There are two options of time distribuition and the user can set labels for them.

 - **Continuous Time:** Data are arranged in a continuous time line according to the selected time interval

Example:

*Inputs:*

![TimeInterval](images/plot/examples/timeInterval.PNG)
![X-Axys](images/plot/examples/xAxis.PNG)

*Output:*

![Output](images/plot/examples/outputXaxys.PNG)

 - **Grouped by time of day [0h-24h]:** Data are arranged by the same time of days (from 0h00 to 23h59). This option allows the user to identify which hours of day are more affected by scintillation (time is given in GNSS time, not in local time).

Example:

*Inputs:*

![TimeInterval](images/plot/examples/timeInterval.PNG)
![X-Axys](images/plot/examples/xAxysDay.PNG)

*Output:*

![Output](images/plot/examples/outputxAxysDay.PNG)


* * *

## **Y-Axis and Labels**
The user can choose one or two parameters (from more than 60) to be plotted at some query, as well as styles for them. The most used and appropriate style is "points" (default), but "lines" and "linepoints" are also available.
