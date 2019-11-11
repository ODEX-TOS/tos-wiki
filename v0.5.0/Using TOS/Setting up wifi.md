---
title: "Setting up wifi"
excerpt: ""
---
Starting up a network connection can happen in one of 2 ways on tos. The GUI and terminal will both be explained here.
[block:api-header]
{
  "type": "basic",
  "title": "GUI Connection to your wifi network"
}
[/block]
Connecting to a network should be pretty simple. This is why we provide an easy to use interface for connecting to wireless networks. All you have to do is open the action center (upper left side on the tos logo.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/6a6914c-Action-center-location.png",
        "Action-center-location.png",
        48,
        435,
        "#1c4c64"
      ]
    }
  ]
}
[/block]
Once opened up you should see the following.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b09d73b-action-center.png",
        "action-center.png",
        462,
        976,
        "#5b6063"
      ]
    }
  ]
}
[/block]
Press the connect to wireless network button to start the network connection wizard.
Select the desired SSID to connect to and optionally enter the password.
[block:callout]
{
  "type": "warning",
  "title": "Supported connections",
  "body": "We only support WEP/WPA and WPA2. Enterprise secured networks currently don't work with this option. You need to resort to the terminal to establish a network connection"
}
[/block]

[block:api-header]
{
  "title": "Terminal"
}
[/block]
This one is also pretty simple. All you need to know is your SSID and your password. Open up a terminal and type in the following
[block:code]
{
  "codes": [
    {
      "code": "tos network list # get a list of all detected networks\ntos network connect <ssid> # connect to a network called <ssid>",
      "language": "shell",
      "name": "bash"
    }
  ]
}
[/block]
If you are trying to connect to enterprise network or the connection type is not supported try the following
[block:code]
{
  "codes": [
    {
      "code": "nmtui # open a terminal user interface",
      "language": "shell",
      "name": "bash"
    }
  ]
}
[/block]