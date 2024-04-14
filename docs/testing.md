# Testing

## Test Plan
TODO: Describe any manual and automated (unit) tests. Uniquely identify each test case. Include prerequisites and test data.

Test Runs
TODO: For each test described above, indicate the current status. 
Create a requirements traceability matrix to validate the completeness of the product.

| Use-Case ID | Requirement ID | Test Case | Status |
| ----------- | -------------- | --------- | ------ |
| Use Case 1 | FR1.1 | The system should allow the user to find the nearest charger - The System does this perfectly | Pass|
| Use Case 1 | FR1.2 | The system should add markers for each charger on the map - The system does this | Pass |
| Use Case 1 | FR1.3 | The system should get permission to access user location via geolocation object. | Pass |
| Use Case 1 | FR1.4 | The system must query the database to get the charger coordinates. | Pass |
| Use Case 2 | FR2.1 | The system should allow the user to find and filter chargers based on their type using UC2. - The system does this and filters on the socket type and distance from the user | Pass |
| Use Case 3 | FR3.1 | The system should provide the user with directions to the charger using UC3. | Fail - UC3 has not yet been added to the project |
| Use Case 1 | NFR1.1 | The app should work on mobile (Portability). | To be tested |
| Use Case 1 | NFR1.2 | The app should display up to 5 of the closest chargers at a time (Usability). | Pass |
| Use Case 1 | NFR1.3 | There is no security required (Security). | To be tested |
| Use Case 1 | NFR1.4 | The source code should be accessable from GitHub (Maintainability). | Pass |
| Use Case 2 | NFR2.1 | The app should return formatted data to the user within 5 seconds (Performance Efficiency). | To be tested |
| Use Case 2 | NFR2.2 | The app should work on different browsers e.g. Chrome and Safari. And the app should work on different types of devices e.g. Mobile and Desktop (Compatability). | To be Tested |
| Use Case 2 | NFR2.3 | The map should default view to bristol if no location data is available (Reliability). | Pass | 
| Use Case 3 | NFR3.1 | The data used by the app should be up to date; Less than one year old (Functional Suitability). | To be tested |


