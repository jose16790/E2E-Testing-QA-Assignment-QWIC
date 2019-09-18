# E2E-Testing-QA-Assignment-QWIC by Jose Durai Prabhakar 

https://www.linkedin.com/in/jose16790/

# API/UI Integration Tests using Postman/Newman

Assumptions : npm is installed and available in the machine. 

If node.js is not installed, follow the steps in the below link.
 
https://learning.getpostman.com/docs/postman/collection_runs/command_line_integration_with_newman/

After node.js is ready to use, follow below steps

1. Open node.js prompt and run below command to install newman globally, remove -g to install locally. 

   npm install -g newman

2. Verify if newman is installed, run below command. Version will be displayed. 

   newman -v 

# Execution of Test Suite: 

1. Run the QA Assignment application shared by Sil in Diego's Git link (
https://github.com/qwicengineering/qa-assignment), following the same procedure. Project is also downloaded along with this git repo.


   Run the application from Search-Form folder

   npm run start 

Once the message displays as "Application is running" follow below steps

2. Open a new command prompt and navigate to the folder "E2E-Testing-QA-Assignment-QWIC" in the downloaded repo, using 'cd' command
 Ex : cd C:\Users\jose\E2E-Testing-QA-Assignment-QWIC
 
3. Execute the Test Suite using the below command (The JSON mentioned below is the executable file for Newman, generated from postman tests I've written) 

   newman run Tests-for-Car-API-newman.json -r cli 

-r cli is for viewing the test report in the command line. -r progress or -r json can be used as well. 

# Please read the detailed document I crafted for the E2E framework proposal, design and assumptions along with E2E/Integration test cases for the application 

https://docs.google.com/document/d/191IHPwj9SucXH7Fa6-CYtZAs8ZCgrM03Tk0eyJPpzKc/edit?usp=sharing 
