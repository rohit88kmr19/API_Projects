# API_Projects

**First Download all the Collections and Import it via Postman, you will be able to see all the collecitons with the below points.**

- There are three projects with different requests run on Newman and Command Line interface.
- The reports are also attached with results (Total Test Cases, Assertions, Failed,Passed).
- Different Methods like Get, Post, Put, Delete , Patch, Head.
- You will be able to see the Test scripts written with different Test Cases in Java Script for the response validation.
- The collections can be run in Postman also by clicking Run collection Option.

 **How to use the newman**

1. Install the node JS
    1. [﻿nodejs.org/en/download/package-manager](https://nodejs.org/en/download/package-manager) 
3. Open the CMD and verify that node and npm are installed. 
    1. node --version
    2. npm --version
    3. npm install -g newman
    4. newman --version
    5. npm install -g newman-reporter-htmlextra
4. Run the collection 
    1. newman run Collection URL -r htmlextra,cli` 

**How to get Collection URL**
1. Click on three dots on the colleciton and select share from the window pane.
2. Select the Via Api tab from the popup.
3. Click on Generate key and then copy the URL.
4. Use the copied URL instaed of Collection.json in the command  newman run Collection.json -r htmlextra,cli .

**Running the API via Newman based on Environment variable like Prod, QA**
1. Download the Project and Environment variable also.
2. Copy the path for both the folder and use the below command to run on  newman.
3. newman run "C:\Users\Asus\Postman\files\Restfull Booker.postman_collection.json" -e "C:\Users\Asus\Postman\files\Prod Env.postman_environment.json" -r htmlextra,cli
4. New Folder will create with newman then report will be visible there.

