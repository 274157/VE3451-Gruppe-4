# VE3451-Gruppe-4
Classifying Electric Engine Conditions through Acoustic Analysis

## Setup
Download the dataset from https://zenodo.org/records/7551261

you need to change DATA path in notebook 01

you need the packages in requirements.txt

Currently we train the data on clips in train_cut only and all of test_cut are used for validation and testing.


## EDA

The code only looks at and plots either chosen clips or everything in the data set.

Test set stays unseen until final evaluation.

## How to run
1. First run 01_data_preparation in preprocessing once to save the training and validation data do data_cache/
2. run all or w/e you want to plot.
3. you can change clip where CLIP = x, or recording for validation plots where RECORDING = "talking_1" or "atmo_medium"


## Findings
- Heavy load has most of its energy at very low frequencies and is atleast 3 times louder than the others in the pure clips, but when background noise is added the difference is smaller.
- Broken has a noticable increase in audio between 4-6kHz
- Good has most of its energy low aswell but not as low as heavy load

