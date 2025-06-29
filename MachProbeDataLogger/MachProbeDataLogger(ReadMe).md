# MachProbeDataLogger
This project documents the design and development of a custom PCB system for logging data from a Mach probe inside a rocket’s nosecone. It is part of my overall rocket sensor instrumentation work.
# Overview
The Mach Probe Data Logger is an embedded system designed to record pressure measurements from two sensors during a rocket flight. The system is optimized for small size, low power consumption, and reliable data storage to survive the entire flight profile, from launch through recovery.
# Function of the PCB
Collect and log pressure data from two I2C pressure sensors in real time.

Detect liftoff using an onboard IMU.

Store all measurements on local flash memory (SD-NAND) for later analysis.

Provide USB or ST-Link connectivity for configuration and data extraction.

Manage its own power via a dedicated battery with voltage regulation.

Essentially, this PCB acts as an autonomous black box for the nosecone, recording conditions to validate Mach number calculations and aerodynamic models.
# Main Task
Interface with two I2C pressure sensors in a confined cylindrical housing.

Sample and log data continuously until battery depletion.

Use an IMU to detect launch events and trigger high-speed logging.

Log data to NAND Flash memory reliably despite vibrations and shocks.

Provide easy access to logged data via USB or programmer interface.

Stay within strict mechanical constraints (diameter ~27 mm).
