## Technical Architecture for Fizzyo Implementation

HealthVault [Microsoft HealthVault](https://www.healthvault.com/en-us/)
is a private data store for an individual’s personal data and gives you the security model (HIPPA approved, etc.) and the granularity to share with different members of the care team (i.e., your parent, your clinician, etc.).  

To aggregate data together for reporting and Machine Learning we are recommending collating game data in DataBase, such as Azure SQL. 

The API and Azure Function will anonymise the data before it makes its way into Azure SQL.  
 
[HealthVault Developer API](https://developer.healthvault.com) 
   
## Architecture Diagram

![Archiecture Design](https://github.com/Fizzyo/Architecture/blob/master/Images/Architecture.png)   
 
 This will provide the the ability to source data from other devices (i.e., fitness trackers, etc.) 
 
 The larger goal would be to use something like Azure Data Lake at the 3rd Party Trusted Source and add a reference to the source in either HealthVault or your DB.
 
With HealthVault you can create very basic dashboards and the API supports care plans.  We’re planning on fronting HealthVault with an API, which opens up PowerBI.com to create the visualisations and allows an app ecosystem to interact with the HealthVault data, like bots for example and dashbaords for patient, career, parents and medics.
