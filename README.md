![Logo](ecovacs-deebot.png)

# node-red-contrib-ecovacs-deebot
[![npm](http://img.shields.io/npm/v/node-red-contrib-ecovacs-deebot.svg)](https://www.npmjs.com/package/node-red-contrib-ecovacs-deebot)
[![npm](https://img.shields.io/npm/dm/node-red-contrib-ecovacs-deebot.svg)](https://www.npmjs.com/package/node-red-contrib-ecovacs-deebot)
[![npm](https://img.shields.io/npm/dt/node-red-contrib-ecovacs-deebot.svg)](https://www.npmjs.com/package/node-red-contrib-ecovacs-deebot)
[![Dependency Status](https://img.shields.io/david/mrbungle64/node-red-contrib-ecovacs-deebot.svg)](https://david-dm.org/mrbungle64/node-red-contrib-ecovacs-deebot)

Node-RED node for running Ecovacs Deebot vacuum cleaner robots

This node uses the [ecovacs-deebot.js](https://github.com/mrbungle64/ecovacs-deebot.js) library.

## Usage

### Ecovacs account

First you have to configure the Ecovacs account:
- "Email / Ecovacs ID"
- "Password"
- "Country code" (see [here](https://github.com/mrbungle64/node-red-contrib-ecovacs-deebot/wiki/Country-codes) for a list of country codes)

### Available nodes

#### Ecovacs Deebot

Available options: 
- Ecovacs "Account"
- "Name" of the Device
- "Device number"
- "Connect on startup"
- "Enable output of simple events"

#### Deebot command

Available options:
- "Command" (e.g. `Start automatic cleaning`, `Retrieve battery state`)
- Command specific fields (e.g. `Map ID`, `Spot area ID`)

## Models

### Supported models

* Deebot 900/901
* Deebot OZMO 930
* Deebot OZMO 920/950
* Deebot T9 series

### These models should work properly or at least partially

* Deebot Slim 2
* Deebot N79 series
* Deebot M88
* Deebot 600/601/605
* Deebot 710/711/711s
* Deebot OZMO 610
* Deebot OZMO 900/905
* Deebot OZMO Slim 10
* Deebot OZMO T5
* Deebot OZMO T8 series
* Deebot N3 MAX
* Deebot N7
* Deebot N8 series
* Deebot U2 series

## Known issues

* There's a strange behavior of the battery value on Deebot 900/901. It's very likely that this is a firmware bug
* Some cleaning commands may not work with Deebot 710/711/711s
* "Edge" command does not work with Deebot U2 (starts auto clean instead)

## Changelog

### 0.2.1
* Device number starts with 1

### 0.2.0
* Initial npm release
  * Added a lot of commands and events
  * Using library version 0.6.1-alpha.6
  * (unclej84) Added Multi-language support
  * (unclej84) A lot of improvements for the node editor
  * (unclej84) Use credentials for account data

## Disclaimer

We are in no way affiliated with ECOVACS.

## License

GNU GENERAL PUBLIC LICENSE

Copyright (c) 2021 Sascha Hölzel <mrb1232@posteo.de>
