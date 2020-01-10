# Homebridge-Chamberlain
> Homebridge plugin for MyQ Garage Doors and Light Controllers
<img src='DemoVideo' />

[![npm](https://img.shields.io/npm/v/homebridge-chamberlain?style=for-the-badge)](https://www.npmjs.com/package/homebridge-chamberlain)
[![npm](https://img.shields.io/npm/dt/homebridge-chamberlain?style=for-the-badge)](https://www.npmjs.com/package/homebridge-chamberlain)


This plugin will allow you to control your MyQ garage door, and light controllers via HomeKit.

## Installation
Install homebridge ```Sudo Npm i -g HomeBridge```

Install this plugin ```Sudo Npm i -g HomeBridge-Chamberlain```

Add the config parameters to your ```config.json``` file. (Add Link)


# Configuration
Click here to learn to how find your device ID's. (Add Link)
> For one Garage Door
```json
{
  "accessory": "Chamberlain",
  "name": "Garage Door",
  "username": "your mychamberlain.com email",
  "password": "your mychamberlain.com password"
}
```
> For more than one Garage Door
```json
{
  "accessory": "Chamberlain",
  "name": "Main Garage Door",
  "username": "your mychamberlain.com email",
  "password": "your mychamberlain.com password",
  "deviceId": "xxx"
},
{
  "accessory": "Chamberlain",
  "name": "Side Garage Door",
  "username": "your mychamberlain.com email",
  "password": "your mychamberlain.com password",
  "deviceId": "xxx"
}
```


# Issues and Contribution

If you run into any issues, please be sure to check the common issues wiki, before opening an issue. (Add Link)

Also if you wish to contribute, submit a PR and I'd be more than happy to merge it in.


## Config extra's to work on:
# Config
Note: Run Homebridge with the deviceID's blank to generate the ID's.
If you get multiple ID's or it says it's invalid, use the one with CG.


If you have multiple garage doors, the plugin will throw an error and list the controllable device IDs. Use those IDs to create individual accessories. Be sure to uniquely name the door via the "name" field, otherwise you'll get a UUID error in the console (`Error: Cannot add a bridged Accessory with the same UUID as another bridged Accessory`).

,
...
```
