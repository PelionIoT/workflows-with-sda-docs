<h1 id="features">Using Portal to create WorkFlows and Setting Secure Device Access Policy</h1>

## Login to Portal
Login to portal using your Pelion Device Management credentials, Select your team in which you want to assign workflows and set secure access policies.


## How to create access policies?

1. If you are admin of this team then you will see option "Access Policies" in Access Management (Access Management -> Access Policies).
2. On Top Right Click on "+ New access policy" button which will open a form for creating New SDA policy.
3. You can edit default name and add description for SDA policy you are creating.
4. Select Selected Function and add "read-data" for giving read only and configure for write permission. 
<!-- Need to verify if token expires after x days then what happens ?-->
5. Token granted for : It's unit is in days so if you give for example 3 then it means this access policy will be valid for 3 days.
<!-- Endpoint Name works, and need to verify if giving Device ID works or not ?  -->
<!-- Please review below statement for endpoint name -->
6. Now, Select Endpoint name(s) / device Id(s) and enter the device endpoint name obtain during configuring device.
7. Select User / Group from dropdown to assign this access policy. 

## How to create Jobs?

1. Select Job Management -> Jobs from left panel.
2. Fill up New Job form with appropriate inputs.
3. Job Name: This name should be unique for a account and this name will be there in Job cell in mobile app in Jobs screen.
4. Description: Add Job description.
5. Location: Add City name in which job has to be performed.
6. Assign To: Select user from dropdown to which this job should be assigned.
7. Planned Start: This can be set for setting Job start date and time.
<!-- What happen if that filename is not there in device, how error case is handled ? -->
<!-- Need to verify the destination, please check if below statement is true or not -->
8. Tasks : Read - "fs/filename.txt" replace filename with file name you want to read from device. 
      <br> Write - Upload the file and give the path for example if filename is xyz.txt then destination will be "/fs/xyz.txt"
9. Add Device IDs or Endpoint names on which this job has to performed. Multiple deviceIDs/Endpoint Names can be added separated by newlines.     
10. Click on "Create Job" button, If disabled then check if you have added task or not.
           
