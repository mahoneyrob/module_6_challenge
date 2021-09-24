#Purpose
The purpose of this project is to find destinations for a vacation.  

The first part, Weather_Database, picked 2000 random longitude and latitude pairs throughout the world, and then used a function from citipy to find the city closest to that coordinate.  I was able to get 740 random cities.  Then I called a openweathermap API to get the current weather for those cities.  Some were not found, and returned weather for 694 cities.  The data was then saved to a csv.

Next, in Vacation_Search, I narrowed down the number of cities based on user inputted temperature ranges.  Then did a search of hotels that are close to the cities found, and selected the hotel in the 0 index for each.  These were mapped with google maps, and had popups listing the city, country, hotel, and temperature of that location.  

Last, in Vacation_Itinerary, I selected 4 cities from the map that were in the same country, and ran a directions layer on the map.  