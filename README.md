# shelly-mqtt-2-influxdb

Read data from Shelly devices using MQTT, and ingesting that data to InfluxDB.

- Read from MQTT, write file to spool/ directory
- Read from spool/ directory, ingest data to InfluxDB

Manually clean files: find ./completed/ -name 'data-*-*.*' -type f -mtime +3 -delete


grab-mqtt-messages-solix: not Shelly related at all. Grab data from an Anker Solix. Getting the data from the solarbank is not part of this project. Have a look at https://github.com/tomquist/solix2mqtt, or something similar.