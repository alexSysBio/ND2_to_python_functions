This repository includes useful functions for the analysis of microscopy images:

nd2_to_array:
  The nd2_to_array function can be used to import .nd2 files into python. The files are stored into a dictionary which includes elemenets of the iteration axis as   keys and the image 2D numpy arrays as values. It uses the nd2 image reader from the pims library:
  https://pypi.org/project/pims-nd2/#:~:text=pims_nd2%20contains%20a%20reader%20for,and%20nice%20display%20in%20IPython.
  
  I have tested most of the implemented iterations from microscopy images I have acquired. If the remaining iterations do not work it should be an easy fix. Please reach out if any exceptions pop up.

  Cite:
    https://www.biorxiv.org/content/10.1101/2024.10.08.617237v2.full
    
    DNA/polysome phase separation and cell width confinement couple nucleoid segregation 
    to cell growth in Escherichia coli
    
    Alexandros Papagiannakis, Qiwei Yu, Sander K. Govers, Wei-Hsiang Lin,  Ned S. Wingreen, Christine Jacobs-Wagner
    
    bioRxiv, https://doi.org/10.1101/2024.10.08.617237, October 22, 2024

Biviriate_medial_axis_estimation:
  The function get_medial_axis draws the central line of elongated (rod-shaped) cells from pole to pole. A set to test the medial axis estimation is also provided along with a notebook that demonstrates how the function works. The get_oned_coordinates function projects all the cell pixels onto the central line,
  in relative or absolute arch-length coordinates from pole to pole. The distance from the central line is multiplied by the sign of the cross product to get the 
  orientation of the cell pixels around the medial axis (above or below).

  Cite:
    https://www.biorxiv.org/content/10.1101/2024.10.08.617237v2.full
    
    DNA/polysome phase separation and cell width confinement couple nucleoid segregation 
    to cell growth in Escherichia coli
    
    Alexandros Papagiannakis, Qiwei Yu, Sander K. Govers, Wei-Hsiang Lin,  Ned S. Wingreen, Christine Jacobs-Wagner
    
    bioRxiv, https://doi.org/10.1101/2024.10.08.617237, October 22, 2024

