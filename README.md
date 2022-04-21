# Final-Project-Proposal
Final Project/ Code for BIOL 599


## Formatting of data files
    Each column heading is either a data column or contains numerical data of different water quality parameter
    
    
  ## In File OysterLanding_dat.csv the following named columns are:
    
   **Date_Sens**: Date/ Time stamp of sensor data in North Inlet
   **Temp**: Temperature data
   ** Sal**: Salinity Data
   **DO_pct**: Dissolved Oxygen percentage
   ** ChlFluor**: Sensor Chorophyll data 
   **Date_Lab**: Date/ Time stamp of lab data in North Inlet
   ** CHLA_N**: Chlorophyll data collected by traditional lab methods
   **F_Temp, etc**.: All F_paramter columns are columns where QA/QC codes are included for suspect data that was       removed
   
   
  
  ## In File WinyahBay_dat.csv headings are the same as above
  
  **Date_sens**: Date/ Time stamp of sensor data in Winyah Bay
   **Temp**: Temperature data
   **Sal**: Salinity Data
   **DO_pct**: Dissolved Oxygen percentage
   **ChlFluor**: Sensor Chorophyll data 
   **Date_lab**: Date/ Time stamp of lab data in Winyah Bay
   **CHLA_N**: Chlorophyll data collected by traditional lab methods
   **F_Temp, etc**.: All F_paramter columns are columns where QA/QC codes are included for suspect data that was       removed
  
  
  ## In File Oyster_Landing_Tidal.csv 
  
  **Date_sens**: Date/ Time stamp of sensor data in North Inlet
   **Temp**: Temperature data
   ** Sal**: Salinity Data
   **DO_pct**: Dissolved Oxygen percentage
   ** ChlFluor**: Sensor Chorophyll data 
   **Date_Lab**: Date/ Time stamp of lab data in North Inlet
   ** CHLA_N**: Chlorophyll data collected by traditional lab methods
   **F_Temp, etc**.: All F_paramter columns are columns where QA/QC codes are included for suspect data that was       removed
  
  
  
  
 ## In File Winyah_Bay_Tidal.csv
 
   **DateTimeStamp**: Date/ Time stamp of sensor data in Winyah Bay
   **Temp**: Temperature data
   **Sal**: Salinity Data
   **DO_pct**: Dissolved Oxygen percentage
   **ChlFluor**: Sensor Chorophyll data 
   **DateTimeStamp**: Date/ Time stamp of lab data in Winyah Bay
   **chla ug/L**: Chlorophyll data collected by traditional lab methods
   **F_Temp, etc**.: All F_paramter columns are columns where QA/QC codes are included for suspect data that was       removed
   
   
   
   
## Where to access more Water Quality/ Nutrient Data from the NOAA/NERR CDMO

https://cdmo.baruch.sc.edu

**Choose the NERR site that you want to request data from the VIEW/DOWNLOAD data interactive map**

**Choose what format you want your data in, the files for this project were requested using the Advance Query System**

**From there you can customize if you want Water quality/ Nutrient/ Meteorlogical data as well as dates that you want your data from**


## Example Code for formatting dates in R

OL_dat$Date_Sens <- as.Date(OL_dat$Date_Sens, format = "%m/%d/%y")

  Changing the column 'Date_Sens' into as date format (as.Date) and specifying the exact date format, 
  'format = %m/%d/%y' , which makes the date format into month, day, year for the entire column
  
  
  
## Example code filterting for certain dates


 OL_dat_yearly <- OL_dat %>% filter(Date_Sens >= as.Date('2021-01-01') & Date_Sens <= as.Date('2021-12-31'))
 
 






  
   
    
