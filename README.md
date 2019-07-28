# OPAF - Order Parameter Automatic Filtration
An algorithm that reduces a large dictionary of order parameters to a smaller set of order parameters by screening for redundancy using a mutual information based distance metric.

Overviews of each of the subdirectories in this repository are provided below. For detailed descriptions of the files within the subdirectories, refer to the README's in each subdirectory.

## ModelSystems

This directory contains two analytical model systems that were used for initial testing of OPAF. The code for the algorithm is the same as for experimental systems, but the input order parameters used are generated internally, rather than from a COLVAR as it would in a real system. It is provided to help users gain an intuition for how the algorithm works.

## BUT

Of the provided applications, this is the most similar to a practical use of OPAF. Input data is from a short unbiased MD simulation of the FKBP/BUT protein-ligand system. In practice, applications of OPAF should resemble the code provided in this directory. It is important to note that since this is a realistic application, a single run can take around 20-30 minutes, depending on your system.

## src

This is the final, ready-to-use version of OPAF that takes as input a COLVAR corresponding to some set of order parameters and outputs a "reduced" COLVAR that only contains the order parameters selected by OPAF.
