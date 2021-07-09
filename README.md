# IoT
## IoT Access Control System

An extremely developer friendly platform for remote access system.

API: http://web.pi1.co/api/door/{userID}/{Appkey}/{TimeDelay}/{DoorID}/{Action}  
or   https://web.pi1.co/api/door/{userID}/{Appkey}/{TimeDelay}/{DoorID}/{Action}

TimeDelay: [1-10] (int) in seconds<br/>
DoorID: 1-6 (int)  1= Main Door, 2 = Room1, … 6= Room5
Action: 0,1 (int)    0:close, 1:open

A waiting period of **3** seconds is recommended.

Example:
To open main door, delay 3 seconds and then close door<br/>
https://web.pi1.co/api/door/{userID}/{Appkey}/3/1/1 

To open Room 3, delay 3 seconds and then close door<br/>
https://web.pi1.co/api/door/{userID}/{Appkey}/3/4/1

To close Room 3, delay will be ignored(No waiting time for close)<br/>
https://web.pi1.co/api/door/{userID}/{Appkey}/3/4/0

Any out of range parameter will result in an error.



