# Exponential Randomised Response 
## Combining the Exponential Mechanism and Randomized Response to Increase Utility in Differentially Private Selection

This repository contains the code to reproduce the publication "---".

## Contents

Experiments: Folder containing all the empirical comparisons between mechanisms.  
differential-privacy-library-main: Folder containing the diffprivlib library with the addition of Exponential Randomised Response

## Setup

1) In the terminal, go to the differential-privacy-library-main folder and install my modified version of diffprivlib (the modification is the addition of the novel mechanism that I present in the aforementioned paper):

$ pip install .

2) In a .py executable or Jupyter Notebook cell import the exponential mechanism functionality

from diffprivlib.mechanisms import exponential

3) To use the novel method, call:

 exponential.EnhancedRandomizedResponse(...)
