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
