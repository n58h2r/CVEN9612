java cCVEN9612 – Catchment Modelling 
Assignment 1 Part 1– Rainfall-Runoff Modeling and Routing 
This part of the assignment is worth 15% of the total grade for CVEN9612. The assignment 
answers are to be submitted online in Moodle as a short report. 
 
Assignment 1 Part 1 is due 10pm 30th September (Week 4) 
 
Total marks available for each part are listed below. 
 
Question 1 – Runoff routing (15 marks) 
There was a large flood on the Richmond and Wilsons Rivers in February 2024, which led to 
extensive damage in Lismore and surrounding areas. The flood hydrograph on the Richmond 
River was measured at Wiangaree (EL. 91m AHD) and we would like to be able to model the 
hydrograph at the town of Kyogle, 21km further downstream (EL 71m AHD). The observed 
streamflow hydrographs at Wiangaree and Kyogle are available on Moodle. 
 
Using Manning’s Equation calculate a representative wave velocity for flow down the channel 
assuming that the hydraulic radius of the channel is R=5.2 and it has a Manning roughness n of 
0.05. Assume the wave celerity is 1.7 times the Mannings velocity. 
 
Employ the Muskingum method to determine the best estimate of the flood hydrograph at Kyogle, 
assuming that an approximate value of K can be calculated by dividing the reach length by the 
wave speed. Calibrate your model to estimate the best value for x by minimizing the sum of 
squared error of the prediction. 
 
Provide a short report (less than 2 pages), with appropriate figures to answer the following 
questions. Show your working where appropriate and justify any assumptions that are required. 
 
a) What time step did you use for your calculations (in hours) and how do you know if it is 
appropriate? (1 mark) 
 
b) What is the peak of the calculated flow hydrograph at Kyogle? (5 marks) 
 
c) What value of x did you use and how did you know this was the optimum value? 
Demonstrate with the use of an appropriate figure. (3 marks) 
 
d) What is the RMSE of the calculated outflow hydrograph compared to the observed data at 
Kyogle? (2 marks) 
 
e) What is the impact of changing the value of x to 0? What is the practical meaning of x = 
0? (2 marks) 
 
f) If there was interest in investigating Nature Based Solutions in the Richmond catchment 
and riparian zone was revegetated and as a result Mannings n was 0.1, what is the new 
peak flow at Kyogle? Explain how revegetation affects the routing of flows. (3 marks) 2 
 
Question 2 – Model Calibration (15 marks) 
Model aim 
In this part of the assignment, you need to model the runoff and Lake Werri Berri in the Thirlmere 
Lakes National Park wetland system using GR4J. The model is to be set up to understand 
1. how often the lake is suitable for water sports and 
2. the risk of bushfires affecting the sensitive peat ecosystem of the lake. 
 
Water sports can only occur when the lake is more than 2 m deep and bushfire risk is too high if 
water levels in lakes are less than 0.1 m for more than 30 consecutive days. The management plan 
for the lakes requires decisions to be supported with 8 years of data hence why a model is required 
as flow data is only available since 2011. The management plan requires the frequency of these 
two events (i.e. water sports and bushfire risk) to be documented. 
 
The aim of the modelling exercise is twofold: 
 
 (i) to understand the implications of choices in modelling such as objective function and 
data transformation on lake water level predictions and what the most appropriate 
choices are given the aims of the model. 
(ii) To assess an alternative GR4J model for the same catchment which uses satellite 
retrieved surro代 写CVEN9612、Java/Python
代做程序编程语言gates using the SRM methodology of Yoon et al., 2023 (week 3 lecture). 
 
Assignment details 
Use the AirGR and SRM packages in R to model the catchment. Instructions for AirGR and a 
short video on setting up a model in AirGR are provided on Moodle. Please be aware that in the 
Surrogate River discharge Model (SRM), only one objective function is available, which is 
focused on minimizing the Surrogate River discharge Model Error (SRME). 
 
Data, code, and the SRM Package can be downloaded via this link: https://deciduous-camp995.notion.site/Sharing-SRM-for-CVEN9612-e7a48b40de9b4f38a16915d1c6a07a4d

Rainfall, evaporation and streamflow data is provided for the catchment on Moodle. Data in all 
files is provided in mm/day. The catchment area is 84 ha. 
 
You can assume that the wetlands have a plan area of 10.5 ha and that water levels can range 
between 0 m and 5 m. Assume that the catchment average rainfall and evaporation also apply 
directly to the wetland water balance. Assume that there are no groundwater interactions and that 
if water levels are higher than 5 m that all flow is lost instantaneously on that day. 
 
You will have to select an appropriate calibration period given the data available for the catchment. 
It is up to you to decide on how best to use the data that is available in setting up the model. You 
will also have to decide what objective function and data transformation is the most appropriate 
given the model aims. 
 
In your short report (less than 3 pages), you need to assess at least two objective functions and two 
data transformations and comment on the sensitivity of your conclusions to the modelling choices 
you made when calibrating using observed flow data. You also need to compare the SRM 
calibration with that for the model version where observed flows are used for calibration, noting 
key similarities and differences. Provide suitable figures and tables of results to support your 
conclusions. 3 
 
Part 2 marking rubric 
 
 1 mark 2 marks 3 marks 4 marks 
Description of 
model set up 
No details 
provided and 
unclear if 
correct set up 
used 
Some details 
provided or 
obvious 
problems with 
simulations 
 Clear description of 
set up, parameter 
values and model 
results 
Clear and 
detailed 
description of 
set up, 
modelling 
choices and 
summaries of 
results 
Modelling 2 
data 
transformatio
n, 2 objective 
functions, 
comparison 
with SRM 
Only one set of 
model 
simulations 
provided 
Either two 
transformations 
or 2 objective 
functions not 
tested 
4 combinations of 
model set up with 
discussion of 
differences/similariti
es and best choice 
 As before, plus 
an assessment 
of similarity and 
differences in 
model with 
respect to the 
SRM version 
Conclusions 
on risk of not 
meeting flow 
requirements 
Incorrect 
recommendatio
n, no discussion 
on model 
limitations 
Either incorrect 
recommendatio
n or no 
discussion on 
model 
limitations 
Clear and correct 
recommendation. 
Only limited 
discussion of model 
limitations 
Clear and 
correct 
recommendatio
n. Thorough 
discussion of 
model 
limitations and 
their 
implications for 
recommendatio
n. 
Reporting 
quality 
Poor quality 
figures/tables, 
poorly 
structured, hard 
to understand 
 Acceptable 
presentation 
quality, with 
potential for 
improvements. 
Well structured, 
tables and figures 
labelled, 
grammatically 
correct 
 
         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
