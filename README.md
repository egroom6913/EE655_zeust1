IOT Application Readme

IOT.js is an application that supports registering new devices, displaying registered devices,        
receiving data from devices, and sending commands to devices. The system maintains logs of all activities            
and persist device information.

Usage

1. Extract the EE755_Assignment1.zip file to a working directory
2. Launch a cmd terminal and change directories to EE755_Assignment1 within the working directory
3. Open a web browser (Chrome, Microsoft Edge, etc) and open the IOT.html file
4. From the terminal command line type node iot to launch the IOT server application. The server app will run 
   on the localhost on port 3000
5. Enter the required information in the fields of the IOT.html page

The IOT application can be evalauted using the postman application using the following methods:
http://localhost:3000/register  (POST)
    requires: deviceID string
              deviceType string 
http://localhost:3000/data (POST)
    requires: deviceID string
              data string 
http://localhost:3000/command (POST)
    requires: deviceID string
              command string 
http://localhost:3000/show (POST)
    no parameters required
