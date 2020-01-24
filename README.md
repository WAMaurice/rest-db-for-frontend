# rest-db-for-frontend
This is a test dataset for frontend developments.

## Description:
This respository holds a db.json file containing a set of example "car" and "bike" data.
The data can be called from the JSON REST server https://my-json-server.typicode.com/WAMaurice/rest-db-for-frontend and shall be used to
design a test frontend application.

*CAUTION: The REST server can also handle POST, PUT, PATCH and DELETE requests but it actually does NOT modify the data! When fetching data after a modification you will not see the changes!*

#### Car
The "status" of a car can be "FREE", "RESERVED", or "MAINTENANCE". These three states should be considered when designing the frontend.

Cars have a "last_tuv" field which stands for the last technical checkup appointment. If a car's "last_tuv" entry is older than 2 years
ago, then it should not be reservable and a warning should be displayed in the car details.

#### Bike
Bikes are a bit simpler than cars, the only important aspect is the "status", which can be "FREE", "RESERVED"
and "MAINTENANCE".
______________________
## Task:
Create a frontend application that has two different views:

1. A user view
2. An admin view

Both views shall retrieve the data from the REST server described above and display them in different ways.

#### User View
The user view shall show a map which displays all cars and bikes and their current status.
The objects should be clickable, showing the details.

#### Admin View
The admin view should be a dashboard listing all cars and bikes, clearly displaying the status of the objects.
Moreover, it shall be possible to view and edit each object in detail
__________________________
## Optional Tasks:

#### User View
Free objects shall have a "reserve" button to simulate the posibility to reserve.
The reserve button should send a REST command to the server modifying the appropiate dataset, by changing the "status" from "FREE" to "RESERVED".

#### Admin View
Cars and bikes shall be created and deleted.
____________________________
## Technical Requirements
There are no technical requirements. You may choose your prefered programming language & framework.
