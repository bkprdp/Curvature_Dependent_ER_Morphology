# Curvature_Dependent_ER_Morphology
This repository contains the necessary files to reproduce the results presented in the article, which is under review -"Curvature-dependent morphological reorganization of the endoplasmic reticulum determines the mode of epithelial migration"
by Simran Rawal, Pradeep Keshavanarayana, Diya Manoj, Purnati Khuntia, Sanak Banerjee, Basil Thurakkal, Rituraj Marwaha, Fabian Spill, and Tamal Das.

The code is distributed as open access. 
Please contact f.spill@bham.ac.uk or p.keshavanarayana@ucl.ac.uk with any questions about the files present in this repo. 

Abaqus inp files are the input files that contain details about geometry and mesh.
Abaqus UMAT files contain the implementation of material definition for active actin cortex described in the article. 
To run, enter the following command on the terminal or command prompt : 
abaqus job=output_file_name input=name_of_input_file user=umat_file_name
where output_file_name is the user's choice of output file name, name_of_input_file is the input file that has .inp format, and umat_file_name is the UMAT file having .f format. 
The results will be stored in ODB format, which can be opened in ABAQUS CAE. 
To get the strain energy, plot strain energy of whole model, which is stored in the history outputs.

PS: To speed up the computations, you can use UMAT_xxx_Simplified.f instead of UMAT_xxx.f. This implementation has a simplified version of numerical integration.
