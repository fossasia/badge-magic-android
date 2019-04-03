# Badge Magic
[![Build Status](https://travis-ci.org/fossasia/badge-magic-android.svg?branch=development)](https://travis-ci.org/fossasia/badge-magic-android)
[![Gitter](https://img.shields.io/badge/chat-on%20gitter-ff006f.svg?style=flat-square)](https://gitter.im/fossasia/fossasia) [![Join the chat at https://gitter.im/fossasia/badge-magic](https://badges.gitter.im/fossasia/badge-magic.svg)](https://gitter.im/fossasia/badge-magic?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Badge Magic is an Android app to control LED name badges. The goal is to provide options to portray names, graphics and simple animations on LED badges. For the data transfer from the smartphone to the LED badge we use Bluetooth. The project is based on the work of [Nilhcem](https://github.com/Nilhcem).

## Download

* Download **[Badge Magic Dev Release here](https://github.com/fossasia/badge-magic-android/blob/apk/badge-magic-dev-release.apk)**
* Download Tested [LED Badge Version here](https://github.com/fossasia/badge-magic-android/blob/apk/LED-badge-dev.apk)

## Permissions
* Bluetooth: For sending data to the badge.
* GPS Location: This has been the standard set by Android for use with Bluetooth Low Energy (BLE) devices. For more information, please read the notes on [Android website](https://source.android.com/devices/bluetooth/ble).

## Communication

Please talk to us on the FOSSASIA [Gitter channel here](https://gitter.im/fossasia/fossasia).

## Reverse-Engineering Bluetooth LE Devices

Security in Bluetooth LE devices is optional, and many cheap products you can find on the market are not secured at all. This applies to our Bluetooth LED Badge. While this could lead to some privacy issues, this can also be a source of fun, especially when you want to use an LED Badge in a different way. It also makes it easy for us to get started with the development of a Free and Open Source Android app. 

As we understand how the Bluetooth LED badge works, converting a text to multiple byte arrays, we can send using the Bluetooth LE APIs. An indepth blog post about reverse-engineering the Bluetooth community [is here](http://nilhcem.com/iot/reverse-engineering-bluetooth-led-name-badge). 

The implementation in the Android app consists of manipulating bits. That may be tricky. A single bit error and nothing will work, plus it will be hard to debug. For those reasons, and since the specs are perfectly clear the reverse engineer Gautier Mechling strongly recommends to start writing unit tests before the code implementation. 

## Available Devices

There are a number of devices with Bluetooth on the market. As far as we can tell they are mostly from the same manufacturer. When you get a device ensure it comes with Bluetooth. There are devices that don't support Bluetooth. These are not supported in the app currently.
* Get one from [here](https://sg.pslab.io/product/led-badge/)

## User Interface

Here is a screenshot of the current image.
![Screenshot](./docs/images/badge-magic-screenshot.jpg)
