# Release notes

## v1.0.0

### Environment and versions
- Supported IoT device: [ST DISCO-L475VG-IOT01A](https://os.mbed.com/platforms/ST-Discovery-L475E-IOT01A/)
- PDMC version: 4.2.1
- Mbed OS version: 5.15
- Supported mobile platform: Android
- Android OS version: Above Android 5.0, Lollipop
- Pelion DM App version: 1.0.0

### Added
- Integrated Workflow Management Service (WMS) with Secure Device Access (SDA).
- Designed new UI/UX and implemented PDM mobile app in Kotlin.
- Integrated WMS APIs in PDM mobile app.
- Added ability to operate the mobile app in offline mode.
- Ability to read and write files from remote IoT device.
- BLE interface between mobile and device.
- Developed a simple, less overhead fragementation protocol to handle packets more than BLE MTU size.

### Known Issues (PDM Mobile app)
<!-- How this will impact user and what will not work under which circumstances ? -->
- Identity providers other than *Native* is not supported.
- Forgot password, not supported.
- 2FA (Two factor authentication), not supported.
- If you enter incorrect password more than 5 times - you will have to reset it using Pelion Portal.
- More than 50 devices in one workflow is not supported.

### Known Issues (workflows-with-sda-client)
- Read and write max file size is 1.7kB.

### Out of scope
- Custom task types other than *configure* and *read-data*.
- Custom branding in mobile app is limited to landscape logo image.
- Mobile app for iOS platform.
- Encrypted link between mobile app and IoT device.
- Firmware update of remote device.