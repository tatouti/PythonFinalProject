# PythonProject

## Alexandre BARRAT & Théo JAOUDET

### Diabetes 130-US hospitals for years 1999-2008

#### Data description : The dataset represents 10 years (1999-2008) of clinical care at 130 US hospitals and integrated delivery networks. It includes over 50 features representing patient and hospital outcomes. Information was extracted from the database for encounters that satisfied the following criteria.
1. It is an inpatient encounter (a hospital admission).
2. It is a diabetic encounter, that is, one during which any kind of diabetes was entered to the system as a diagnosis.
3. The length of stay was at least 1 day and at most 14 days.
4. Laboratory tests were performed during the encounter.
5. Medications were administered during the encounter.
 
#### The data contains such attributes as patient number, race, gender, age, admission type, time in hospital, medical specialty of admitting physician, number of lab test performed, HbA1c test result, diagnosis, number of medication, diabetic medications, number of outpatient, inpatient, and emergency visits in the year before the hospitalization, etc.


Our project was about a dataset that has infos abour **diabetics people in 130-US hospitals.** 

First, we took that dataset and tried to understand every column of it, which let to the **columns description** in the begining of the notebook.

Then, we decided to do some **basics graphics**, with some interesting groups by age, weight, gender, number of medecines, ... We saw that some parameters are **useless alone**, while other seemeed to be **interesting.**

So we took those interesting parameters, and we started to do more **complete analysis**. For example we did a heatmap about the weight and age of the people in the hospital, which let to the description of a **typical profile** of a patient. Afer all those graphics, we found our target for the machine learning, since the dataset didn't have any. 

We decided to target the **Time in hospital**. In order to do that, we changed every useful variable possible into floats and integers. This parameter seemed to be quit useful, and was already a **safe value**, since we didn't touch it. We did a **correlation matrix**, which wasn't very promising at first sight. But we tried a lot of **machine learning models**. We did the necessary transformations and **ranked them**. Then we choose the one that, for us, had performed better, which was the **Support Vector Machine.** After getting that result, we optimised it by changing to parameter **gamma.** In the end, we had a model that seemed to be working correctly, with a good score. The last graphic show us that he most important parameter for our data was by far the **number of medications** that the patient have been given. 


### Conclusion

By targeting this parameter, we aimed to optimise the **planification** of the rooms and beds, depending of the profile of the patient. This prediction could help the hopital workers to plan better the **preparation** of the rooms, so that it is easier for them to assign people to rooms and clean them. But this prediction could also help **patients**, so that they have their room **clean and ready**, and they can have an **expected date of release**. The model could also help the hospital to **prioritize patient** according of their profile, and the medicines that they need. 
We can also say that other data could be interesting to analyse, like the **number of meds** necessary - to have a better stock managemenent -, the **most used** meds and the one that are to a **very specific** type of patient, or the **number of lab procedures** needed for each patient.
