<html>
<h1 align="center">GRBL_SPD</h1>
<h3 align="center">Router integration board for CNC (Currently for Makita 701C only)</h3>

<p align="center">
<img height="300" src="https://github.com/ThunderCNC/GRBL_SPD/blob/main/images/MakitaGrbl_v3.png">
</p>
</html>
**Features for Makita 701C:**
  - 10,000 to 30,000 RPM
  - On/Off control

This project allows for automatic control of a standard router for CNC machines. It has been developed for use with, but not limited to the Arduino Uno board that is commonly used as a controller. Connections from the controller to the GRBL_SPD include power (5v), ground, and the PWM (0-5v) signal. The enable pin was not needed to distinguish on/off states which leaves it available for control of a dust collection system, lighting system or whatever necessary. 
