---
layout: post
title:  "Elemental Abundance"
date: 2024-7-14
image: assets/images/periodic.png
tags: [planet, tutorials, resources, summer2024 ]
---


&nbsp;    
<img width=900 src="/assets/images/periodic.png" class="img-fluid" />
&nbsp;

*Credit: Wikipedia. https://en.wikipedia.org/wiki/Periodic_table#/media/File:Colour_18-col_PT_with_labels.png*   

<br/>

**CONCEPTS & TERMS**   

**concentration**   
Concentration is a measure of the relative amount of dissolved substances in a solution. Concentration can be expressed in many different ways.

**parts per million (ppm)**   
The number of grams of an element dissolved in 1,000,000 g of water.

**parts per billion (ppb)**   
The number of grams of an element dissolved in 1,000,000,000 g of water.   

**trace element**   
Elements with concentrations measured in ppm or ppb are called trace elements. For example, if 40g of a trace elememt are found in 1,000,000 g of water, the trace element's concentration is 40 ppm.    

**parts per thousand (ppt)**   
Concentration can be expressed in terms of the number of grams of an element dissolved in 1,000 g of water. The unit for this measure is parts per thousand, or ppt. For example, salinity is hte measure of the number of grams of salts per kilogram (kg) of water. The average salinity of seawater is about 35 g/kg of seawater, or 35 ppt.   

**periodic table**   
The periodic table arranges all the known elements in an array. Elments are arranged left to right and top to bottom in order of increasing atomic number, which coincides with increasing atomic mass. The rows of elements are periods. The period number of an element signifies the highest energy level an electron in that element occupies.   

**counts per second (cps)**   
Counts per second, abbreviated to *cps*. Sensitivity is expressed as counts per second per unit concentration (e.g. cps/ppb). Without sufficient sensitivity, small particles cannot be detected. 

**analyte**   
Analyte refers to the component of a sample that is ultimately determined directly or indirectly.   

**matrix**   
Matrix refers to the components of a sample other than the analyte of interest.   
The matrix can have a considerable effect on the way the analysis is conducted and the quality of the results are obtained; Such effects are called matrix effects.   

**standard solution**   
A standard solution is a solution containing an accurately known concentration.  
Standards are prepared in volumetric flasks.   
The mass concentration μg ml<sup>-1</sup> (it could also be expresses as mg l<sup>-1</sup>) is also referred to as ppm (parts per million).   

**commonly used prefixes (multiple-prefix-symbol)**   
10<sup>3</sup>: kilo, K   
10<sup>6</sup>: mega, M   
10<sup>9</sup>: giga, G   
10<sup>12</sup>: tera, T   
10<sup>15</sup>: peta, P   
10<sup>-3</sup>: milli, m   
10<sup>-6</sup>: micro, μ   
10<sup>-9</sup>: nano, n   
10<sup>-12</sup>: pico, p   
10<sup>-15</sup>: femto, f   

**limit of detection (LOD)**   
The limit of detection (LOD) of an analytical procedure is the lowest amount of analyte in an unknown sample that can be detected but not necessarily quantified, that is, recorded as an exact concentration.

**accuracy**   
Accuracy refers to the difference beetween the mean of a set of results or an individual result and the value that is accepted as the true or correct value for the quantity being measured.   

**precision**   
Precision refers to the closeness of agreement between independent test results obtained under stipulated conditions.   

**bias**   
Bias characterizes the systematic error in each analytical procedure and is the deviation of the mean analytical result from the true value.   

**calibration**   
Calibration refers to the set of operations that establish, under specified conditions, the relationship between values indicated by a measuring instrument or measuring system and the corresponding known values of the measurand.   

**calibration curve**   
Calibration curve refers to graphical representation of a measuring signal as a function of quantity of analyte.

<br/>

**DATA ANALYSIS**   

**Excel**   
- **<em>Hide rows or columns</em>**: right-click the selected rows or columns and then select Hide   
- **<em>Unhide</em>**: Format -> Column -> Unhide   
- **<em>Dollar sign</em>**: Add dollar sign for absolute reference before the row and the column, e.g., $AG142, G$48   
- **<em>Freeze first two columns</em>**: Select the third column and select View -> Freeze Panes   



**graph**   
You can plot a graph with Excel, or Python, or by hand (I recommend you always try to plot a graph by hand first if you are a new learner- you need the skill to plot a graph). Graphs are used to describe a relationship between two variables, x and y. It is normal practice to identify the x-axis as the horizontal axis for the independent variable, e.g., concentration in μg ml<sup>-1</sup>. The y-axis is used to plot the dependent variable, y, e.g., signal response in mV. The mathematical relationship for straight line graphs is: y = mx + b, where y is the signal response in mV, x is the concentration in μg ml<sup>-1</sup>, m is the slope of the line of best fit of the graph, and c is the intercept on the x-axis.     


**Linest function in Excel**   
The linest function in Excel is a tool to fit a line (y=mx+b) to the data in order to identify the relationship between two variables (x and y). The linest function uses the least square procedure which fits a line to a set of data points by minizing the sum of the squares of the residuals of the points from the curve. 

You need two columns of data, one for variable x and one for y.   
x &nbsp; &nbsp; &nbsp; &nbsp;y   
1 &nbsp; &nbsp; &nbsp; &nbsp;1   
9 &nbsp; &nbsp; &nbsp; 1.35   
16&nbsp; &nbsp; &nbsp;1.36   
24&nbsp; &nbsp; &nbsp;1.24   
31&nbsp; &nbsp; &nbsp;1.21   
38&nbsp; &nbsp; &nbsp;1.16   


<br/>

**LEARNING MATERIALS**   
- [Periodic Table of the Elements](https://depts.washington.edu/eooptic/linkfiles/The%20Elements.pdf){:target="_blank"}   
- [Periodic Tables of Elemental Abundances](https://drive.google.com/file/d/12kSfP_ekUiRW2ONNmmFnXPRgQK-UIrOt/view?usp=sharing){:target="_blank"}   
- [Abundance of 30 Elements in Lunar Rocks](https://drive.google.com/file/d/1BawQqY8FTfDbtCSoUMKgWvmTTi-GWZJT/view?usp=sharing){:target="_blank"}
- [Environmental Sampling and Analytical Methods (ESAM) by EPA](https://www.epa.gov/esam){:target="_blank"}   
- [EPA Method 200.8](https://www.epa.gov/sites/default/files/2015-06/documents/epa-200.8.pdf){:target="_blank"}   
- [Analyzing Trace Elements with EPA Method 200.8](https://www.thermofisher.com/us/en/home/industrial/environmental/environmental-learning-center/environmental-resource-library/us-epa-methods/analyzing-trace-elements-epa-method-200-8.html){:target="_blank"}



