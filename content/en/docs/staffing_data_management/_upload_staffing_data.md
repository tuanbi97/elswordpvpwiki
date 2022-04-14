---
title: "Upload Staffing Data"
linkTitle: "Upload Staffing Data"
weight: 1
description: >
  In this section we will learn how upload staffing data into Palexy system.
---

## Prerequisites
- Your account must have `Admin` or `Store Manager` role
- You must know the store code of the store you are updating 

## Steps
1. Go to `Store Staffing Management` page using top menu in `CONFIGS` section
<img src="https://storage.googleapis.com/palexy-static-files/documents/staff_menu.jpg"
     alt="Staffing Menu"/>

2. In Staffing Data Management page, click on `Batch Upload` button to go to upload page.
<img src="https://storage.googleapis.com/palexy-static-files/documents/staff_overview.png"
     alt="Staffing Data Overview"/>

3. Below is the UI of Upload Staffing Data page.
<img src="https://storage.googleapis.com/palexy-static-files/documents/staff_upload_with_date.png"
     alt="Staffing Upload Page"/>

4. Firstly, please choose the date range that you want upload staffing data for at `Apply date range` field. Note that this field is required and only data within this range will be updated.
<img src="https://storage.googleapis.com/palexy-static-files/documents/staff_upload_select_date.png"
     alt="Staffing Upload Page Select Date"/>

5. Next is to select files to upload. We allow user to upload mutliple staffing files at the same time. The format of the file name has to following the following example syntax: if you want to upload staffing data for May of 2021 for a store with name Palexy Central and code 123456, you will need to select apply date range from May 1, 2021 to May 31, 2021, and the file will be named **123456_Palexy Central.xlsx**. 

    Now please choose your files and click `Upload Files` to upload. In the UI below we upload 2 files for store AAA and BBB:
<img src="https://storage.googleapis.com/palexy-static-files/documents/stafll_upload_date_select_files.png"
     alt="Staffing Upload Select Files"/>
  
    *Please note that the content of the file has to conform with the format that has been agreede between your organization and Palexy*

    *Contact your admin if you do not know what is your store code*

6. In case of success, the UI will look like below.
<img src="https://storage.googleapis.com/palexy-static-files/documents/staff_upload_success.png"
     alt="Staffing Upload Success"/>

7. In case of failure the UI will look like below. Please read the error message carefully to understand what go wrong with the failed files.
<img src="https://storage.googleapis.com/palexy-static-files/documents/staff_upload_partial_fail.png"
     alt="Staffing Upload Partial Fail"/>

     *Note that when uploading multiple files, some files may succeed and some files may fail, only failed files that needs to correct and upload again.*
     
After data is uploaded succesffuly, you can follow the guide at [Review Staffing Data]({{< ref "_review_staffing_data.md" >}}) section to check if the data has been processed correctly.


## How data is processed
- If upload fails, nothing will change.
- If upload succeeds, all data in the applied date range be removed and replaced by data on that date range found in the uploaded file. 