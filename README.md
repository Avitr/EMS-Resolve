# EMS-Resolve
To resolve the issues related to EMS for millions of people in India.
Software to track n number of Emergency vehicles in a region, using apps on there android phones and then distributing them all over the region to reduce the response time using GPS technology and tracking traffic and travel time data in real time through Google Maps.

Requirements For Fleet Management software

# Add comments or changes required if any right next to the Line in between these { ___ }.
 
1. PATIENT APP - P
2. DRIVER APP - Q

3. F.M.S.

#-

Sends and Recieves signal such as location, data to and from P & Q.
	
	a. Assigns unique code to each P & Q :- P -jkl & Q -xyz once it recieves data per new registration to identify each unit separately and stores it on a database.

	b. Recieves location data in real time/ Tracks Location of all the Q-xyz when the user logs in to app.

	c. Takes real time data using Google Maps API and divides a particular region into smaller grids on the basis of Distance, and primarily Max. Time to travel (ETA) in real time,
	   and identifies each grid edge as a G-abc.

	d. Searches for G-abc and Q- xyz in the database and Assigns a position to all the Q-xyz to the G-abc grids > Sends signal to Q-xyz to reach G-abc Location. 
	  d1 > Searches constantly for G-abc and Q-xyz in database and Repeats d.
	   d2 > If G-abc = 0 & Q-xyz =>0,then repeats d1 > If G-abc > 0 & Q-xyz>0, then repeats d. > If G-abc > 0 & Q-xyz = 0, then send signals for G-abc to the nearest G -xyz1 / Q-xyz1. 
	     
	e. Assigns a new unique code to both Q-xyz and G-abc as Q-xyz0 and G-xyz0 respectively.
	   > Checks the location of G-xyz0 and Q-xyz0 if found same assigns a new value to both as G-xyz1 and Q-xyz1.

	f. Can Recieve data sent from P-jkl, and analyse and track the location and then send it to the nearest Q-xyz1 on grid with the location, username, 
	   contact info to reach P-jkl to reduce the ETA. 
	> Recieves data from Q-xyz1 once it clicks to starts the responder trip,and assigns a new unique code to the Q-xyz1 once it is assigned a task as Q-wxyz1.
	> Recieves data from Q-wxyz1 once it reaches the P-xyz location and records the ETA for P-xyz and saves it on the database.
	> Recieves data from Q-wxyz1 once it reaches its destination Hospital, and reassigns Q-xyz as it's unique identity number and repeats d.

	g. Allows Admin or multiple users to log into the software and extract data from the system.

	h. Allows admin or multiple users to assign a P-jkl1 and manually enter Its Contact info, Name, Age, Address/Location(preferrably on Maps) etc., and send it to Q-xyz1 nearest on grid with the 
	   location, username, contact info to reach P-jkl to reduce the ETA. 
	> Recieves data from Q-xyz1 once it clicks to starts the responder trip,and assigns a new unique code to the Q-xyz1 once it is assigned a task as Q-wxyz1.
	> Recieves data from Q-wxyz1 once it reaches the P-xyz location and records the ETA for P-xyz and saves it on the database.
	> Recieves data from Q-wxyz1 once it reaches its destination Hospital, and reassigns Q-xyz as it's unique identity number and repeats d.

	i. Allows admin to create, delete, permit or edit other users and to restrict each unique user to use only a specific part.
