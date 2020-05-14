<h1 id="features">Using Pelion Device Management Application for WorkFlow Management</h1>

After you have installed Pelion Device Management Application, you can begin using its features. 

## Login Screen:
Sign In to mobile app using your Pelion Device Management Native credentials. 


## Select Account :
1. Choose the account/team from the list of accounts.

1. If you are associated with single team then Jobs screen will directly be opened.

## Jobs List Screen :

1. Jobs screen will fetch workflow jobs data from server and In Pending tab you can see Job listed which are assigned to you.

1. Each job requires to be performed on the device(s) will require secure access policy and also if job assigned to you is configure type then a file is also downloaded, so make sure you are connected to internet.

1. If you can see blue color icon on the right of the job cell then it means required data (token and file) are downloaded and you will be good to go and that job can also be executed even if you donot have internet connection.

1. If you see yellow color icon then it means token/file is not downloaded yet so wait for it to turn into blue icon, If you click on yellow icon cell then inside you will see option to file download / token download.

1. Each Job cell contain information like Job name, number of device, Secure Access valid date/time, and location.

1. Inside Completed tab you can see all the completed jobs you have executed.

## Job page :
1. If Secure Device access are valid i.e. SDA token is not expired (configured by admin from portal while setting SDA policy), then you can see information regarding job and SDA expiry date/time.

1. If SDA token is expired then status is expired and you can see refresh icon, on click of which it will try to renew the token again (this require internet connectivity).

## Job execution :
1. Job can be run either by clicking on Run Job button or swiping on particular device on which you want job to be executed.

1. If your Bluetooth is not turn on, then a popup with message "An app is asking to turn on Bluetooth" will come, click on Allow which will turn on bluetooth. Also, If your location are disabled, and you click on Run Job then a popup will open having information about why location service is required, as it needed for scanning nearby BLE devices.

1. If there is no device nearby, Then "No device found" status will be shown with Retry button to re scan nearby BLE devices.

## Settings :
1. User can change theme - Light and Dark.

1. Configure SDA Service - User can change ServiceUUID and Service-CharacteristicUUID as per your firmware configuration.

1. Help & Support - Customer help and support related to Pelion Device Management along with other informations like Third party libraries we use in app, and documentation.
