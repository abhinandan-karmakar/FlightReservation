# FlightReservation

# Need to change the "application.properties" based on the DB configuration.

# Required the below tables to run this application.

Table Name : user
Structure:
ID	int	NO	PRI		auto_increment
FIRST_NAME	varchar(20)	YES			
LAST_NAME	varchar(20)	YES			
EMAIL	varchar(20)	YES	UNI		
PASSWORD	varchar(256)	YES	

Table Name : flight
Structure:
ID	int	NO	PRI		auto_increment
FLIGHT_NUMBER	varchar(20)	NO			
OPERATING_AIRLINES	varchar(20)	NO			
DEPARTURE_CITY	varchar(20)	NO			
ARRIVAL_CITY	varchar(20)	NO			
DATE_OF_DEPARTURE	date	NO			
ESTIMATED_DEPARTURE_TIME	timestamp	YES		CURRENT_TIMESTAMP	DEFAULT_GENERATED

Table Name: passenger
Structure:
ID	int	NO	PRI		auto_increment
FIRST_NAME	varchar(256)	YES			
LAST_NAME	varchar(256)	YES			
MIDDLE_NAME	varchar(256)	YES			
EMAIL	varchar(50)	YES			
PHONE	varchar(10)	YES			

Table Name: reservation
Structure:
ID	int	NO	PRI		auto_increment
CHECKED_IN	tinyint(1)	YES			
NUMBER_OF_BAGS	int	YES			
PASSENGER_ID	int	YES	MUL		
FLIGHT_ID	int	YES	MUL		
CREATED	timestamp	YES		CURRENT_TIMESTAMP	DEFAULT_GENERATED


# Overview of the project

# Launch Page
![image](https://github.com/abhinandan-karmakar/FlightReservation/assets/59645372/6864d73f-8fc1-4956-8fcc-d7c35f5adf5b)

# Login Page
![image](https://github.com/abhinandan-karmakar/FlightReservation/assets/59645372/8cadf7e0-0c03-4fda-bea2-d4a35ba2de22)

# Signup Page
![image](https://github.com/abhinandan-karmakar/FlightReservation/assets/59645372/939a2e48-37b6-483f-a787-d48f79eb0064)

# Flight Search Page
![image](https://github.com/abhinandan-karmakar/FlightReservation/assets/59645372/8938a30f-f685-438b-a283-2cbb33abee54)

# Show All Flights
![image](https://github.com/abhinandan-karmakar/FlightReservation/assets/59645372/71e2ebc8-0bfb-4be6-9c76-76a8378d4cc1)

# After select the flight this form will show to fill the passenger details
![image](https://github.com/abhinandan-karmakar/FlightReservation/assets/59645372/3ae54d59-8151-4341-b969-9d137e052f90)












