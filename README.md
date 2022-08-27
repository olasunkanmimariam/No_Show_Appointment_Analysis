# Data Analysis Udacity Nanodegree

# No_Show_Appointment_Analysis: Investigate The Dataset

## Contents

Introduction

Data Wrangling

Exploratory Data Analysis

Conclusion

### Introduction

A patient makes a doctor's appointment, and didn't show up. Why?

The dataset collects information from 100k medical appointments in Brazil and is focused on the question of whether or not patients show up for their appointment. A number of characteristics about patient are included in the data

Original data can be access using this link https://www.google.com/url?q=https://www.kaggle.com/joniarroba/noshowappointments&sa=D&ust=1532469042118000

#### Data Dictionary
01 - PatientId: Identification of a patient

02 - AppointmentID: Identification of each appointment

03 - Gender: Male or Female

04 - AppointmentDay: The day of the actuall appointment, when they have to visit the doctor.

05 - ScheduledDay: The day someone called or registered the appointment, this is before appointment of course.

06 - Age: How old is the patient.

07 - Neighbourhood: Where the appointment takes place.

08 - Scholarship: 1 or 0 .This indicates whether or not the patient is enrolled in Brasillian Welfare program Bolsa Família.

09 - Hipertension: 1 or 0

10 - Diabetes: 1 or 0

11 - Alcoholism: 1 or 0

12 - Handcap: 1 or 0

13 - SMS_received: 1 or more messages sent to the patient.

14 - No-show: Yes or No.

##### Note: 'No' if the patient showed up to their appointment. and 'Yes' if they did not show up

#### Questions:

Analyzing this dataset aim to answer the following:

--How many percentage of patients miss their appointment

--What age category miss the appointment most and why?

--Is waiting days a factor for showing up for appointment?

--Does SMS received prompt patient to show for their appointment?

--Does patients enrollment in Brasillian Welfare program(i.e scholarship) affect their appointment

### Conclusion

Analyzing the dataset, I addressed a few issues like renaming columns to make them conform to standard, dropping the wrong data and unwanted columns. I also added new columns from existing ones.

Here are some insights uncovered:

--The scheduling of appointments began on 2015-11-10 and ended on 2016-06-08.

--Appointments for visits began on 2016-04-29 and ended on 2016-06-08.

--Children and youth account for the majority of people enrolled in Brasillan welfare programs (scholarships).

--On average, Old people have the highest hypertension and diabetes, while adults have the highest alcoholism.

--79.9% of patients show up to the doctor's appointment, while 20.1% did not

--Among the 20.1% who failed to attend, Child and Youth had the highest rate. This may be because hypertension, diabetes, and alcoholism are rare among them. WHILE

--Based on 79.9% of patients that showed up, Old, Adult always showed up the most because they often had hypertension, diabetes, and alcoholism

--In total, 37,072 patients scheduled appointments on the same day, 1726 did not show up, representing approximately 5% of the total.

--In general, the longer the waiting days, the greater the possibility of patients not showing up

--Out of 35,482 patients that received SMS, 25,698 showed up for the appointment. This implies that sending SMS to patients for reminders will prompt their show up

#### Limitations

The dataset contains incorrect data, such as patients under the age of 0 and those with negative waiting days values. This could be a result of data entry errors.
Further information, such as type of appointment (routine check-up, specialist visit, lab test), brief medical history, will benefit our analysis.

##### In conclusion:
A regular SMS should be sent to the patients regarding their appointment date.

A patient's appointment date should be scheduled within a short time period, as long waiting days would result in the patient not showing up later.

There should be more patients enrolled in the Brasillan welfare program.
