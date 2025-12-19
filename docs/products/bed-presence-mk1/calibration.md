---
icon: lucide/rocket
---

# Calibration

The calibration process customizes the sensor thresholds to your bed.

## Automatic Sensor Calibration

The automatic calibration process requires you to get into and our of your bed. It records the sensor readings while the
bed is both occupied and unoccupied and automatically calculates the best trigger pressure.

1. Navigate to the device under Home Assistant Devices. Find the Configuration section.
1. Have the person you are calibrating for gently lay on their side of the bed.
1. Let the sensor settle for a few seconds and press Calibrate Occupied for the correct side of the bed.
1. Get out of bed.
1. Leave the entire bed unoccupied for a couple minutes, then press Calibrate Unoccupied for the correct side of the bed.
1. Repeat for the other side of the bed.
1. The goal of the automatic calibration is to get the trigger value to a good starting point. If you find that you are
getting false triggers, want to increase/decrease sensitivity, etc, continue to Manual Sensor Calibration.

## Manual Sensor Calibration

If you find that the automatic values don't work well, you can manually set the ==Trigger Pressure==. Viewing the graph of
the sensor pressure can help guide your desired pressure.

- If using only once sensor, you can set the value slightly higher than the “non occupied” pressure.
- If using both sensors, make sure to set it high enough that someone on the opposite side of the bed doesn’t trigger it.

