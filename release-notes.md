# Release notes

## Workflows with Secure Device Access v1.1.0

### What's new:
- Added two-factor authentication (2FA) feature to the Android app.
- Added a Captcha challenge when you enter a wrong password more than five times in the Android app.
- Handled scenario in which the Android app went into **Pelion DM isn't responding** state for write tasks of more than 2kB.
- Performance improvements and fixes to credential management in Android app.
- Minor bug fixes in Device Management Portal related to deleting jobs and UI issues.
- Pelion Device Management (PDM) mobile app for Android version: 1.1.0.


## Workflows with Secure Device Access v1.0.0

### Supported environment and versions
- IoT device: [ST DISCO-L475VG-IOT01A](https://os.mbed.com/platforms/ST-Discovery-L475E-IOT01A/).
- Device Management Client version: 4.2.1.
- Mbed OS version: 5.15.
- Mobile platform: Android.
- Android OS version: Android Lollipop, 5.0 and higher.
- Pelion Device Management (PDM) mobile app for Android version: 1.0.1.
- workflows-with-sda-client firmware version: 1.0.1.

### Added
- Integrated Workflow Management Service (WMS) with Secure Device Access (SDA).
- Designed new UI/UX and implemented PDM mobile app for Android in Kotlin.
- Integrated WMS APIs in PDM mobile app for Android.
- Ability to operate the mobile app in offline mode.
- Ability to read and write files from remote IoT device.
- BLE interface between mobile app and IoT device.
- Handled fragmentation of packets bigger than the BLE MTU size.
- BLE discover service UUID and service characteristics UUID are customizable.
- Support for a max file size of 1kB for read and write tasks.
- Support for `configure` and `read-data` workflow task types.


### Known issues - Pelion Device Management mobile app for Android
- Identity providers other than *Native* not supported.
- *Forgot password* not supported.
- Two-factor authentication (2FA) not supported.
- If you enter an incorrect password more than five times, you have to reset the password using Device Management Portal.
- More than 50 devices in one workflow not supported.
- When the application tries to read or write a file of more than 2kB, it sometimes goes into the **Pelion DM isn't responding** state.
- When using the custom service UUID and service characteristics UUID, the application sometimes goes into the **Pelion DM keeps stopping** state.

### Known issues - Pelion Portal
- On the **New job** page, if you enter data in the description field and then delete it, it converts to a mandatory field.
- On the **New job** page, the **Assign to** field does not display the assignee's name.
- On the **Job details** page, error logs are not available for the failed read tasks.
- On the **Job details** page, jobs appear as **Unassigned** even when they are assigned.
- Inconsistent behavior when deleting jobs on the **Jobs** page.

### Out of scope
- Custom task types other than *configure* and *read-data*.
- Custom branding in mobile app is limited to landscape logo image.
- PDM mobile app for iOS platform.
- Encrypted link between PDM mobile app for Android and IoT device.
- Firmware update of remote device.
