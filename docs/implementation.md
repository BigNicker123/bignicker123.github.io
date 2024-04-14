# Implementation

## Introduction
This web app utilises both the Mapbox API and Bristol Open Data API to pinpoint nearby electric vehicle charging stations. By leveraging the user's geolocation, it organises and presents charger details in a table format, featuring name, location, type, socket type, and distance. 

The dataset, obtained from the Bristol Open Data API, offers information on electric vehicle charging points, encompassing attributes such as name, location coordinates, charger type, and socket type. It is relatively small, containing only 26 rows. However, to streamline the user experience, various columns containing unnecessary information for the web app's purpose have been filtered out.

Configuration data includes the API endpoint URL for charger data retrieval and the Mapbox access token for map rendering.

## Project Structure
TODO: Provide an outline of the project folder structure and the role of each file within it.
provide a table listing the number of jslint warnings/reports for each module.

```
└── 📁bignicker123.github.io-main
    └── 📁App
        └── FilterCharger.html
        └── FindNearestCharger.html
        └── Main.html
        └── ProvideDirections.html
        └── style.css
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
TODO: Describe the major components of your architecture. Are any particular architectural styles being used?

![Insert your component Diagram here](images/component.png)

## Bristol Open Data API
TODO: Document each query to Bristol Open Data

![UML Class diagrams representing JSON query results](images/class1.png)
TODO: Repeat as necessary
