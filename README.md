# iSensor IMU Expansion Boards
## Introduction

This repository contains several expansion boards, FX3 pods, and miscellaneous circuit boards I've designed over the years to interface with ADI iSensor IMUs. All of these designs were validated at some point, but regardless, may have small issues (usually mechanical alignment)! 

### [48x, 49x Breakout Board](https://github.com/juchong/iSensor-Expansion-Boards/tree/main/48x_49x%20Breakout%20Board)

This board was designed as a smaller, more space-efficient replacement for the ADIS16IMU1/PCBZ board and provides similar functionality. All of the necessary signals are routed from the 24-pin, 1mm connector to the 16-pin, 2mm connector. 

<img src="docs/pictures/48x_49x_breakout.jpg" alt="ADXL_ADXRS Breakout Pod" style="zoom:50%;" />

A copy of the Rev C version of this PCB can be ordered from OshPark using this [link](https://oshpark.com/shared_projects/d1aorWWM).

### [ADXL_ADXRS Breakout Pod](https://github.com/juchong/iSensor-Expansion-Boards/tree/main/ADXL_ADXRS%20Breakout%20Pod)

This board was designed to interface with the EVAL-ADIS-FX3 (hence the "pod" nickname) and provides a generic interface for ADI accelerometers (ADXL-series devices) and gyroscopes (ADXRS-series devices) with a **digital** interface. 

<img src="docs/pictures/inertial_sensor_breakout.jpg" alt="ADXL_ADXRS Breakout Pod" style="zoom:50%;" />

A copy of the Rev A version of this PCB can be ordered from OshPark using this [link](https://oshpark.com/shared_projects/PcQ047B9).

### [FX3 Unit Test Loopback Pod](https://github.com/juchong/iSensor-Expansion-Boards/tree/main/FX3%20Unit%20Test%20Loopback%20Pod)

This board provides a compact and convenient way of verifying that the EVAL-ADIS-FX3 was manufactured correctly by looping back GPIO pins to each other. [This](https://github.com/juchong/EVAL-ADIS-FX3-Production-Test) repository contains additional software and documentation resources. 

<img src="docs/pictures/loopback_pod.jpg" alt="ADXL_ADXRS Breakout Pod" style="zoom:50%;" />

A copy of the Rev B version of this PCB can be ordered from OshPark using this [link](https://oshpark.com/shared_projects/FAYf9S82).

### [SPI Extender](https://github.com/juchong/iSensor-Expansion-Boards/tree/main/SPI%20Extender)

These boards provided an example for using LVDS transmitters and receivers to push SPI through a CAT6 Ethernet cable (twisted pair). Using these boards, we were able to reliably communicate with an ADI IMU through 25 feet of cable. 

### [iSensor Arduino Shield](https://github.com/juchong/iSensor-Expansion-Boards/tree/main/iSensor%20Arduino%20Shield)

This shield was developed as a reference design for easily interfacing an Arduino-compatible device with most iSensor evaluation boards. The shield includes a switching regulator that can be used to power the IMU instead of relying on the host system's 3.3V supply. 