# DIABETIC PATIENT'S DATA ANALYSIS OF THE DATA FROM GLUCOSE MONITORS, ACTIVITY SENSORS, SLEEP SENSORS AND LOCATION MONITORS

CONTEXT OF THE PROJECT:
A type 1 diabetic patient uses a Continuous Glucose Monitoring (CGM) device to monitor the blood sugar and to keep track of the changes in the blood levels of the blood glucose levels. These CGM devices be used alone or in conjunction with digitally connected medical devices for the purpose of managing diabetes. One such digitally connected medical device is an automated insulin pump, typically called as automated insulin dosing (AID) systems.

It is logical to conclude that the amount of blood glucose are influenced by the amount to sugar consumed by the patient.
This project connects data from other health sensors to relate the influence of these parameters with the patient’s blood glucose. Co-relating blood glucose levels to multiple features can help in the holistic control of blood glucose levels for the patient. 

CONTENTS OF THE DATA:
	Raw data was collected from a type 1 diabetes patient who uses a CGM device for monitoring his blood glucose levels.
	Along with a CGM device, this patient also uses the following health monitors:
1.	A sleep monitoring device (Beddit) which records the features related to the patient’s sleep patterns
2.	An activity tracker
3.	A location monitor

DATA DICTIONARY:
1.	CGM data: Contained the blood glucose data (dependent variable) obtained from the CGM device. This device collects continuous data every 15 mins. This data set has 6839 instances with 4 features: 

-	Time: Contained the date time stamp of the event 
-	Record_Type: Contained data  about the type of the record.
o	Two types of record: 
	‘0’ means the machine automatically generates the blood glucose levels at the prefixed programmed time intervals 
	‘1’ means the blood glucose level is voluntarily measured by the patient.

-	Historic_ Glucose: Contained the data from the automatic measurements from the CGM device

-	Scan_Glucose: This feature contains the data from the voluntary measurements from the CGM device


2.	Beddit data: This data set contains data about the patient’s sleep pattern. It had 30 instances with 18 features. 

-	average_respiration_rate: Contained the data about the respiratory rate of the patient in breaths per minute

-	away_duration: Contained data about the amount of time (in seconds) the patient was out of the bed 	


-	beddit_user_id: Contained the device generated user ID	

-	date: Contained the date stamp of the event	


-	end_timestamp	id: Contained the time stamp about the end of the sleeping duration.	

-	resting_heart_rate: Contained data of the average heart rate of the patient during sleep and measured as beats/ minute

	
-	score_amount_of_sleep, score_awakenings, score_bed_exits, score_sleep_efficiency, score_sleep_latency, score_snoring :These features had empty instances (0 values)	
-	sleep_duration: Contained the total sleep time (in seconds)

-	start_timestamp: The time stamp of the sleeping cycle	


-	timezone: Contained the data about the time zone device works on ( here it works in “Berlin time” zone)	

-	updated: Contained the datetime stamp when the data was populated in the device	


-	wake_duration: Contained the time in seconds during which the patient was awake.

3.	Steps data: Contained the data about the patient’s activity profile. This dataset had 9  features and 31 instances.

-	active_time: Data about the the patient’s activity duration (seconds)
	
-	date: Contained the date of the event	


-	distance: Data about the user’s distance covered during the activity (meters)
	
-	id: Device generated reference IDs	


-	jawbone_user_id: Device generated reference IDs
	
-	steps: The count of the number of steps taken by the user to cover the specific distance 
-	steps_id: Device generated reference IDs	

-	timezone: “Berlin Zone”	


-	updated: date the data was saved to the device

INSPIRATION AND OBJECTIVES:
1.	To clean the raw data for analysis and derive insights from the data
2.	To create visualizations using the data using python and tableau to help generate insights and relation between the various features.
3.	To build a log reg model which can be used to decide which of these features has a better influence on the patient’s diabetic control apart from his diet.

Model application:
Packages used:
Pandas, numpy, matplotlib.pyplot, seaborn, scikit
Visualization of this was also done in “Tableau”
Acknowledgements:
Dmitri for sharing the data sets
