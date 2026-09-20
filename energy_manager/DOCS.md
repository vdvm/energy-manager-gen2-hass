# Energy Manager (Gen2)

Local daemon that curtails solar production when exporting electricity
costs money, maximizing self-consumption.

## Configuration

Fill in the configuration parameters in the Configuration tab:

- **Installation:** Timezone and coordinates.
- **Measurement:** P1 meter IP address and token.
- **Inverter:** Inverter Modbus TCP IP address and port.
- **Price:** Contract type, price components and energy source.
- **Outputs:** MQTT broker connection settings.

## Limits

The form and the app refuse values outside these limits, so a typo never
reaches the control loop:

- **Controller interval:** `1s` to `60s`, or `auto`.
- **Measurement stale after:** 1 to 59 seconds.
- **Recorder retention:** 1 to 3650 days.

A value the form cannot check (such as the controller interval) stops the
app at startup; the log names the option and the reason.
