ABOUT THE SOFTWARE:
This is a 1D electrical resistivity inversion software. Its input is the apparent resistivity and acquisition’s parameters, and its output is the inverted model. This software uses a novel methods to transform data from apparent resistivity to true resistivity and invert for number of layers (selected automatically), 
true resistivity and thickness of each layer. The method follows the two-steps approach suggested by Simms and Morgan (1992) to systematically resolve the optimum number of layers. 
The first step is to run a fixed layer thickness inversion. 
Then, we use the outcome of the first inversion to determine the optimum number of layers as an input parameter for the second step, which is a variable-thickness inversion (layers’ thicknesses and resistivities are inversion parameters) for the final resistivity model. 
Both steps use rescaled Ridge Trace, damped least-square inversion. Unlike other software, it determines all inversion input parameters from the data file (maximum depth of interest, number of layers, initial resistivity,damping values, and number of iteration). 
The method utilizes an integrated program that performs the two inversion steps sequentially. The proposed method, which uses the robust ridge trace regression algorithm, has proven to be stable and accurate.


FEATURES:
The interface allow the user to load the data by browsing for the file from your personal computer. 
The user has the option to select between two different acquisition configurations (Schlumberger Array, or Wenner Array).
The interface has the feature to plot the uploaded apparent resistivity accordingly. It will plot the Wenner apparent resistivity after it converts it to Schlumberger apparent resistivity. 
The simple interface has a button “Run Inversion”, that will run the two steps of the inversion with detailed information about each iteration that includes RMSE, minimum/maximum damping value,data and inverted fit, and resistivity model. 
In between the two steps, it will show the user how it calculate the number of layers and give the option for the user to change that value using a bar or manually entering the value as positive integer. 
It will carry on to the next step of inversion in a similar way. As a last plot, it will show the final inverted model verses depth. 
Once the inversion is done, the user has the option of saving the data by clicking on “save”. The data can be saved in the following format:*.txt, *.mat, *.dat.

This GUI has been written so that it can easily be transported to any other machine supporting MATLAB GUIs.



INPUT DATA:
The input data can be in any of the following formats: *.txt, *.mat, *.dat.
For Schlumberger array:
Column (1) —- “L” half of potential electrode separation.
Column (2) —- “A” half of current electrode separation.
Column (3) —- Apparent resistivity in ohms.meter.
For Wenner array:
Column (1) —- “a” current/potential electrode separation in meter.
Column (2) —- Apparent resistivity in ohms.meter.




OUTPUT DATA:
The output data can be saving in one the following formats: *.txt, *.mat, *.dat.
Structure:
Column (1) —- Depth in meter.
Column (2) —- Inverted resistivity in ohms.meter.



AUTHORS:
Ammar Alali 
Earth Resources Laboratory, Massachusetts Institute of Technology.
ammarali@mit.edu
ammar.m.alali@gmail.com

Professor Frank Dale Morgan
Earth Resources Laboratory, Massachusetts Institute of Technology.  
fdmorgan@mit.edu

Darrell Coles
Earth Resources Laboratory, Massachusetts Institute of Technology.
