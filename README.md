# Data-Integration-and-Reshaping
Given multilple datasets in various formats and task is about creating a housing information dataset in Victoria, Australia.


Task 1: Data Integration

COLUMN	DESCRIPTION
	
ID	A unique id for the property
	
Address	The property address
	
1. Suburb (15/100)	The property suburb. The suburb must only be calculated using Vic_suburb_boundary.zip. Default value: “not available”
	
2. Price	The property price
	
3. Type	The type of property

4. Date	Date of sold
	
5. Rooms	Number of bedrooms
	
6. Bathroom	Number of bathrooms
	
7. Car	The number of parking space of the property
	
8. LandSize	The area of the property
	
9. Age	The age of the property at the time of selling
	
10. Latitude	The Latitude of the property
	
11. Longitude	The Longitude of the property
	
12. train_station_id (15/100)	The closest train station to the property that has a direct trip to the Southern Cross Railway Station. A direct trip is a trip where there are no connections (transfers) in the trip from the origin to the destination. Default value: -1

13. distance_to_train_station	The direct distance from the closest train station (identified above) to the property. Default value: -1

14. travel_min_to_CBD (15/100)	The average travel time (minutes) from the closest train station (regional/metropolitan) that has a direct trip to the “Southern  Cross  Railway  Station”  on  weekdays  (i.e. Monday-Friday) departing between 7 to 9:30 am. For
example, if there are 3 direct trips departing from the closest train station to the Southern Cross Railway Station on weekdays between 7-9:30 am and each takes 6, 7, and 8 minutes respectively, then the value of this column for the property should be (6+7+8)/3.). Default value: -1

15. over_priced? (4/100)	A boolean feature indicating whether or not the price of the property is higher than the median price of similar properties (with respect to bedrooms, bathrooms, parking_space, and property_type attributes) in the same suburb on the year of selling. Default value: -1

16. crime_A_average (3/100)	The average of type A crime in the local government area the property belongs to, in the three years prior to selling the property as the property. For example, if a property is sold in 2016, then you should calculate the average of the crime type A for 2013, 2014 and 2015. Default value: -1

17. crime_B_average (3/100)		The average of type B crime in the local government area the property belongs to, in the three years prior to selling the property as the property. For example, if a property is sold in 2016, then you should calculate the average of the crime type B for 2013, 2014 and 2015.Default value: -1
					
18. crime_C_average (3/100)		The average of type C crime in the local government area the property belongs to, in the three years prior to selling the property as the property. For example, if a property is sold in 2016, then you should calculate the average of the crime type C for 2013, 2014 and 2015. Default value: -1
					
19. closest_primary_school		The name of the closest primary school to the property. Default value: “not available” 

20. distance_to_closest_primary		The direct distance between the property and the closest primary school. Default value: -1

21. primary_school_ranking		The ranking of the closest primary school to the property as scraped from http://www.schoolcatchment.com.au/?p=12301  If the school is not listed, the value of this field should be set to “not ranked”. Default value: -1
					
22. closest_secondary_school		The name of the closest secondary school to the property. Default value: “not available”
					
23. distance_to_closest		The direct distance between the property and the closest
secondary secondary school. Default value: -1

24. secondary_school_ranking		The ranking of the closest secondary school to the property as scraped from
https://sites.google.com/a/monash.edu/secondary-school-ranking/   If the school is not listed, the value of this field should be set to “not ranked”. Default value: -1
					

	

	
