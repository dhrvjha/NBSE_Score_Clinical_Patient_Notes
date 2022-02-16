# NBSE - Score Clinical Patient Notes

# Introduction

NBSE → National Board of Medical Examiners

NBSE conducts exam for physicians, scoring them on basis of “patient notes” which is a note that a physicians are required to make after analyzing patient’s symptoms.

The accuracy of these notes can have direct effect on a patient.

# Task

map “clinical concept”  features provided to the patient’s note annotation.

# Provided Information for solving the task

### train.csv

1. id = pair of patient note and feature, (pn_num_feature_num)
2. case_num = case to which patient note belongs
3. pn_num = patient note annotated in this row.
4. feature_num = the feature annotated in this row.
5. annotation = text within a patient note indicating a feature
6. location = character span indicating location of each annotation within the note.

### features.csv

1. feature_num = unique id for feature
2. case_num = case in which patient belongs.
3. feature_text = description of the feature.

### patient_notes.csv

1. pn_num = unique id for patient note
2. case_num = reference to clinical case a patient note represents
3. pn_history = text of encounter by test taker.

### 

# Challenges

The biggest challenge is a feature can be expressed in many ways example-

Feature → “loss of interest in activities”

expressed → “no longer plays tennis”