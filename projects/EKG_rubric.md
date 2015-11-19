## Real-world challenge
This project aims at making heart-rate monitoring products more affordable for the public. Another goal of the project is to make such devices portable, since the current devices are large and can mostly be housed in hospitals or other health-care institutions. EKG devices in hospitals allow patients to monitor their heart rate for 10-15 minutes at max. However, heart failures don't happen during this time period. Making heart rate monitors that can give continuous feedback to the user would help immensely in better monitoring of heart related ailments.
This product could be especially benefitical to heart patients, but could also be of use to other people who perform physically intensive activities.

## Data / Materials
An ArduinoPro mini was used in conjunction with SparkFun's heart rate monitor to gather heart rate data of the team members. Currently, the data is stored into a computer using a USB drive that is connected to the Arduino.
The challenge in this method of data collection is that the recording is a series of electrovoltage changes. However, a heart beat is a much more complex phenomenon than just a time series of electrovoltage data. There are known to be atleast three waveforms constituting of a heart beat. Next steps in the data collection process is to figure out how can machines identify the intervals in heartbeats. Machine learning methods can be used here to train systems to calculate/glean the information of interest to the users.

## Approach
Python is used as the primary tool for data analysis in the project. The Arduino used in the project was also programmed using the Arduino programming language.

## Project Management
The first milestone of the project was to get the Arduino to start capturing heart rate information. The final goal is to be able to upload live heart rate information to a cellphone using Bluetooth technology. The data analysis of this data would be done in a smartphone in real-time.

## Other
At this stage, figuring out what kind of information is expected to be gleaned out of heart rate data is important. Setting a simple and straightforward expectation from the data would help in getting the final deliverable up and running in less time, and would give more time for testing and debugging of the application.
