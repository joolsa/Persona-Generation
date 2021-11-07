# Big Data, Small Personas: How Algorithms Affect the Demographics of Data-Driven User Segments

This repository contains the materials for the "Big Data, Small Personas" research paper.


>**Big Data, Small Personas: How Algorithms Affect the Demographics of Data-Driven User Segments**
>*Salminen, J., Chhirang, K., Jung, S.-G., Thirumuruganathan, S., Guan, K.W., & Jansen, B. J. (2021).Big Data, Small Personas: How Algorithms Affect the Demographics of Data-Driven User Segments.*

>Link to paper: [TBA]

# Dataset
Data.csv contains data to run the persona generation algorithms. NOTE: The data file is scrambled to protect business-sensitive information, and thus provide an example of data structure and dimensionality rather than real data. To generate meaningful personas, the data files should be replaced with real user data obtained from YouTube Analytics or other compatible source. NOTE: Due to GitHub's file size restrictions, the example dataset (48MB) is provided via Dropbox: https://www.dropbox.com/s/oifkk6fmzb332so/Data.csv?dl=0

# Persona decomposition
This notebook illustrates the segmentation procedures undertaken using the tested algorithms.

# Persona evaluation
This notebook illustrates the evaluation of the generated personas using the metrics defined in the paper (diversity, fairness, consistency).

=======INSTRUCTIONS=======

You can install the libraries required to run the code by using this command:

    pip install -r requirements.txt

The replication of the methodology involves four steps. The steps are explained as follows.

STEP 1: Download the example dataset: https://www.dropbox.com/s/oifkk6fmzb332so/Data.csv?dl=0
STEP 2: Decompose the personas:

(a) Persona decomposition.ipynb -- this file contains the necessary code for decomposing the example dataset.
(b) Decomposition results in two files that are required for persona generation (normal and transposed file).

STEP 3: Submit your decomposed files (normal and transposed) to Automatic Persona Generation: https://persona.qcri.org (contact the authors if you need assistance).

STEP 4: You will receive back files corresponding to contents of the "personas" folder (i.e., these are the personas we generated from our dataset).
You can then evaluate the personas in these files using the following notebook:

(c) Persona evaluation.ipynb -- this file contains the necessary code for evaluating Persona Diversity, Fairness, and Consistency (DFC).

=======REQUIREMENTS=======

scikit-learn==0.23.dev0
numpy==1.18.4
umap-learn[plot]==0.4.1
pandas==0.25.3
matplotlib==3.1.3
seaborn==0.10.0

