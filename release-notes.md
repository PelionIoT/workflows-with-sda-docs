# Release notes

## Workflows with Secure Device Access v1.0.0

### Supported environment and versions
- IoT device: [ST DISCO-L475VG-IOT01A](https://os.mbed.com/platforms/ST-Discovery-L475E-IOT01A/)
- Device Management Client version: 4.2.1
- Mbed OS version: 5.15
- Mobile platform: Android
- Android OS version: Android Lollipop, 5.0 and higher
- Pelion Device Management (PDM) mobile app version: 1.0.2
- workflows-with-sda-client firmware version: 1.0.1

### Added
- Integrated Workflow Management Service (WMS) with Secure Device Access (SDA).
- Designed new UI/UX and implemented PDM mobile app in Kotlin.
- Integrated WMS APIs in PDM mobile app.
- Ability to operate the mobile app in offline mode.
- Ability to read and write files from remote IoT device.
- BLE interface between mobile app and IoT device.
- Handled fragementation of packets bigger than the BLE MTU size.
- BLE discover service uuid and service characteristics uuid are customizable.
- Supported max file size for read and write task is 1kB.
- Supported workflow task types `configure` and `read-data`.


### Known issues - PDM mobile app
- Identity providers other than *Native* not supported.
- *Forgot password* not supported.
- Two-factor authentication (2FA) not supported.
- If you enter an incorrect password more than five times, you have to reset the password using Device Management Portal.
- More than 50 devices in one workflow not supported.
- When try to read or write a file of size more than 2kB, sometimes the app goes into the state *Pelion DM isn't responding*.

### Out of scope
- Custom task types other than *configure* and *read-data*.
- Custom branding in mobile app is limited to landscape logo image.
- PDM mobile app for iOS platform.
- Encrypted link between PDM mobile app and IoT device.
- Firmware update of remote device.
