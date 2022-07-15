#Exploratory Data Analysis of Diabetes Hospital Readmission in the United States through Decision Tree
What factors collected from the United States' Hosiptals will help predict diabetes readmission.

* With our selected features, the decision tree we have composed will predict the diabetes early readmission rate in the United States. Defined as within a month

#Dataset
* Center for Clinical and Translational Research, Virginia Commonwealth University https://archive.ics.uci.edu/ml/datasets/Diabetes+130-US+hospitals+for+years+1999-2008

* Discovered through https://www.kaggle.com/brandao/diabetes?select=diabetic_data.csv

* 1)	It is an inpatient encounter (a hospital admission).
* (2)	It is a “diabetic” encounter, that is, one during which any kind of diabetes was entered to the system as a diagnosis.
* (3)	The length of stay was at least 1 day and at most 14 days.
* (4)	Laboratory tests were performed during the encounter.
* (5)	Medications were administered during the encounter.

Data Was taken from 130 hospitals
* 18 Midwest
* 58 Northeast 
* 28 South
* 16 West

Note that a portion of hospitals were labeled as having a bed size of less than 100. And 14 hospitals had a bedsize > 500



## Details
The Data consists of around 101,766 rows - one row per encounter ID - and 50 columns.

#### encounter_ID
* An unique identification number at the time a patient's appointment is scheduled.

#### patient_nbr
* An unique number of a patient

#### race
* Patient's race is Caucasian, Asian, African American, Hispanic, and other

#### gender
* Patient's gender male, female, and unknown/invalid

#### age
* Patient' age grouped in 10-year intervals: 0, 10), 10, 20), …, 90, 100)

#### weight
* Weight of patient (lBs).

#### admission_type_id
* An ID corresponding with 4 distint cirumstance a patient was admitted.

#### discharge_disposition_id
* A two-digit ID that corresponds with 28 distint values of a patient's discharge status.

### admission_source_id
* The code indicating the source of the referral for the admission or visit.
* https://resdac.org/cms-data/variables/claim-source-inpatient-admission-code-ffs

### time_in_hospital
* Number of days patient spend in the hospital between admission and discharge

### payer_code
* A code that is assiged to an insurance company for the purpose of transmitting your claims electronically.

### medical_specialty
* Specialize medical practice 

### num_lab_procedures
* Number of lab procedures

### num_procedures
* Number of procedures

### num_medications
* Number of medications.

### number_outpatient
* Number of outpatients

### number_emergency
* Number of emergencies 

### number_inpatient
* Number of inpatients

### diag_1
* The primary diagnosis (coded as first three digits of ICD9); 848 distinct values

### diag_2
* Secondary diagnosis (coded as first three digits of ICD9); 923 distinct values

### diag_3
* Additional secondary diagnosis (coded as first three digits of ICD9); 954 distinct values

### number_diagnoses
* Number of diagnoses

### max_glu_serum
* Indicates the range of the result or if the test was not taken. Values: “>200,” “>300,” “normal,” and “none” if not measured

### A1Credult
* Indicates the range of the result or if the test was not taken. Values: “>8” if the result was greater than 8%, “>7” if the result was greater than 7% but less than 8%, “normal” if the result was less than 7%, and “none” if not measured.
* This is a very important measure of glucose control - and used to help measure the preformance of diabetes control.  

### Medications
* 23 features for medications For the generic names: metformin, repaglinide, nateglinide, chlorpropamide, glimepiride, acetohexamide, glipizide, glyburide, tolbutamide, pioglitazone, rosiglitazone, acarbose, miglitol, troglitazone, tolazamide, examide, sitagliptin, insulin, glyburide-metformin, glipizide-metformin, glimepiride- pioglitazone, metformin-rosiglitazone, and metformin- pioglitazone

### change  
* Indicates if there was a change in diabetic medications (either dosage or generic name). Values: “change” and “no change”

### diabetesMed
* Indicates if there was any diabetic medication prescribed. Values: “yes” and “no”

### readmitted
* No readmission
* A readmission in less than 30 days (this situation is not good, because maybe your treatment was not appropriate)
* A readmission in more than 30 days (this one is not so good as well the last one, however, the reason can be the state of the patient