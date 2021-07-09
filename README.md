# IoT
IoT Access Control System

API:
URL: http://web.pi1.co/api/door/{userID}/{Appkey}/{TimeDelay}/{DoorID}/{Action}    

TimeDelay: [1-10] (int) in seconds
DoorID: 1-6 (int)  1= Main Door, 2 = Room1, … 6= Room5
Action: 0,1 (int)    0:close, 1:open


Example:
To open main door, default delay 5 seconds and then close door
https://web.pi1.co/api/door/{userID}/{Appkey}/5/1/1 

To open Room 3, default delay 5 seconds and then close door
https://web.pi1.co/api/door/{userID}/{Appkey}/5/4/1

To close Room 3, delay will be ignored
https://web.pi1.co/api/door/{userID}/{Appkey}/5/4/0

Any out of range parameters will result in an error



