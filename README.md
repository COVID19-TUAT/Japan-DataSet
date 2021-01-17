# Japan-DataSet
This is the data repository for the COVID-19 in Japan. We try to unify the format of the COVID-19.  
We have already unified that in Japan! Now, we attempt to create unified data for each area narrower than prefecture (prefecture is like a U.S. state).  
  
Every data is stored by the same JSON format. Item "date", "data", "parent" and "child" have values in list.  
If data(positiveIncrease_release, positiveIncrease_onset, etc.) hasn't values, it has empty list.
- data
  - positiveRelease
    - date
    - data
  - positiveOnset
    - date
    - data
  - death
    - date
    - data
  - hospitalizedCurrently
    - date
    - data
  - inspection
    - date
    - data
  - consultations
    - date
    - data
  - population
- parent
- children
  
Description for each item　is shown below.
- positiveRelease: today's the number of new positive cases (**reported date base**)
- positiveOnset: today's the number of new positive cases (**onset date base**)
- death: today's the number of new death cases
- hospitalizedCurrently: currently hospitalization 
- inspection: today's the number of inspections
- consultations: today's the number of consultaions to Coronavirus Consultation Center
- population: population in the area  
              (if we can't get population, the value is null)
- parent: list of parent directory
- children: list of subdirectory

