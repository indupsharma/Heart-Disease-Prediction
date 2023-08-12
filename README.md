# Heart-Disease-Prediction
This is a group project done under the supervision of Prof. Charles Lynch as a part of the course, Information: Representation, Processing, and Visualization (AIT664).
Team: Indu Priya Sharma, Sai Sujit, and Kishore Nanda
The references to the data are mentioned below
Project has the below mentioned files
  1. Project report
  2. Code worked on
  3. CSV data file
  4. tableau visualizations

The team had chosen this topic to focus on below area
      Heart Disease and attacks are among the most prominent health issues in the United States. According to the CDC [1], the highest cases of death is due to heart disease in the United States. The United States observes one death every 34 seconds on the account of a ‘cardiovascular disease’. In 2020, according to the statistics, one out of every 5 deaths happening was due to heart disease which accounted for nearly 700,000 deaths. Almost 805,000 people had a heart attack in the United States out of which nearly 25% had already had an attack. So, this issue is a critical risk factor and needs attention. The focus is to predict or detect the chance/likelihood of Heart Disease/ Attack using data analytics and machine learning to assist medical workers and the public.

About Data:
  The dataset is easily found and available on UCI Machine Learning website, and could also be found in Kaggle. The dataset consists of 75 attributes, but only 14 are utilised as per the project requirements the team worked on. There are 8 categorical and 5 numerical variables along with one target variable. Here is an overview on the attributes that our project would be focusing on:
  
  ●	Age: Numerical Variable
         This attribute tells about the age of the patient. This can help us understand the distribution of affected and unaffected patients. 
         This can also be utilised as a categorical variable once we use this as an interval range: under x years, x- y years and so on 
         (depending on the initial exploratory data analysis).
	 
  ●	Sex: Categorical Variable
         This attribute has two values: 1 and 0 which signifies the two types of gender.
	 
  ●	Exang: Categorical Variable
           This attribute has two values: 1 and 0.
           1 indicates that exercise has caused angina which basically is a condition that results in 
           chest pain.
           0 indicates that exercise was not the reason behind angina.	
	   
  ●	Ca: Categorical Variable
        This attribute has values ranging from 0 to 3 which tells about the number of major vessels.
  
  ●	Cp: Categorical Variable
        This attribute has values ranging from 1 to 4 which tells about the pain type:
        ○  1: Typical Angina									
        ○  2: Atypical Angina
        ○  3: non-Anginal Pain
        ○  4: Asymptomatic		
  
  ●	Trtbps: Numerical Variable
            This variable tells about the resting blood pressure and the units is mm Hg.		
  
  ●	Chol: Numerical Variable
          This variable tells about the person’s cholesterol which is measured by BMI Sensor and the unit is mg/dl.		
  
  ●	Fbs: Categorical Variable
         This attribute has two values: 1 and 0.
         1 indicates that exercise has caused angina which basically is a condition that results in chest pain.
         0 indicates that exercise was not the reason behind angina.
  
  ●	Rest_ecg: Categorical Variable
              This attribute has values ranging from 0 to 2 which tells about the resting electrocardiographic results:	
              ○  0: Normal Ecg					
              ○  1: Person has ST-T wave abnormality							
              ○  2: Person has probable or definite left ventricular hypertrophy by Estes’ criteria
 
  ●	Thalachh: Numerical Variable
              This attribute tells about the maximum heart rate noted
  
  ●	Target: Categorical Variable
            This attribute has two values: 1 and 0.
             1 indicates that the patient has a likelihood of heart attack/disease.
             0 indicates that exercise was not the reason behind angina.
            This will also be utilised as the target variable that can be used for building ML models.

Below are a few quesetions that the team had worked on finding the answers
					 				
Questions:

1.	Some of the essential questions we wish to answer during our project:
2.	What is the most critical factor that may cause Heart Attack/ disease?
3.	What factor can reduce the likelihood of Heart Attack/ disease?
4.	What insights can be gained using this dataset that can assist Medical experts?
5.	What model will help in accurately predicting future likelihood? 
6.	How the heart rate of a person will have an impact on the chances of getting a heart attack?
7.	How does the age factor affect the raise of heart attacks in a person?
8.	Which sex category is mostly affected by heart attacks?

To answer the above questions the team had worked on the below analysis.

Data Cleaning:

Defination: The process of fixing or removing the incorrect, corrupted, incorrectly formated, duplicate or incomplete data within the dataset[4].

As per the heart.csv file there were no missing values found and the data looked fine. Altough it was found that the data could be normailized which was done post the exploratory data analysis.

Exploratory Data Analysis:

Defination: EDA is used by data scientist to analyse and investigate the data set and summarize their main charteristics, often emoploying data visualization methods. It best manuplicates the data sources to get the answers you need, making it simpler to find patterns, spot the anomalies, test hypothesis and check assumptions [5].

Basic exploration of data was performed using Python to find various statistics of the obtained data. Intiall, distribution of data was taken and parameters which were considered are observed.

<img width="454" alt="EDA" src="https://github.com/indupsharma/Heart-Disease-Prediction/assets/133023339/8a4d7dc9-03da-4ff5-8eac-6ef1c8c6fffd">

The team believed that the heart attack is depended on the factors such as age, sex, cholesterol and heart rate(thalachh). So, analysis was done on each facotr individually which is as follows:

Based on the analysis performed on the sex and occurrence of attack, it was observed that, males highly suffered cardiac arrest.

<img width="208" alt="image" src="https://github.com/indupsharma/Heart-Disease-Prediction/assets/133023339/3ade663e-78de-4c1e-9835-4c9e3671c341">

Other important factor that was focused was age. The age was collated into age groups to better understand the results. Post analysis results show that people of age group 60 had dear chances of cardiopulmonary arrest.

Below graphs shows us the results of the analysis:

<img width="228" alt="image" src="https://github.com/indupsharma/Heart-Disease-Prediction/assets/133023339/c8962589-2905-4b0c-919b-6699cf186786">

In the next steps the analysis was performed based on the heart rate and the age. As, per the report the occurrence of cardiac arrest is highly probable with increase in the heart rate. Maximum people below the age group of 53 had coronary infractory, on the other hand the age group rangin from 55 to 70 did not show any signs of occurrence. The heart rate of people who had attack ranged to maximum 200, to as low as 100.

It was also observed that the chest pain type (cp = 0) typical angina (chest pain due to excess physical and emotional stress) was one of the reasons causing coronary thombrosis.


  ![image](https://github.com/indupsharma/Heart-Disease-Prediction/assets/133023339/1b89b757-893b-4ca3-a731-1f669c3646d6)


















References: 

[1] Heart Disease Facts | cdc.gov. (2022, July 15). Centers for Disease Control and Prevention. Retri eved September 18, 2022, from https://www.cdc.gov/heartdisease/facts.htm 

[2] UCI Machine Learning Repository: Heart Disease Data Set. (n.d.). Retrieved September 18, 2022, from https://archive.ics.uci.edu/ml/datasets/Heart+Disease 

[3] Kaggle: Your Home for Data Science. (n.d.). Retrieved September 18, 2022, from https://www.k aggle.com/datasets/rashikrahmanpritom/heart-attack-analysis-prediction-dataset+

[4] “Guide to data cleaning: Definition, benefits, components, and how to clean your data,” Tableau, https://www.tableau.com/learn/articles/what-is-data cleaning#:~:text=tools%20and%20software-,What%20is%20data%20cleaning%3F,to%20be%20duplicated%20or%20mislabeled. (accessed Aug. 5, 2023). 

[5] What is exploratory data analysis? (no date) IBM. Available at: https://www.ibm.com/topics/exploratory-data-analysis (Accessed: 05 August 2023). 



