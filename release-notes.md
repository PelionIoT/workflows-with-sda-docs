<h1 id="features">Release Notes</h1>

## Environment and Version :
Device: Discovery board.<br>
PDMC version: 4.2.1<br>
Mbed OS version: 5.15<br>
Supported Mobile OS: Android<br>
Android OS version: Above Android 5.0, Lollipop.<br>
Pelion DM App version: 1.0.0<br>
Portal : required for SDA and creation of WorkFlows.<br>
File format : .txt (supported)<br>
FilePath: /fs/filename.txt <br>

## Known Issues (PDM Mobile App): 
<!-- How this will impact user and What will not work under which circumstances ? -->
1. Forgot password, not supported. 
2. 2FA (Two factor authentication), not supported.
3. If you enter incorrect password more than 5 times - you will have to reset it using the web portal.
4. Limitation - Not supported more that 50 devices in one workflow job.

## Known Issues (Firmware) :

1. A workflow job to read a file of size more than 200 bytes is not supported.
2. Write operation max limit - 1.7kb.