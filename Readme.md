## Technical Architecture for Fizzyo Implementation

## Architecture Diagram

![Architecture Design](https://github.com/Fizzyo/Architecture/blob/master/Images/FizzyoArch.JPG)   
 
 This will provide the the ability to source data from other devices (i.e., fitness trackers, etc.) 

 ## Fizzyo API 

The Fizzyo API is fully documented at 
[Fizzyo API](https://api.fizzyo-ucl.co.uk/)

## Fizzyo Platform

 ![Fizzyo Tech Stack](https://github.com/Fizzyo/Architecture/blob/master/Images/Fizzyotech.JPG) 


## Data Analysis
 
![Data Analysis Architecture](https://github.com/Fizzyo/Architecture/blob/master/Images/Fizzyoda.png)   
## Data Visualisation 

## Microsoft HealthVault

HealthVault [Microsoft HealthVault](https://www.healthvault.com/en-us/)
is a private data store for an individual’s personal data and gives you the security model (HIPPA approved, etc.) and the granularity to share with different members of the care team (i.e., your parent, your clinician, etc.).  

To aggregate data together for reporting and Machine Learning we are recommending collating game data in DataBase, such as Azure SQL. 

The API and Azure Function will anonymise the data before it makes its way into Azure SQL.  
 
[HealthVault Developer API](https://developer.healthvault.com) 
With HealthVault you can create very basic dashboards and the API supports care plans.  We are fronting HealthVault with an API and using PowerBI.com to create the visualisations and allows an app ecosystem to interact with the HealthVault data, like bots for example and dashbaords for patient, career, parents and medics.
