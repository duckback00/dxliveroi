# dxliveroi

Delphix Live ROI

(EDITS are a WIP)

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
  - Wait a few seconds for the Live ROI to establish connection into the Delphix Engine and retrive the data
  - You will see the Live ROI updating the "Dashboard" sheet

More to come...



