# Teslamate-Home-Assistant-MQTT-Autodiscovery
A Home Assistant Script to auto-discover MQTT topics populated by the Teslamate application

## Instructions: 
  1. Edit variables on lines 20-24 per your own setup.
  2. Modify, add, or delete any sensors as necessary.
  3. Save file into your configuration.yaml, or if you use packages save it 
     into the packages folder as a separate yaml file.
  4. In Home Assistant, go to developer tools and reload scripts.
  5. In Home Assistant, go to scripts and run "Teslamate - Create Entities".
  6. (Optional) Create an automation to re-run the script every time the
     software version sensor has a state change. This will keep the software
     version shown in the device details in-sync with the actual version.   
