# rlb-simple-room-booking-Bacon
Use Brightsign player/device as a file server for a simple room booking application

Please see below for a video demo of how this application works:

[Download video](http://brightsignnetwork.com/download/Romeo/BS-Simple-Booking-room.MOV)

### Setup the Brightsign player as a File server for room booking

Unzip the content of the "Record-server" to a blank SD card

<img width="271" alt="image" src="https://github.com/user-attachments/assets/11085886-e353-46d7-b7cb-f20f54d46921" />

Adjust the Static IP address parameters to suit your network in the autorun.brs file:

<img width="529" alt="image" src="https://github.com/user-attachments/assets/327d98cf-4536-4957-b886-9b5205b9b062" />

Insert the SD card with the modified autorun.brs file and the nodeApp folder in the brightsign device that you would like to use as a file server (app tested on XT1145 with BOS/FW 9.0.168) and Power ON the Brightsign device.

In this example, I have configured my Brightsign device with an IP address of 192.168.1.106 which means that the /records-manager page should be accessible via "http://192.168.1.106:3000/records-manager"

<img width="969" alt="image" src="https://github.com/user-attachments/assets/a55f3d80-785d-4db5-acf6-c2b731995b19" />

Make sure to adjust the URL for accessing the /records-manager on your Brightsign device according to the static IP address that you have set in the previous steps

As per the Demo video, you should be able to add and remove records from the server by entering a new value in the text field and clicking "Add Record" next to the input text field or clicking the "Remove" button next to an existing record

<img width="743" alt="image" src="https://github.com/user-attachments/assets/380ae11b-2df4-44bc-9728-70b622370bda" />

### Publish BrightAuthor:Connected (BACon) presentation for room booking Application

In the Name-selector-app-BAcon folder, open the "booking-screen.html" file and change the value of the jsonUrl variable so it matches the IP address of your Local Brightsign server

<img width="773" alt="image" src="https://github.com/user-attachments/assets/014bd0dc-7255-4bd0-b732-5b93146befda" />

Launch BACon and open the "Room-booking-screen.bpfx" file and link all the files in the folder when prompted to do so by BACon.

Publish the presentation to a player that is connected to a touch screen or to one of the Brightsign built-in screen that are touch capable.

### How to select a new name/value from the Brightsign server and display it on another Brightsign device/player?

As per the video demo in this Readme file, leave your finger pressed down in the top right corner of the screen for 5+ seconds and this should display the dropdown menu with the latest version of the records/name list. Once the dropdown menu is displayed you should be able to select a new name/value to be displayed accross the screen.

Please note that the touch area that allows to display the dropdown list for name/value selection is only 200x200 pixels.

<img width="962" alt="image" src="https://github.com/user-attachments/assets/4c84cb74-170b-42da-b376-fb31266f40e7" />







