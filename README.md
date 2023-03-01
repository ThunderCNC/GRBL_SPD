<html>
<h1 align="center">GRBL_SPD</h1>
<h3 align="center">Router integration board for CNC (Currently for Makita 701C only)</h3>

<p align="center">
  <img height="300" src="https://github.com/ThunderCNC/GRBL_SPD/blob/main/images/MakitaGrbl_v3.png">
</p>
</br>
<div align="center">
<p align="center">Link to purchase kits</p>
<a href="https://www.tindie.com/stores/gingertesla/?ref=offsite_badges&utm_source=sellers_GingerTesla&utm_medium=badges&utm_campaign=badge_medium">
  <img src="https://d2ss6ovg47m0r5.cloudfront.net/badges/tindie-mediums.png" alt="I sell on Tindie" width="150" height="78">
</a>
</div>
</br>
<p align="center">Developed for use with, but not limited to the Arduino Uno board (Flashed with GRBL 1.1)</p>
</br>

<p> 
  <h2>Features for Makita 701C:</h2>
  <ul>
    <li>10,000 to 30,000 RPM</li>
    <li>On/Off control</li>
    <li>External manual controls</li>
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
<p><b><i>GRBL_SPD TO ROUTER:</i><b></br>  There are five connections inside the router. Three are to the the wires left when the router speed dial is removed and the other to connect to the relay. The cable/cables used for these connections should be shielded to help eliminate EMF. The relay breaks the power connection to the router and by leaving the connection to the factory switch makes for a fail safe. There is plenty of room inside the router housing for the relay to make thins neat.
</p>
</br>
<p><b><i>MANUAL CONTROL TO GRBL_SPD:</i><b></br> This feature has five connections as well. Three connect to an external potentiometer and two connect to a switch. At any point with the power on to the controller the switch will activate the router. When a file is being sent and a cut path is in progress, if needed you can turn on the switch to override the set RPM. To ensure there is no sudden drop or rise in RPM it will not override until the manual dial is within approx 2% of the set RPM. 
</p>
  
<h3>INSTALLATION</h3>
<a href="https://github.com/ThunderCNC/GRBL_SPD/blob/main/installation/ConnectionDiagram.pdf">Connection Diagram</a>
</html>
