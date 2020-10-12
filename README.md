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

SEVERITYCODE contains a balanced mix of 1 and 2 codes and won't require under-sampling.  However other attributes such as 'LIGHTCOND' (which contains data related to the light conditions at the time of the collision), will require under-sampling in order to avoid a biased fit with respect to a prevalence of 'Daylight' entries.  The dataset is quite large so under-sampling shouldn't have a negative effect on accuracy.  The data will need to be cleaned due to the presence of null values for some attributes.

Initial attributes that may have a notable relationship with accident severity:

* LOCATION - location of collision using two street names.
* JUNCTIONTYPE - category of junction at which collision occurred.
* INATTENTIONIND - Whether or not collision was due to inattention (Y/N).
* COLLISIONTYPE - type of collision (e.g. rear-ended).
* PERSONCOUNT - total number of people involved in the collision.
* PEDCOUNT - number of pedestrians involved in collision.
* PEDCYLCOUNT - number of bicycles involved in collision.
* VEHCOUNT - number of vehicles involved in collision.
* INCDTTM - date and time of collision
* WEATHER - description of weather conditions during collision.
* ROADCOND - condition of road during collision.
* LIGHTCOND - light conditions during collision.
* SPEEDING - was speeding a factor in the collision (Y/N).
* SEGLANEKEY - lane segment in which collision occurred.
* CROSSWALKKEY - crosswalk at which collision occurred.
