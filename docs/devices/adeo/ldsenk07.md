---
title: "ADEO LDSENK07 Homebridge/HomeKit integration"
description: "Add HomeKit support to your ADEO LDSENK07, using Homebridge, Zigbee2MQTT and homebridge-z2m."
---
<!---
This file has been GENERATED using src/docgen/docgen.ts
DO NOT EDIT THIS FILE MANUALLY!
-->
# ADEO LDSENK07
> ENKI LEXMAN wireless smart outdoor siren


# Services and characteristics
The following HomeKit Services and Characteristics are exposed by
the ADEO LDSENK07

* [Battery](../../battery.md)
  * Battery Level
  * Charging State
  * Status Low Battery



## Exposes

```json
[
  {
    "type": "composite",
    "property": "warning",
    "name": "warning",
    "features": [
      {
        "type": "enum",
        "name": "mode",
        "property": "mode",
        "access": 2,
        "values": [
          "stop",
          "burglar",
          "fire",
          "emergency",
          "police_panic",
          "fire_panic",
          "emergency_panic"
        ],
        "description": "Mode of the warning (sound effect)"
      },
      {
        "type": "enum",
        "name": "level",
        "property": "level",
        "access": 2,
        "values": [
          "low",
          "medium",
          "high",
          "very_high"
        ],
        "description": "Sound level"
      },
      {
        "type": "enum",
        "name": "strobe_level",
        "property": "strobe_level",
        "access": 2,
        "values": [
          "low",
          "medium",
          "high",
          "very_high"
        ],
        "description": "Intensity of the strobe"
      },
      {
        "type": "binary",
        "name": "strobe",
        "property": "strobe",
        "access": 2,
        "value_on": true,
        "value_off": false,
        "description": "Turn on/off the strobe (light) during warning"
      },
      {
        "type": "numeric",
        "name": "strobe_duty_cycle",
        "property": "strobe_duty_cycle",
        "access": 2,
        "value_max": 10,
        "value_min": 0,
        "description": "Length of the flash cycle"
      },
      {
        "type": "numeric",
        "name": "duration",
        "property": "duration",
        "access": 2,
        "unit": "s",
        "description": "Duration in seconds of the alarm"
      }
    ]
  },
  {
    "type": "numeric",
    "name": "battery",
    "property": "battery",
    "access": 1,
    "unit": "%",
    "description": "Remaining battery in %",
    "value_min": 0,
    "value_max": 100
  },
  {
    "type": "binary",
    "name": "battery_low",
    "property": "battery_low",
    "access": 1,
    "value_on": true,
    "value_off": false,
    "description": "Indicates if the battery of this device is almost empty"
  },
  {
    "type": "binary",
    "name": "tamper",
    "property": "tamper",
    "access": 1,
    "value_on": true,
    "value_off": false,
    "description": "Indicates whether the device is tampered"
  },
  {
    "type": "numeric",
    "name": "linkquality",
    "property": "linkquality",
    "access": 1,
    "unit": "lqi",
    "description": "Link quality (signal strength)",
    "value_min": 0,
    "value_max": 255
  }
]
```

# Related
* [Other devices from ADEO](../index.md#adeo)
* [Zigbee2MQTT documentation for this device](https://www.zigbee2mqtt.io/devices/LDSENK07.html)