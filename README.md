# ssTEM-Image-Analysis
This code performs a semi-automated image analysis procedure to identify microtubules in serial section transmission electron micrographs (ssTEM) of a C. elegans PLM neuron.

Note, this code is based on Python 3.7 

Scientific paper using this code: doi: 10.1016/j.bpj.2022.11.2946.

<b> Files: </b> <br>
1. Automated_Analysis: Performs automated template matching to identify microtubules in the full image set. <br>
2. Manual_Edits: Allows the user to make edits to the automated results by clicking missed microtubules and drawing boxes around false positives. <br>
3. Registration: Registers microtubule match locations in adjacent images to trace microtubules throughout the full image stack. <br>
4. RealisticGeometry_ABAQUSInput: Adds randomly dispersed crosslinks to the ssTEM-based microtubule geometry and converts the results into an ABAQUS mesh. Generates an ABAQUS input file. <br> 
5. IdealizedGeometry_ABAQUSInput: Generates an idealized geometry of regularly spaced, equally-sized microtubules with randomly dispersed crosslinks. Generates an ABAQUS input file. <br>

<b> Dependencies: </b> <br>

OpenCV v3.4.2: https://github.com/opencv/opencv <br> 
NumPy v1.18.1 <br> 
pandas v1.0.3 <br>
SciPy v1.4.1 <br>
scikit-learn v0.22.1 <br>
openpyxl v3.0.6 <br>
pycpd: https://github.com/siavashk/pycpd
