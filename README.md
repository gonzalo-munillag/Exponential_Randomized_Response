# Exponential Randomised Response 
## Combining the Exponential Mechanism and Randomized Response to Increase Utility in Differentially Private Selection

This repository contains the code to reproduce the publication "---".

## Contents

[Experiments](https://github.com/gonzalo-munillag/Exponential_Randomised_Response/tree/main/Experiments): Folder containing all the empirical comparisons between mechanisms.  
[differential-privacy-library-main](https://github.com/gonzalo-munillag/Exponential_Randomised_Response/tree/main/differential-privacy-library-main): Folder containing the diffprivlib library from IBM ([Original here](https://github.com/IBM/differential-privacy-library)) with the addition of the Exponential Randomised Response mechanism. 

The code of the Exponential Randomised Response mechanism can be specifically found [here](https://github.com/gonzalo-munillag/Exponential_Randomised_Response/blob/0155ffea84110c2c02841f070bdb5379381b2cb7/differential-privacy-library-main/diffprivlib/mechanisms/exponential.py#L194)

## Setup

1) In the terminal, go to the differential-privacy-library-main folder and install my modified version of diffprivlib (the modification is the addition of the novel mechanism that I present in the aforementioned paper):

$ pip install .

2) In a .py executable or Jupyter Notebook cell import the exponential mechanism functionality

from diffprivlib.mechanisms import exponential

3) To use the novel method, call:

 exponential.EnhancedRandomizedResponse(...)
