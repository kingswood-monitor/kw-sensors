# Sensors

This library provides a set of sensor drivers for a Kingswood Environment System 
environment sensor. Readings are encoded in a Protobuf format for transmission.

## usage

```
#include "sensors.h"

if (!init_sensors())
	Serial.prinln("Sensor initialisation failed");

uint8_t sensor_data[255];
uint8_t bytes_written = build_packet(packet_id++, sensor_data, 255);
```
