<html>
<h1 align="center">GRBL_SPD</h1>
<h3 align="center">Router integration board for CNC (Currently for Makita 701C only)</h3>

<p align="center">
  <img height="300" src="https://github.com/ThunderCNC/GRBL_SPD/blob/main/images/MakitaGrbl_v3.png">
</p>
<p>Developed for use with, but not limited to the Arduino Uno board (Flashed with GRBL 1.1) that is commonly used as a controller.</p>
<p> 
  <h2>Features for Makita 701C:</h2>
  <ul>
    <li>10,000 to 30,000 RPM</li>
    <li>On/Off control</li>
  </ul>
</p>


<h2>ABOUT THE GRBL_SPD</h2>
<p>
  This project allows for automatic control of a standard router for CNC machines. GRBL_SPD lets you set the rpm for your bits in software such as Vectric and have it automatically set your router. This cicuit replaces the potentiometer in the router and has an accuracy of approximately between +/- 100 to 200 RPM. In most cases this deviation has no impact on the machining process. You now don't have to turn on the router before sending the file, GRBL_SPD will do it for you. The enable pin on the controller was not needed to distinguish on/off states which leaves it available for the control of a dust collection system, lighting system or whatever necessary. There are inputs for manual control which overrides the RPM setting in the GRBL file being sent. 
</p>

<h3>CONNECTIONS</h3>
<p><b><i>CONTROLLER TO GRBL_SPD:</i></b></br>  Connections from the controller to the GRBL_SPD include power (5v), ground, and the PWM (0-5v) signal. Since both on/off and rpm are durived from the PWM pin, you must ensure in your post processor that S0 is included at the end of the file. Some grbl senders will automatically send S0 when M0 is sent, some will not so it's better to add it. Power and ground from the controller are self explanitory when using Arduino as they are clearly marked.
</p>
</br>
<p><b><i>GRBL_SPD TO ROUTER:</i><b></br>  
</p>
  
</html>
