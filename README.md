# dxliveroi

Delphix Live ROI

Goal: Provide to the user a real-time value (quantified in $) from using Delphix.

The Delphix Live ROI is an Excel Workbook that:
  - uses Delphix APIs to connects to the Delphix Engine (DE)
  - retrieves from the DE all jobs (with start/end/elapsed time) and storage data (usage)
  - computes a real-time dashboard on the value of Delphix for certain jobs performed
  
How to use Live ROI:
  - when opening the XLS, make sure you accept to enable macros
  - go to the "Config" sheet and enter value for
    - Hostname/IP Address of the Delphix Engine
    - Username and Password for a Delphix user
    - Make any edits you want in the "Current/Legacy Customer Process" section
  - press the "Fetch Data"
  - Confirm that the connection parameters are corrrect
  - Wait for a panel to be displayed confirming that Live ROI established connection and retrived data
  - You will see the Live ROI updating the "Dashboard" sheet
  
Explanation of Worksheets:

Dashboard Worksheet 
  Sums the number of times VDBs are PROVISION, REFRESH and REWIND.	
	Legacy Time - Time is used to take to perform an operation in the past [Customer Input Data]	
	Time in Delphix - Total elapsed time it took in Delphix to perform operations	
	Hours Saved with Delphix - Legacy time minus elapsed time	
	Value of Saved Time - Hours saved with Delphix * blended labor cost [Customer Input Data])
  Storage Savings - Disk space saved (coming from Delphix and stored in Data1 sheet) * storage cost [Customer Input Data]
  Combined Savings - Total of all "Value of saved time" + storage savings
		
Config Worksheet
  Configuration Data: Only change the fields in blue	
		
Data Worksheet
  Data on jobs returned from the Delphix Engine
  
Data1 Worksheet
  Data on storage returned from the Delphix Engine
  	
Read Me Worksheet
  Help on using Live ROI
  
Reference Industry Data Worksheet
  Sample of key metrics for 25 Delphix customers
