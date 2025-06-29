# Main Board Description
The Main Board is built around the STM32G4 Nucleo-32 (NUCLEO-G431KB) development board. It serves as the central controller for the Mach Probe Data Logger.

# Key functions:

Uses the STM32G431KBU6 MCU to interface with two I2C pressure sensors.

Connects to an IMU for detecting lift-off events and triggering high-speed logging.

Logs all flight data to an SD-NAND flash memory chip for reliable post-flight retrieval.

Provides USB or ST-Link connectivity for programming, configuration, and data download.

Includes power regulation (buck converter or LDO) to supply stable voltage from a single 18350 Li-ion battery.

# Features:

Compact design to fit within a 27 mm diameter nosecone module.

Rugged layout with strain relief to survive launch vibration and shock.

Always-on operation until battery depletion, with reliable performance from 0 – 85 °C.
