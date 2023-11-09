# IARC 2022
Click on the below image to view the IARC 2022 Hardware round video
<!-- https://www.youtube.com/watch?v=Fl70FG0QKSU -->
<div align="left">
      <a href="https://drive.google.com/file/d/17pwk510tO8LMX1NhYVc4hkQPEKJ-GdMF/view?usp=sharing">
         <img src="\results\drone pic.jpeg" style="width:60%;">
      </a>
</div>


<img src="/results/iarc_mast.gif" width="30%" height="30%"/>  <img src="/results/iarc_mast_real.gif" width="30%" height="30%"/><br>
<img src="/results/replacement_ros.gif" width="60%"/>



## Broad Mission Logic - 
The Mothership takes off along with the daughtership in tow, and starts taking laps around the Pylon, using GPS Global Waypoint navigation. After the Laps are over, the Daughtership seperates from the Mothership, takes off, and starts looking for the Mast. It does so by moving around the mast, and using Machine Learning to detect the Mast Board. It then uses OpenCV to detect the LED Navigation lights, and then orients itself according to their position and orientation. After it has a good estimate of the mast board location, it approaches the module and starts the "coarse tuning" maneuver, which enables better controls of the end effector. Then, the "fine tuning" maneuver starts, which runs at a faster rate than the "coarse tuning maneuver", and that updates just the end-effector position according to the position of the module. Both of these maneuvers take the module location from the Machine Learning Module, and use PID Controllers to controls the actuators involved. Once the Module is aligned with the end-effector for a specified minimum amount of time, the end-effector executes the "replacement" maneuver, where it grabs the mast, removes the module, and then places another one in place of it. All this while, the Mothership is returning home. It started that as soon as the daughtership seperated from it. 
<br>
<br>
Click on the below image to view the IARC 2021 simulation round video
<!-- https://www.youtube.com/watch?v=Fl70FG0QKSU -->
<div align="left">
      <a href="https://www.youtube.com/watch?v=Fl70FG0QKSU">
         <img src="https://img.youtube.com/vi/Fl70FG0QKSU/0.jpg" style="width:60%;">
      </a>
</div>




