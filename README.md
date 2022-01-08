# ABHAuctionPostmanSmokeTest

- This is a collection used to automate the manual api tests for the https://abh-auction.herokuapp.com/ app.
The collection contains an environment called "New User" and all the necessary colection variables. 
All requests contain tests and some such as the "sign up" request contain pre-request scripts.

# Test Runs:
## 1. Postman
1. Install Postman
2. Select File and click import
3. Import the .json file from the repository
4. Test run methods:
     - Run the tests using test runner by dragging and dropping the collection into the test runner
     - Run the test using the Monitor by creating a new monitor and selecting the collection

## 2. Command prompt
1. **Install newman using this command:** npm install -g newman
2. **Install newman report tool using this command:** npm install -g newman-reporter-htmlextra
3. cd into the directory where the api.json file that you pulled from git is.
4. Test run methods:
     - **To just run the test in the cmd use:** newman run ABHAuctionApp-smokeTest.postman_collection.json
     - **To run the test and get a html report generated in the same folder as the api.json use:** newman run ABHAuctionApp-smokeTest.postman_collection.json -r htmlextra
