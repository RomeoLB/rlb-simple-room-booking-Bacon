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








