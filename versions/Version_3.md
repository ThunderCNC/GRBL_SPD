<!DOCTYPE html>
<html lang="en">
<head>

</head>
<body> 
  <h1 align="center">GRBL_SPD v3 (Makita 701c)</h1>
  <div align="center">    
      <img width="80%" src="https://github.com/ThunderCNC/GRBL_SPD/blob/main/images/MakitaGrbl_v3.png">  
  </div></br>

  <div align="center">
  <p >Link to purchase kits</p>
  <a href="https://www.tindie.com/stores/gingertesla/?ref=offsite_badges&utm_source=sellers_GingerTesla&utm_medium=badges&utm_campaign=badge_medium">
    <img src="https://d2ss6ovg47m0r5.cloudfront.net/badges/tindie-mediums.png" alt="I sell on Tindie" width="150" height="78">
  </a>
  </div>




  <p> 
    <h2>Features for Makita 701C:</h2>
    <ul>
      <li>10,000 to 30,000 RPM</li>
      <li>On/Off control</li>
      <li>External manual controls</li>
    </ul>
  </p>


  
  <h2>CONNECTIONS</h2>
   <p><b><i>OPTIONAL CONNECTIONS:</i></b></br>  The three connections to control the RPM of the router and the PWM are neccessary. The potentiometer, switch and relay are not neccessary for function. It's up to you what you connect. 
  </p>
  <p><b><i>CONTROLLER TO GRBL_SPD:</i></b></br>  Connections from the controller to the GRBL_SPD include power (5v), ground, and the PWM (0-5v) signal. Since both on/off and rpm are durived from the PWM pin, you must ensure in your post processor that S0 is included at the end of the file. Some grbl senders will automatically send S0 when M5 is sent, some will not so it's better to add it. Power and ground from the controller are self explanitory when using Arduino as they are clearly marked.
  </p>
  
  <p><b><i>GRBL_SPD TO ROUTER:</i><b></br>  There are five connections inside the router. Three are to the the wires left when the router speed dial is removed and the other to connect to the relay. The cable/cables used for these connections should be shielded to help eliminate EMF. The relay breaks the power connection to the router and by leaving the connection to the factory switch makes for a fail safe. There is plenty of room inside the router housing for the relay to make things neat but it can be anywhere along the mains line.
  </p>
  
  <p><b><i>MANUAL CONTROL TO GRBL_SPD:</i><b></br> This feature has five connections as well. Three connect to an external potentiometer and two connect to a switch. At any point with the power on to the controller the switch will activate the router. When a file is being sent and a cut path is in progress, if needed you can turn on the switch to override the set RPM. To ensure there is no sudden drop or rise in RPM it will not override until the manual dial is within approx 2% of the set RPM. 
  </p>
    
  <h2>INSTALLATION</h2>
  <figure>
      <figcaption>Installation Diagrams:</figcaption>
      <ul>
        <li><a href="https://github.com/ThunderCNC/GRBL_SPD/blob/main/installation/ConnectionDiagram.pdf">Connection Diagram (Arduino Uno format)</a></li>
      </ul>
  </figure>
  <figure>
      <figcaption>STL files for manual control:</figcaption>
      <ul>
        <li><a href="https://github.com/ThunderCNC/GRBL_SPD/blob/main/stl/ManualMount.stl">Manual Control Mount (Millright MegaV)</a></li>
        <li><a href="https://github.com/ThunderCNC/GRBL_SPD/blob/main/stl/FillerMount.stl">Manuall Control Filler (For non-MegaV CNCs)</a></li>
      </ul>
  </figure>
  <p><b><i>CONTROLLER TO GRBL_SPD:</i></b>
    
  </p>
</body>
</html>
