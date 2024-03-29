# Big Data, Small Personas: How Algorithms Affect the Demographics of Data-Driven User Segments

## Introduction

This repository contains the materials for the "Big Data, Small Personas" research paper.


>**Big Data, Small Personas: How Algorithms Affect the Demographics of Data-Driven User Segments**
>*Salminen, J., Chhirang, K., Jung, S.-G., Thirumuruganathan, S., Guan, K.W., & Jansen, B. J. (2021).Big Data, Small Personas: How Algorithms Affect the Demographics of Data-Driven User Segments.*

>Link to paper: [TBA]

## What's Needed?

### 1. Dataset
Download the example dataset from Dropbox. This dataset (Data.csv) contains data to run the persona generation algorithms. NOTE: The data file is scrambled to protect business-sensitive information, and thus provide an example of data structure and dimensionality rather than real data. To generate meaningful personas, the data files should be replaced with real user data obtained from YouTube Analytics or other compatible source. NOTE: Due to GitHub's file size restrictions, the example dataset (48MB) is provided via Dropbox: https://www.dropbox.com/s/oifkk6fmzb332so/Data.csv?dl=0

### 2. Persona decomposition (Python notebook)
This notebook illustrates the segmentation procedures undertaken using the tested algorithms.

### 3. Persona evaluation (Python notebook)
This notebook illustrates the evaluation of the generated personas using the metrics defined in the paper (diversity, fairness, consistency).

More detailed instructions are presented below.

## Instructions

STEP 1: Install the libraries required to run the code by using this command:

    pip install -r requirements.txt

The replication of the methodology involves four steps. The steps are explained as follows.

STEP 2: Download the example dataset: https://www.dropbox.com/s/oifkk6fmzb332so/Data.csv?dl=0

STEP 3: Decompose the personas:

>Persona decomposition.ipynb -- this file contains the necessary code for decomposing the example dataset.

The decomposition outputs two files that are required for persona generation (normal and transposed file).

STEP 4: Submit your decomposed files (normal and transposed) to Automatic Persona Generation: https://persona.qcri.org (contact the authors if you need assistance).

STEP 5: You will receive back files corresponding to contents of the "personas" folder (i.e., these are the personas we generated from our dataset).
You can then evaluate the personas in these files using the following notebook:

> Persona evaluation.ipynb -- this file contains the necessary code for evaluating Persona Diversity, Fairness, and Consistency (DFC).

