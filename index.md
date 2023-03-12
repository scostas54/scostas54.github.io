
# Projects Index

- [PID Ball & Beam](#pid-ball-&-beam)
- [Automated Hydroponics Greenhouse Project](#automated-hydroponics-greenhouse-project)
- [Total Flatness Analysis of Optical Element](#total-flatness-analysis-of-optical-element)
- [Servo Motors Control through Android Mobile App](#servo-motors-control-through-android-mobile-app)
- [Other Small Projects](#other-small-projects)

___

# Contact me!
<table>
  <tr>
    <td><a href="https://www.linkedin.com/in/samuel-costas-951894110/"><img src="https://drive.google.com/uc?export=view&id=1QA5wfyIx0F-cwll2CzRn5zFvO2czkHH5" alt="1" width= 80px></a></td>
    <td><a href="https://github.com/scostas54"><img src="https://drive.google.com/uc?export=view&id=1c6UzlFVSe5ZSTzDTRQ8dqv6RyNZvTVrx" align="left" alt="1" width= 80px></a></td>
    <td><a href="mailto:scostas54@gmail.com" target="_blank"><img src="https://drive.google.com/uc?export=view&id=1Kb9aYAu-mFuBCfIwlxredtIy8SFiuNDq" align="left" alt="1" width= 80px></a></td>
  </tr>
</table>

___

# Projects Overview

## [PID Ball & Beam](https://github.com/scostas54/PID-Ball-Beam)

Dynamic systems are systems that change or evolve in time according to a fixed rule. A dynamic system is a system whose current state generates its successive state by a rule or principle of change (the so-called evolution rule) and thus produces a trajectory in a state space.

<a title="Sbyrnes321, CC0, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:QuantumHarmonicOscillatorAnimation.gif"><img width="256" alt="QuantumHarmonicOscillatorAnimation" src="https://upload.wikimedia.org/wikipedia/commons/9/90/QuantumHarmonicOscillatorAnimation.gif"></a>

In this system, te ball rolls on the beam without slipping under the action of the force of gravity. The beam is tilted from an external torque to control the position of the ball on the beam.

A PID controller has been implemented using an arduino nano. An IR sensor is used to measure the distance from the ball to the sensor (position), a servo motor applies an external torque to the beam and thus varies the angle and slope of the beam.

A PID controller continuously calculates an error value e(t) as the difference between a desired setpoint (SP) and a measured process variable (PV) and applies a correction based on proportional, integral, and derivative terms (denoted P, I, and D respectively), hence the name.

<a title="Arturo Urquizo, CC BY-SA 3.0 &lt;https://creativecommons.org/licenses/by-sa/3.0&gt;, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:PID.svg"><img width="512" alt="PID" src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2d/PID.svg/512px-PID.svg.png"></a>

An smartphone app has been developed in Adroid Studio (Java programming language) to establish the desired setpoint. The application opens a bluetooth socket that connect our smartphone with a HC05 bluetooth module connected to the aformentioned Arduino NANO.

The application consists of a simple GUI with a scroll bar, when used, the smartphone sends a integer through the previously established bluettoth communication.

[Click here or the image below to see the video](https://youtu.be/IA2fYVFnM1o)

<a href="https://youtu.be/IA2fYVFnM1o"><img src="https://i.ytimg.com/an_webp/IA2fYVFnM1o/mqdefault_6s.webp?du=3000&sqp=CNrAtKAG&rs=AOn4CLBUJrUQqyXa8eyyp4AMoruc1Cd0eA" width= 500px></a>

Check the code in the Github Repository --> [Link to Repository](https://github.com/scostas54/PID-Ball-Beam)

## [Automated Hydroponics Greenhouse Project](https://github.com/scostas54/Greenhouse_Project)

The purpose of this project is to develop an automated and easy-to-use hydroponic greenhouse. This greenhouse can be used in small apartments to grow fresh vegetables quickly and easily.

<table>
  <tr>
    <td><img src="https://drive.google.com/uc?export=view&id=1lckodjqgPnASNYDFuCkUAGjMT8MpJpJC" alt="1" width = 400px></td>    
    <td><img src="https://drive.google.com/uc?export=view&id=1snk4FFNHdyghvBcBQ0uam_Zl-F82w67O" align="top" alt="2" width = 650px></td>
   </tr> 
   <tr>      
    <td><img src="https://drive.google.com/uc?export=view&id=1biuOsKzwus5In8cLqJbGgNJqkEDGb97-" align="left" alt="3" width = 650px></td>
  </tr>
</table>

The system has many different sensors to monitor different parameters such as humidity, temperature, CO2...

The purpose is to act directly on these variables through the use of different devices such as fans, humidifiers and custom led panels. There is also a small water pump that moves the water continusiously to avoid the formation of biological sediments. These sensors are controlled with an **ESP32**, this microcontroller has integrated WIFI and the threshold of the sensors can be changed by means of an HTTP request through an Internet browser.

<table>
  <tr>
    <td><img src="https://drive.google.com/uc?export=view&id=1yMX5zxBrfOC6z4vaUgkRBVl2oivkjMTY" alt="1" width = 650px></td>
    <td><img src="https://drive.google.com/uc?export=view&id=18TXGzmk0s2qLfhLgw47s4Yce2X8LF-4_" alt="2" width = 650px></td>
   </tr> 
   <tr>
      <td><img src="https://drive.google.com/uc?export=view&id=1DvrTNQu4ngFWiFgICWopdQbHb2gpRxN0" alt="3" width = 650px></td>
      <td><img src="https://drive.google.com/uc?export=view&id=16OBgelQKbYxGcLZpz7pK6qSbLpl6Uc95" alt="4" width = 650px></td>
  </tr>
   <tr>
      <td><img src="https://drive.google.com/uc?export=view&id=1cW-UZmOjdvImH3ErONZnlas5ZIiO6nVH" alt="5" width = 650px></td>
   </tr>
</table>

The collection of data for a later analysis is also a purpose of this project, for this the ESP32 sends, through the WIFI network, the data collected by the sensors to a database in MariaDB through an Apache HTTP Server mounted on a Raspberry Pi.

<table>
  <tr>
    <td><img src="https://drive.google.com/uc?export=view&id=160c58ugWzSC6xJpzBJw35az3HxjUCl2s" alt="1" width=1000px></td>    
   </tr>   
   <tr>
    <td><img src="https://drive.google.com/uc?export=view&id=1qjNdEg7ob01mAKtG0ovI8ckvUat34HAT" alt="2" width=1000px></td>    
   </tr> 
</table>

Check the code in the Github Repository --> [Link to Repository](https://github.com/scostas54/Greenhouse_Project)


## [Total Flatness Analysis of Optical Element](https://github.com/scostas54/Optical-element-total-flatness-analysis)

This MATLAB program that I developed as my final project during my degree in mechanical engenieering, allows to determine the flatness of optical elements such as mirrors or reflectors. Starting from four phase distributions, it gives as a result the deviations with respect to an ideal plane for each surface.

Many of the different techniques that make up Optical Metrology provide information on the quantities being measured through phase differences encoded in turn in the form of spatial intensity variations, the so-called fringe patterns. The decoding process that provides the spatial distribution of the phase (phase map) using one or more of these fringe patterns is called "Phase Evaluation".

There are different phase evaluation methods, most of them assume a sinusoidal dependence between intensity and phase. In a series of these methods, the so-called Phase Shift Algorithms or PSAs are used as a tool to obtain the phase through an inverse trigonometric function whose argument is a combination of intensity values shifted in phase, obtained from one or various stripe patterns. (Sánchez, 2014)

In our case we use one of these algorithms, the so-called Schwider-Hariharan. It starts with five images, each is a pattern of stripes in which the phase is shifted 90º between each image.

<table>
  <tr>
    <td><img src="https://raw.githubusercontent.com/scostas54/Optical-element-total-flatness-analysis/main/Original%20Images/AB90patron.jpg" alt="1" width = 600px></td> 
    <td><img src="https://raw.githubusercontent.com/scostas54/Optical-element-total-flatness-analysis/main/Original%20Images/ABpatron.jpg" alt="2" width = 600px></td>
   </tr> 
   <tr>
      <td><img src="https://raw.githubusercontent.com/scostas54/Optical-element-total-flatness-analysis/main/Original%20Images/BCpatron.jpg" alt="3" width = 600px></td>
      <td><img src="https://raw.githubusercontent.com/scostas54/Optical-element-total-flatness-analysis/main/Original%20Images/CApatron.jpg"  alt="4" width = 600px></td>
  </tr>
</table>

The intensity values of those images (patterns) are combined and with the application of this PS algorithm the corresponding phase map is obtained.

<table>
  <tr>
    <td><img src="https://raw.githubusercontent.com/scostas54/Optical-element-total-flatness-analysis/main/Original%20Images/AB90mapa.jpg" alt="1" width = 600px></td> 
    <td><img src="https://raw.githubusercontent.com/scostas54/Optical-element-total-flatness-analysis/main/Original%20Images/ABmapa.jpg" alt="2" width = 600px></td>
   </tr> 
   <tr>
      <td><img src="https://raw.githubusercontent.com/scostas54/Optical-element-total-flatness-analysis/main/Original%20Images/BCmapa.jpg" alt="3" width = 600px></td>
      <td><img src="https://raw.githubusercontent.com/scostas54/Optical-element-total-flatness-analysis/main/Original%20Images/CAmapa.jpg"  alt="4" width = 600px></td>
  </tr>
</table>

The phase obtained with these methods, because we are using an arcotang function, appears in module 2π, in particular it takes values on the range between -π and π, which makes the neccesary to apply the process called unwrapping, in which the phase jumps are recomposed.

By applying unwrapping to the phase maps, a continuous phase is obtained.

<table>
  <tr>
    <td><img src="https://raw.githubusercontent.com/scostas54/Optical-element-total-flatness-analysis/main/4%20lambda%20unwrapped%20images/AB90.bmp" alt="1" width = 600px></td> 
    <td><img src="https://raw.githubusercontent.com/scostas54/Optical-element-total-flatness-analysis/main/4%20lambda%20unwrapped%20images/AB.bmp" alt="2" width = 600px></td>
   </tr> 
   <tr>
      <td><img src="https://raw.githubusercontent.com/scostas54/Optical-element-total-flatness-analysis/main/4%20lambda%20unwrapped%20images/BC.bmp" alt="3" width = 600px></td>
      <td><img src="https://raw.githubusercontent.com/scostas54/Optical-element-total-flatness-analysis/main/4%20lambda%20unwrapped%20images/CA.bmp"  alt="4" width = 600px></td>
  </tr>
</table>

That unwrapping process will keep a linear relationship with the magnitude to be measured (distance difference between both arms of the interferometer in our case), this allows us to work in Matlab using these maps as matrices. By applying the developed algorithm, the result is a 3D plot and matrix that contains the deviation from the reference plane for the mirror under test.

<table>
  <tr>
    <td><img src="https://raw.githubusercontent.com/scostas54/Optical-element-total-flatness-analysis/main/Result%20Graphs/4%20franjas%20A.JPG" alt="1" width = 600px></td> 
    <td><img src="https://raw.githubusercontent.com/scostas54/Optical-element-total-flatness-analysis/main/Result%20Graphs/4%20franjas%20B.JPG" alt="2" width = 600px></td>
   </tr> 
   <tr>
      <td><img src="https://raw.githubusercontent.com/scostas54/Optical-element-total-flatness-analysis/main/Result%20Graphs/4%20franjas%20C.JPG" alt="3" width = 600px></td>
  </tr>
</table>

Check the code in the Github Repository --> [Link to Repository](https://github.com/scostas54/Optical-element-total-flatness-analysis)

## [Servo Motors Control through Android Mobile App](https://github.com/scostas54/Servo-Motors-Control-Through-Android-Mobile-App)

This application allows the user to control 2 servomotors through an Android application developed in Adroid Studio (Java programming language). The application opens a bluetooth socket that allows us to connect our smartphone with a HC05 bluetooth module connected to an Arduino NANO.

The application consists of a simple GUI with two scroll bars, when moving these bars the smartphone sends two integers (it could be any other number or letter), one per scroll bar, through the previously established bluettoth communication.

To test the functionality, a simple mechanism was printed with my [Ender-3 3D](https://www.creality.com/en/goods-detail/ender-3-3d-printer). This mechanism has two degrees of freedom (yaw and roll), the angle of each axis is controlled by the scroll bars of the mobile app starting at 90º, an LCD screen is also used to show the current position of the servo motors (range from 0 to 180)

<table>
  <tr>
    <td><img src="https://drive.google.com/uc?export=view&id=1YLeX5v57HA1ZY0TJsweDnFQ0ZgBRMMIF" alt="1" width = 600px></td> 
    <td><img src="https://drive.google.com/uc?export=view&id=1md70AUWeVjVXqKm3HbD7ErXPqtdqvQJl" alt="2" width = 600px></td>
   </tr> 
</table>
<a href="https://www.youtube.com/watch?v=TeB_hDIixrQ&ab_channel=SamuelCostas"><img src="https://drive.google.com/uc?export=view&id=1FBWkYSVbCb_Z1fR5koE5kmyqB-L3u5mE" width= 800px></a>

## Other Small Projects

### [Garage Door](https://github.com/scostas54/Automation-of-a-garage-door-Spanish-)
This code can be used to atomate a garage door by using an arduino, some relays, an infrared sensor, some switches, pushbuttons and a remote control.

### [SPI Communication](https://github.com/scostas54/SPI-Communication-spanish-Comments)
This scripts can be used to transmit text information between two arduino boards through an SPI communication.
