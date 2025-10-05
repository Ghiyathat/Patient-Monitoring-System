## Patient Monitoring System with Numpy
This project implements a simple patient monitoring system using Numpy. Synthetic data was generated for 4 patients over 3 days, with measurements taken twice daily (morning and evening). 

The project demonstrates how Numpy arrays can be used to structure, manipulate, and analyze multidimensional healthcare datafor isights that support public health decision making.

### Data Structure

Each Patient record contains:
1. Heart Rate (bpm)
2. Systolic Blood Pressure (mmHg)
3. Diastolic Blood Pressure
4. Temperature (⁰C)

The dataset was stored as a numpy array with shape (4, 3, 2, 4), structured as follows:
- Axis 0 -- Patients (4)
- Axis 1 -- Days (3)
- Axis 2 -- Time of Day (0: Morning, 1: Evening)
- Axis 3 -- Vital signs (HR, SBP, DBP, Temp)

What I did:
1. Synthetic Data Generation
   - Created a `(4, 3, 2, 4)` Numpy array to represent patient data
   - Generated random values within medical ranges:
     - Heart Rate: 60 - 100 bpm
     - Systolic BP: 90 -120 mmHg
     - Diastolic BP: 60 - 80 mmHg
     - Temperature: 36 - 39 ⁰C

### Data Analysis
- Extracted patient - and day-specific vital signs
- Isolated key metrics (e.g., all temperatures or evening HR for a patient)
- Detected abnormal readings (fever > 37.5⁰C)
- Checked for critical events (SBP > 140 mmHg)
- Computed:
   - Average HR per patient
   - Mean SBP across hospital
   - Max temperature per day
- Sorted patients by average heart rate
- Created new focused arays (e.g., HR and Temp only)

### Key skills demonstrated
- Numpy multidimensional array creation and manipulation
- Conditional filtering and and statistical computation
- Healthcare data simulation and anomaly detection
- Structured data analysis for public health insights

### Tools Used
- Python
- Numpy

Reference


