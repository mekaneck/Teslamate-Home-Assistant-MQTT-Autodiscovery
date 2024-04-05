# Teslamate-Home-Assistant-MQTT-Autodiscovery
A Home Assistant Script to auto-discover MQTT topics populated by the Teslamate application

## Instructions: 
  1. Edit line 21 with your discovery prefix
  2. Add your vehicle on lines 27-33. If you have multiple cars, make
     additional list entries.
  3. Save file into your configuration.yaml, or if you use packages save it
     into the packages folder as a separate yaml file.
  4. In Home Assistant, go to developer tools > YAML and click SCRIPTS to reload
     them.
  5. In Home Assistant, go to 'automations' > 'scripts' and run 'Teslamate
     Entity Creator'.
     
#### (Optional:)
  6. Modify, add, or remove any sensor starting on line 51. All entries under
     the "config:" key are documented here:
     https://www.home-assistant.io/integrations/sensor.mqtt/#configuration-variables
     In order to pass a template, the brackets must be commented out. Use the
     following example as a reference:
     `value_template: "{{ '{{' }} value | float(0) * 1.234 {{ '}}' }}"`
  7. Create an automation to re-run this script whenever the software version
     sensor is updated. This ensures the correct software version is shown on
     the MQTT device page for each vehicle.

## References:
Take insipration from the Teslamate documentation regarding the types of sensors you can create:
https://docs.teslamate.org/docs/integrations/home_assistant/#mqtt_sensorsyaml-mqtt-section-of-configurationyaml
