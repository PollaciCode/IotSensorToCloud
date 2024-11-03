# IotSensorToCloud

This is a project to move sensor data from IoT devices to an azure cloud environment. From there, the data will be cleaned and put into proper pipelines. 
The Azure Cloud environment will eventually be linked to a local server to achieve a hybrid cloud model. 
At some point, I would like to have the data put into a visualization software, such as splunk, tableau, or some other equivalent. 

# Users: 
I have configured users in the AWS environment with the IAM system. Currently I have only 2 users, a read only user and an active admin user that is seperate from the root account. 

Permissions for these users have been configured so that the read only user can ONLY view all internal parts of the AWS Environment, while the admin can both edit and view all resources. 


# The IoT Device:
For the IoT device, I used several RaspberryPis with different sensors attached, such as temperature sensors. 
I then attached these devices to an AWS IoT Core with MQTT. I currently just did a single device setup with this. 
The Active message subscribed to and published from is "Hello World". 

It is planned to configure the remaining devices in bulk for scalability. 

I am working on updating the active topics to publish/subscribe to on both the IoT core and device sides. 

