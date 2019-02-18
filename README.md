# NEST-With-Node-RED
This is a flow for dealing with NEST thermostats and Node-Red

This flow will make a periodic request to NEST via its API and convert the data as needed to MQTT and it will send an
email on abnormal events.

At this time it sends Temperature, Humidity and thermostat status to MQTT (other can be added if needed), it also checks for
an online/offline status of each device and it sends an email when the device status changes.
It also sends an email if the house transition from away to home, and if any thermostat sees a temperature below
a set limit.

Each block has a manual trigger for testing and a periodic one for normal quires of the API at NEST.

To use, you need to get an API key and code from NEST developer web page...
