This project gives the latitudes and longitudes of the points from starting location to end location at a distance of 50m.

When someone hits API it goes directly to DirectionsController.java class. It first gets reponse from Google Maps API and then latitude and longitutde at every 50m .It uses haversine formula clubbed with section formula to get the results. 
DirectionService.java contains the core logic of the code.

I have created claases for every different object that I receive in Google Directions API response and all these classes are mentioned in Dto package.
Also Google Direction api gives distance in 2 units - feet, miles and I have a function DirectionsService.java which converts the distance based on units to meter.

This a maven based Java 8 project.

Sample Curl - curl --location --request GET 'http://localhost:8080/google/directions?origin=Disneyland&destination=Universal Studios Hollywood'
Response is too big to be mentioned here. Hence attaching the screenshot(SampleResponse.png) for the above start and end location.