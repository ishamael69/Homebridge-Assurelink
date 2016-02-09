
# Assurelink Plugin (modified form Liftmaster)

Installation
Install homebridge using: npm install -g homebridge
Install this plugin using: npm install -g homebridge-assurelink
Update your configuration file. See the sample below.

Configuration:

Example config.json:

    {
      "accessories": [
        {
          "accessory": "Assurelink",
          "name": "Garage Door",
          "username": "<your Assurelink email address>",
          "password": "<your Assurelink password>"
        }
      ]
    }

If you have multiple garage doors connected to your Assurelink account, the plugin will print out an error followed by the multiple device IDs it found. You'll need to use these IDs to enter your doors as separate accessories:

    {
      "accessories": [
        {
          "accessory": "Assurelink",
          "name": "Side Garage Door",
          "username": "<your Assurelink email address>",
          "password": "<your Assurelink password>",
          "deviceID": "<device ID>"
        }
      ]
    }
