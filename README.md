# ha-blueprints

## Automation

Repo for with home assistant blueprints 

### automation/robb-smarrt-8-switch-ROB_200-007-0.yaml

It’s a simple blueprint for ROBB SMARRT ZigBee Wall switch, that  maps all the available actions for all 8 buttons.
The available actions are:

- short press (each button)
- long press (each button)

This allows you to map any of the button (events) to any action you choose.
Should now also work for these types ROB_200_025_0, VES-ZB-WAL-012, SR-ZG9001K8-DIM

### automation/robb-smarrt-4-switch-ROB_200-008-0.yaml

Same as 8 button wall switch but for the 4 button variant

### automation/robb-smarrt-2-switch-ROB_200-009-0.yaml

Same as 8 button wall switch but for the 3 button variant

### automation/robb-smarrt-4-ch-remote-ROB_200-024-0.yaml

It’s a simple blueprint for ROBB SMARRT ZigBee Remote controller, that  maps all the available actions for all 5 vertical buttons.
The available actions are:

- short press (each button)
- long press (each button)

This allows you to map any of the button (events) to any action you choose.
Should now also work for this type: ZGRC-KEY-013
Now with debouncing thanks to @arnoudkooi

### automation/robb-smarrt-rgbw-remote-ROB_200-016-0.yaml

It’s a simple blueprint for ROBB SMARRT ZigBee RGBW Remote controller, that maps all the available actions for all 5 S buttons and enabling RGBW light to changes color per group (1-3)
This allows you to map any of the button (events) to any action you choose.


### automation/robb-smart-8-switch-ROBB-ROB_200-007-0.yaml
Old name keeping for installed base

## ESPHome_examples 

Repo with some ESPHome yaml examples i do use.. 

### ESPHome_examples/dim-led.yaml

Control a dimmable LED with a single on/off-switch used with a wall-mounted mains-switch controlling a relay as input and a MOSFET controlling the LED.
Switch off->on will fade the LED to its 100%, Switch on->off will fade the LED to its 0%.
If the switch is switched again during fading the LED will remain on the current  light level. With a short toggle, the light will dim to 0% or to the previous light level. (The yaml file contains a double implementation, so for 2 LED's with their own switch)      

### ESPHome_examples/garage-door.yaml

Open/close the garage door with HA, using a relay by-passing a push-button for manually opening. Feedback about the door position is done via an untra-sonic distance sensor mounted above the sliding door. 


