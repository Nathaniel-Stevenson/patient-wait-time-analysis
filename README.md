# Patient Wait Time Analysis

## Overview
This analysis uses a publicly available simulated dataset of patient flow and wait times across multiple hospitals. The goal is to identify how patient load per nurse interacts with wait times.
Data source: https://www.kaggle.com/datasets/maalona/hospital-triage-and-patient-history-data

## Metric
Patients to nurse ratio = number of patients divided by number of nurses

## Key Findings
Patients to nurse ratio is a key determiner in the total time a patient will spend at a facility. 

While more patients to nurse always increases wait time, the average time difference between 1 patient to nurse and 2 patients to nurse only reduces wait time by 4 minutes. This represents twice the patient load per nurse with little benefit to total wait time. This is consistent with available capacity at these levels.

Wait time seriously begins to change from 2 patients to nurse -> 3 patients to nurse, increasing wait times by 40 minutes on average. Wait times remain stable before 2 patients to nurse, but increase sharply after that point. Current breakdown is insufficient to find optimal staffing ratio.

Wait times can be controlled by
- Accurate prediction of patient numbers with predictive staffing
- Increasing the number of nurses ad hoc during rushes

## Further analysis recommended 
- Further breakdown to attempt to determine optimal staffing ratio
- Effect of time of day on patients to nurse ratio
- Specialist available effect on total wait time
- Patients to nurse ratio effect on time to medical

## Limitations
- Uses averaged buckets
- Does not capture distribution-level effects
