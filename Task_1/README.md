Data Loading:

The dataset "Medical Appointment.csv" was loaded into a Pandas DataFrame named df\_raw.

Data Exploration:

The dataset was explored to understand its structure, data types, and potential issues.  
Missing values, duplicates, and inconsistent data formats were identified.  
Special attention was given to the 'ScheduledDay' and 'AppointmentDay' columns to check for data type and format inconsistencies.

Data Cleaning:

Negative ages were handled by replacing them with the median age.  
Missing values were checked for and imputed appropriately. Since no missing values were present, no imputation was done.  
Duplicate rows were removed.

Data Wrangling:

Text values in the 'Gender' and 'Neighbourhood' columns were standardized.  
Date columns ('ScheduledDay', 'AppointmentDay') were converted to datetime objects.  
A new column, 'days\_until\_appointment', was created to calculate the time difference between scheduling and appointment dates.  
Columns were renamed to a uniform format (e.g., 'PatientId' to 'patient\_id').  
Data types were ensured to be correct (e.g., 'age' as an integer).

The cleaned and prepared dataset is stored in a new DataFrame named df\_wrangled.  
The cleaned dataset was saved to a CSV file named "cleaned\_data.csv".  
Overall, the cleaning and preparation process involved handling missing values, removing duplicates, standardizing text and date formats, creating a new feature, renaming columns, and ensuring correct data types. This resulted in a cleaner and more consistent dataset suitable for further analysis.