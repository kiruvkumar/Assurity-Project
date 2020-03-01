# Assurity-Project

https://api.tmsandbox.co.nz/v1/Categories/6327/Details.json?catalogue=false

# Acceptance Criteria

  Name = "Carbon Credits"
  CanRelist = true
  The promotions element with Name = "Gallery" has a Description that contains the text "2x larger image"
  
This is postman collection file which contains the tests. I have used Postman and Newman for this assignment and validated using Custom JS. You can use this file and run below commands. This will help run the test from command line or from a CI/CD platform like Jenkins too.

All three acceptance criteria are created as tests and they pass. I have also tested with different combinations too.

Test reporting is also configured which exports html report

# Below are one time setup steps to run the tests from cmd/ Jenkins:

npm install -g newman
npm install -g newman-reporter-htmlextra

# Command to run the test from cmd/ Jenkins
newman run AssurityTest.postman_collection.json --reporters cli,htmlextra --reporter-htmlextra-title "ASSURITY API TEST REPORT" --reporter-htmlextra-darkTheme --reporter-htmlextra-export "newman/AssurityTestTestReport.html"


