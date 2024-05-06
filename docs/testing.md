# Testing

## Test Plan
Testing for the Car Charger Finder application will utilise both manual and automated approaches to ensure comprehensive coverage. Manual testing will involve real user scenarios to validate features like finding the nearest charger and filtering based on type. Automated testing will focus on unit tests for specific functions and integration tests to ensure seamless component interaction. Performance, compatibility, and security testing will also be conducted to assess efficiency, cross-device functionality, and system robustness. This combination of testing methodologies aims to ensure that the application meets all functional and non-functional requirements, providing users with a reliable and user-friendly experience.

## Tests

| Test Case | Description               | Testing Approach            | Prerequisites     | Test Data               |
|-----------|---------------------------|-----------------------------|-------------------|-------------------------|
| UC1 - FR1.1 | The system should allow the user to find the nearest charger.| Manual testing with real user scenarios | Access to the application, a browser with geolocation support | Testers' actual location coordinates |
| UC1 - FR1.2 | The system should add markers for each charger on the map.| Automated unit testing  | Unit testing framework set up, map rendering functionality implemented | Mock charger data with known coordinates |
| UC1 - FR1.3 | The system should get permission to access user location via geolocation object.  | Manual testing | Access to the application, a browser with geolocation support | N/A (User interaction) |
| UC1 - FR1.4 | The system must query the database to get the charger coordinates.| Automated unit testing combined with integration testing| Access to the database, database connection established | Mock charger data stored in the database |
| UC2 - FR2.1 | The system should allow the user to find and filter chargers based on their type using UC2.| Manual testing with real user scenarios | Access to the application, filtering functionality implemented | Testers' actual location coordinates, mock charger data |

## Test Runs (Requirements)

| Use-Case ID | Requirement ID | Test Case | Status |
| ----------- | -------------- | --------- | ------ |
| Use Case 1 | FR1.1 | The system should allow the user to find the nearest charger - The System does this perfectly | Pass|
| Use Case 1 | FR1.2 | The system should add markers for each charger on the map - The system does this | Pass |
| Use Case 1 | FR1.3 | The system should get permission to access user location via geolocation object. | Pass |
| Use Case 1 | FR1.4 | The system must query the database to get the charger coordinates. | Pass |
| Use Case 2 | FR2.1 | The system should allow the user to find and filter chargers based on their type using UC2. - The system does this and filters on the socket type and distance from the user | Pass |
| Use Case 3 | FR3.1 | The system should provide the user with directions to the charger using UC3. | Fail - UC3 has not yet been added to the project |
| Use Case 1 | NFR1.1 | The app should work on mobile (Portability). | Pass - iPhone |
| Use Case 1 | NFR1.2 | The app should display up to 5 of the closest chargers at a time (Usability). | Pass |
| Use Case 1 | NFR1.3 | There is no security required (Security). | Can't be tested |
| Use Case 1 | NFR1.4 | The source code should be accessable from GitHub (Maintainability). | Pass |
| Use Case 2 | NFR2.1 | The app should return formatted data to the user within 5 seconds (Performance Efficiency). | Pass depending on internet speed |
| Use Case 2 | NFR2.2 | The app should work on different browsers e.g. Chrome and Safari. And the app should work on different types of devices e.g. Mobile and Desktop (Compatability). | Pass |
| Use Case 2 | NFR2.3 | The map should default view to bristol if no location data is available (Reliability). | Pass | 
| Use Case 3 | NFR3.1 | The data used by the app should be up to date; Less than one year old (Functional Suitability). | To be tested |
