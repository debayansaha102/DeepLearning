ReadMe
BeadDetectionAndAnalysis is a module that allows you to find the centroid of beads from a deficused 3D stack, extract 1D signals within a range around the centroid, and then fit a gaussian curve to this signal to extract properties of the bead. Depending on the fit quality some of the beads are termed as nto a bead and hencefoth dropped from analysis. The module is under development in Myers lab.

Usage:
This is a standalone script on jupyter notebook where the imports are standard modules found on pip install
Go on compiling every cell under the heading "Defining Functions" until you reach "Processing Images"
Change the parameters on the "Input cells" and verify the suitability in the "Output Cells". If you are happy with the output cell make changes in the following "Input Cell" and go on therafter.
Once you are happy with all the outputs and parameter settings, change the mode operation and execute all the cells

Output:
In the folder given as input, a sub folder with name Analysis will be created
Tha Analysis folder will contain ZParam%n.csv,YParam%n.csv, XParam%n.csv where %n is the image number(timepoints).
Each of these .csv files represent the parameters for curve fitting of the Z,Y,X signal respectively. Each row of this .csv file represeents each bead. The coulmns represent amplitude of the gaussian,  center of the gaussian, width of the gaussian, ydisplacement of the gaussian(background) respectively.