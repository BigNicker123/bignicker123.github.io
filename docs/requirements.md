# Requirements

## User Needs

### User stories
* As an electric car user I want to find car chargers so I can charge my car.
* As a user, I want to filter charging stations based on the type of charger (e.g., Level 2, DC Fast Charger) so that I can choose the one that is compatible with my electric car. <br>
* As a user, I want to be able to see the charging station's operating hours and pricing information, if available, so that I can plan my charging stops efficiently and budget for it. <br>
* As a user, I want the app to provide directions to the selected charging station, either through an integrated navigation system or by launching a third-party navigation app. <br>

### Actors
Actors that appear in the following use-cases are as follows:

* Driver - An electric car user

### Use Cases

| UC1 | Find nearest charger | 
| -------------------------------------- | ------------------- |
| **Description** | Show the charger and driver on the map with the driver at the centre |
| **Actors** | Driver |
| **Assumptions** | None
| **Steps** | <ol><li>Select the map</li><li>Give permission to use location</li><li>Get charge coordinates for database</li><li>Centre map on user location</li><li>Add a marker on the map for each charger</li></ol> |
| **Variations** | None |
| **Non-functional** |  |
| **Issues** |  |

| UC2 | Find type of charger | 
| -------------------------------------- | ------------------- |
| **Description** | To allow the driver to filter the type of charger,(e.g., Level 2, DC Fast Charger) |
| **Actors** | Driver |
| **Assumptions** | Permission has been given to use location</td></tr>
| **Steps** | <ol><li>Show a drop down menu</li><li>Allow user to filter options from menu</li><li>Show filtered results with a marker on the map for each charger</li></ol> |
| **Variations** | None |
| **Non-functional** |  |
| **Issues** |  |

| UC3 | TODO: USE-CASE NAME | 
| -------------------------------------- | ------------------- |
| **Description** | TODO: Goal to be achieved by use case and sources for requirement |
| **Actors** | Driver |
| **Assumptions** | TODO: Pre/post-conditions if any</td></tr>
| **Steps** | TODO: Interactions between actors and system necessary to achieve goal |
| **Variations** | TODO: OPTIONAL - Any variations in the steps of a use case |
| **Non-functional** | TODO: OPTIONAL - List of non-functional requirements that the use case must meet. |
| **Issues** | TODO: OPTIONAL - List of issues that remain to be resolved |


![Use-Case Diagram](Images/UseCase-Diagram1.png)

## Software Requirements Specification
### Functional requirements
TODO: create a list of functional requirements. 
    e.g. "The system shall ..."
    Give each functional requirement a unique ID. e.g. FR1, FR2, ...
    Indicate which UC the requirement comes from.


### Non-Functional Requirements
TODO: Consider one or more [quality attributes](https://en.wikipedia.org/wiki/ISO/IEC_9126) to suggest a small number of non-functional requirements.
Give each non-functional requirement a unique ID. e.g. NFR1, NFR2, ...

Indicate which UC the requirement comes from.
