# homeassistant-paxcalima
Home assistant Custom component for  Pax Calima fan

This is offered AS IS.Feel free to fork. 

Installation
    Find out the MAC address and pin of your Pax Calima with calima -s. Pin code is in you fans motor unit. 
    Put __init__.py, sensor.py, manifest.json into <config>/custom_components/paxcalima/ on your home assistant installation (where <config> is the directory where your config file resides).
    Add the following to your configuration.yaml (or modify your sensor heading, if you already have one):

sensor:
  - platform: paxcalima
    mac: 00:11:22:AA:BB:CC # replace with MAC of your Pax Calima 
    pin: 57854677 # Replace with you pin code

Then restart Home Assistant and if everything works, you'll have some new sensors.
