# Cordova WebBluetooth Plugin

This plugin provides rudimentary support for the [WebBluetooth API](https://webbluetoothcg.github.io/web-bluetooth/) via [Evothings BLE plugin](https://github.com/evothings/cordova-ble) & [BLEAT adapter library](https://github.com/thegecko/bleat).

*THIS REPO IS FORKED*

Cordova on Android already exposes window.navigator.bluetooth but when enabled in the Android permissions returns an error saying "Web Bluetooth is not available on this device...".

This fork removes the check for the existing window.navigator.bluetooth so that the _addAdapter helper function is added and the code doesn't error in Android.