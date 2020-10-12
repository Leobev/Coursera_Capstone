# Coursera_Capstone: Car accident severity analysis for Seattle

Used for Applied Data Science capstone project

# Business Understanding:

Road accidents carry a substantial economic cost to the city of Seattle.  The local government is interested in analysis of collision data to help inform decisions that will hopefully reduce the volume and severity of traffic collisions in the city.  The objective is to develop a model that can accurately demonstrate a relationship or otherwise between accident severity and other variables within the dataset.  The strength of the relationships will help determine where resources should be prioritised.

# Data Understanding:

The collisions data was provided by the Seattle Police Department and recorded by Traffic Records Group of the SDOT Traffic Management Division.
The data is updated weekly and spans a period from 2004 to mid 2020.  The dataset has 194,673 rows and 37 attributes excluding 1 duplicate. 
Attributes with significant missing data, duplicate data or data not relevant to the objective will not be used for the model.

The dependant variable is labeled 'SEVERITYCODE', using a code that corresponds to the severity of the collision.

* 3 - fatality
* 2b - serious injury
* 2 - injury
* 1 - prop damage
* 0 - unknown

SEVERITYCODE
