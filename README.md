# lelo-f1-web-client
LELO F1 SDK Web Bluetooth Client

The original and official repository with sample code for Android and iOS as well as BLE specifications can be found at [https://github.com/LELO-Devs/F1s-SDK](https://github.com/LELO-Devs/F1s-SDK).

This is an unofficial vanilla JavaScript  client based on the new Web Bluetooth API.

## WARNING: Work in progress! Currently developing on Chrome.

See the [Working demo](https://fabiofenoglio.github.io/lelo-f1-web-sdk/example.html)

# Available methods

All method return promises and can be chained.

- requestDevice -> returns list of devices responding to filter (name equals 'F1s')
- connect (device)
- searchAndConnect (shortcut for requestDevice chained with connect)
- disconnect
- waitForAuthorization

- getManufacturerName -> returns string
- getFirmwareRevision -> returns string
- getHardwareRevision -> returns string
- getModelNumber -> returns string
- getSoftwareRevision -> returns string
- getBatteryLevel -> returns integer
- getKeyState -> returns boolean
- getUseCount -> returns integer
- resetUseCount
- getButtonsStatus -> returns an object {plus: boolean, minus: boolean, central: boolean}
- getMotorsSpeed -> returns integers [motorSpeed, vibeSpeed]
- getMainMotorSpeed -> returns integer
- getVibratorSpeed -> returns integer
- setMotorsSpeed (motorSpeed, vibeSpeed) 
- setMainMotorSpeed (motorSpeed)
- setVibratorSpeed (vibeSpeed)
- shutdownMotors
