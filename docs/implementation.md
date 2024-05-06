# Implementation

## Introduction

`FindNearestCharger.hmtl` utilises both the Mapbox API and Bristol Open Data API to pinpoint nearby electric vehicle charging stations. By leveraging the user's geolocation, it organises and presents charger details in a table format, featuring name, location, type, socket type, and distance. 

The dataset, obtained from the Bristol Open Data API, offers information on electric vehicle charging points, encompassing attributes such as name, location coordinates, charger type, and socket type. It is relatively small, containing only 26 rows. However, to streamline the user experience, various columns containing unnecessary information for the web app's purpose have been filtered out.

`FilterCharger.html` extends the capabilities of `FindNearestCharger.html` by integrating filtering mechanisms for electric vehicle charging stations. Users can now specify charger type, socket type, and distance filters to refine their search criteria. Upon applying these filters, the code dynamically sorts the charging stations based on their proximity to the user's location and displays the filtered results both on the map and in a table format. This sorting process involves calculating the distance between each charging station and the user's location, followed by sorting the stations in ascending order based on this distance metric. Finally, the sorted charging stations are presented to the user, providing a more tailored and efficient means of discovering nearby charging options.

Configuration data includes the API endpoint URL for charger data retrieval and the Mapbox access token for map rendering.

## Project Structure
In the "App" directory of the project, we have several files dedicated to facilitating users in finding electric vehicle charging stations conveniently. "FilterCharger.html" enables users to filter charging stations based on their preferences, while its corresponding stylesheet "FilterChargerStyle.css" ensures a visually appealing interface. Similarly, "FindNearestCharger.html" assists users in locating the nearest charging stations, with its associated stylesheet "FindNearestChargerStyle.css" providing the necessary visual design. These files collectively form the user interface components of the application, streamlining the process of accessing electric vehicle charging infrastructure. Additionally, "Index.html" serves as a landing page, providing users with an entry point to the application.

```
└── 📁bignicker123.github.io
    └── 📁App
        └── Charging.jpeg
        └── FilterCharger.html
        └── FilterChargerStyle.css
        └── FindNearestCharger.html
        └── FindNearestChargerStyle.css
        └── Index.html
        └── IndexStyle.css
        └── ProvideDirections.html
        └── ProvideDirectionsStyle.css
    └── 📁docs
        └── 📁Images
            └── Context-diagram.png
            └── RobustnessDiagram.png
            └── UseCase-Diagram1.png
            └── wireflow3.png
            └── wireframeUC1.png
        └── deployment.md
        └── design.md
        └── implementation.md
        └── planning.md
        └── requirements.md
        └── testing.md
    └── readme.md
```
## Software Architecture

The architecture of this web application revolves around a client-server model, where the client-side interface, built with HTML, CSS, and JavaScript, interacts with the server-side Bristol Open Data API to fetch information about electric vehicle charging points. Utilising the Mapbox API, the application integrates interactive maps into the interface. JavaScript functions handle geolocation retrieval from the browser, enabling the user's location to be used for fetching nearby charging points and centring the map view. Upon receiving data from the API, further JavaScript functions process and sort the information, displaying relevant details such as charger name, location, type, socket type, and distance from the user. This architecture embodies a modular approach, with distinct components managing frontend rendering, data fetching, geolocation handling, data processing, and dynamic content updates.

### Component Diagram
![Component Diagram](Images/ComponentDiagram.png)

## Bristol Open Data API

`FindNearestCharger.hmtl` makes two requests to the Bristol Open Data API. First, in the `fetchChargerData()` function, it retrieves charging point data based on the user's location. Then, within `sortChargerDataByDistance()`, it calculates distances between each charger and the user, sorting and displaying the nearest ones. These queries ensure up-to-date information on nearby charging stations.

`FilterCharger.html` sends two requests to the Bristol Open Data API. Firstly, in the `fetchChargerData()` function, it retrieves charging point data based on the user's geolocation. Then, within `applyFilters()`, it filters the chargers based on user-defined criteria and displays the nearest ones on the map and in the table. These queries ensure that users receive accurate and relevant information about nearby charging stations.

### UML Diagram
One Location can have many Chargers.

![UML Diagram](Images/UMLUC1.png)

## Linting

This table shows the issues and solutions that occured during the implementation phase for this web app



