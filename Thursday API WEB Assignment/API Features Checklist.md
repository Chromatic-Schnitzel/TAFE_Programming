## Pre-Submission Checklist
	Documenting REST API endpoints
- [x] 
	- [x] Tool 1
	- [x] Tool 2
	- [x] Tool 3
	- [x] Documentation Screenshots or export

	# PART FOUR Database Tasks
- [x] Configuration
	- [x] Screenshot of the configuration of a TTL Index
	- [x] Screenshots of Configuration File and Testing to demonstrating Persistence
	- [x] Trigger Details
	- [x] Trigger Email
	- [x] Trigger 1 code
	- [x] Trigger 1 Data Before Screenshot
	- [x] Trigger 1 Data After Screenshot
	- [x] Trigger 2 Code
	- [x] Trigger 2 Before Screenshot
	- [x] Trigger 2 After Screenshot
	- [x] Description of Database Authentication
	- [x] Screenshot of Configuring Database Authentication
	- [x] Screenshot of Successful Database Authentication
	- [x] Screenshot of Unsuccessful Database Authentication
	- [x] Description of Database Authorisation
	- [x] Screenshot of Configuring Database Authorisation
	- [x] Screenshot of Successful Database Authorisation
	- [x] Screenshot of Unsuccessful Database Authorisation
	- [x] Description of Data Encryption in place to meet project requirements
- [x] Partitioning
	- [x] Description of the selected Partition key and justification for this choice
	- [x] Screenshot/s demonstrating a collection partitioned using the selected key, including the collection name, number of chunks, shards and distribution spread
	- [x] Review of Partitioning and description of process to maintain distribution or optimise data

Endpoints:
- [x] GET Single
- [x] GET Multiple
- [x] POST Single
- [x] POST Multiple
- [x] PUT Single
- [x] PUT Multiple
- [x] DELETE Single
- [x] DELETE Multiple

Scenario Requirements/Endpoint Details:
- [x] Insert a new reading for a weather station
	To allow for the connection of new sensors to the dataset through this endpoint, will receive weather data and validate this data before inserting into the database.
- [x] Insert a new user
	Allow Administrators to create a new user account with a specified level of access
- [x] Insert multiple sensor readings for single station
	To allow for batch inserts every day, rather than one-by-one as the data is recorded
- [x] Find the maximum precipitation recorded in the last 5 Months for a specific sensor, returning the sensor name, reading date / time and the precipitation value
	To allow students to retrieve data that might provide insights into changes in weather patterns based on temperature fluctuations.
- [x] Find the temperature, atmospheric pressure, radiation, and precipitation recorded by a specific station at a given date and time
- [x] Find the maximum Temp(C) recorded for all stations for a given Date / Time range (start and finish date) returning the Sensor Name, reading date / time and the Temperature value
	To allow students to retrieve data that might provide insights into changes in weather patterns based on temperature fluctuations.
- [x] Create a query that includes an index key
	provide efficient querying by ensuring that an index is included for large or complex queries
- [x] Delete a user by Id
	Remove a single user account - revoking access to Authorised actions
- [x] Delete multiple users that have the ‘Student’ role and last logged in between two given dates
	Allow Administrators to remove a range of created user accounts based on a date range.
- [x] Update a specified entries’ precipitation value to a specific value
	To allow Admin users to correct errors in the dataset
- [x] Update access level for at least two users in the same query, based on a date range in which the users were created
	To Allow Administrators to upgrade or downgrade multiple users that were created in batches (upgrading or downgrading an entire group of students)

## Post-Submission Checklist
- [x] Post Weather
	- [x] Remove Student Role Permissions
	- [x] Add Sensor Role Permission
- [x] Update Precipitation
	- [x] Remove Student Role Permissions
- [x] Update User Role
	- [x] Remove Last Access field from DTO
- [x] Max Precipitation
	- [x] Return Value for only one sensor
	
- [x] Part 3, Task 2:
	- [x] 3.9 Authorisation Succeeding
		- [x] Add image of the User account associated with the apiKey to show assigned role
	- [x] 3.9 Authorisation Failed
		- [x] Add image of the User account associated with the apiKey to show assigned role
- [x] Part 3, Task 3:
	- [x] 3.11 Expected responses from the endpoint
		- [x] "Some of your endpoints in the documentation are missing some of their response codes such as the 401 & 403 for Api Key related issues, 400 for any endpoint that receives an input and 500 for any server related errors. Please update these."
	- [x] 3.12 Provided evidence of the documentation for each endpoint.
		- [x] "Once you have updated your endpoint documentation, please redo your PDF of the docs."
- [ ] Part 4, Task 1:
	- [ ] 4.2 MongoDB has been configured to accept persistence of objects including objects of different data types.
		- [ ] - Screenshots of the configuration file and options have been provided.
			- [ ] "This is a good start; can I also get you to add images showing your persistence is working. Refer to the class lesson plans for how to do this."
	- [ ] 4.3 In accordance with the scenario provided:
		- [ ] - At least two (2) triggers have been proposed and the corresponding events and notifications have been identified.
			- [ ] "Your 2nd trigger is not one specified by the scenario. Your log changes trigger should instead be a trigger that logs reading deletions. Please update this."
		- [ ] - Email to the manager or relevant stakeholder seeking confirmation of the triggers before implementing them has been provided as evidence.
			- [ ] "This will need to be updated to match your change of trigger."
	- [ ] 4.4  The triggers have been implemented and tested. Screenshots of code and of testing are provided for each trigger.
		- [ ] "Your images for the 2nd trigger will need to be updated once you change your trigger."
	- [ ] 4.5   Configured Authentication and Authorisation as per business requirements. Screenshots of the configuration process are provided, demonstrating the results of using both correct credentials and incorrect credentials.
		- [ ] "In the Successful authorization section. Can you please add 1 more image to the top of the section to show which login is being used for the create database test?"
- [ ] Part 5:
	- [ ] 5.1
		- [ ] "Please add some more details about what parts of the system/database you would check to see if they are the cause of the deletion."
	- [ ] 5.3
		- [ ] - Outlined the criteria that were used to partition a specific data store, and described the benefits achieved.
			- [ ] "Please add some more details to each section to explain the benefits of using these criteria for your key."
		- [ ] - Explained how sort keys can be used in a partition to increase performance, and outlined their functions and features in a NoSQL implementation.
			- [ ] "Please research what sort keys are in other systems and give me a brief explanation of them."
	- [ ] 5.4
		- [ ] "Add some more details to explain how the TTL works and what requirements need to be considered to set a TTL."
	- [ ] 5.6
		- [ ] Identified the debugging and testing methodology used and described four (4) techniques used to debug and test the API.
			- [ ] "Some of these answers are about the tools used, not the techniques."
			- [ ] "Please add some more details about the debugging techniques you employed when using Swagger, Response Codes and the Chrome developer tools and how useful the techniques were."
	- [ ] 5.8
		- [ ] - Numeric
			- [ ] "Please specify the specific data types allowed by the numeric field in Mongo Db"
		- [x] - Boolean
			- [x] "Please update this description to remove any mistake that you can actually set Yes/No as the values in this type. Just explain the type and what values it actually allows."
		- [ ] - Complex
			- [ ] "What other type of data can be stored in a complex type in mongo db."