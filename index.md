
## Projects Index

- [Automated Hydroponics Greenhouse Project](#automated-greenhouse-project)
- [Total Flatness Analysis of Optical Element](#total-flatness-analysis-of-optical-element)
- Servo Motors Control through Android Mobile App
- Other Small Projects
___
## Contact me!
<table>
  <tr>
    <td><a href="https://www.linkedin.com/in/samuel-costas-951894110/"><img src="https://drive.google.com/uc?export=view&id=1QA5wfyIx0F-cwll2CzRn5zFvO2czkHH5" alt="1" width= 80px></a></td>
    <td><a href="https://github.com/scostas54"><img src="https://drive.google.com/uc?export=view&id=1c6UzlFVSe5ZSTzDTRQ8dqv6RyNZvTVrx" alt="1" width= 80px></a></td>
    <td><a href="mailto:scostas54@gmail.com" target="_blank"><img src="https://drive.google.com/uc?export=view&id=1Kb9aYAu-mFuBCfIwlxredtIy8SFiuNDq" alt="1" width= 80px></a></td>
  </tr>
</table>

___
## Projects Overview

### [Automated Hydroponics Greenhouse Project](https://github.com/scostas54/Greenhouse_Project)

The purpose of this project is to develop an automated and easy-to-use hydroponic greenhouse. This greenhouse can be used in small apartments to grow fresh vegetables quickly and easily.

<table>
  <tr>
    <td><img src="https://drive.google.com/uc?export=view&id=1lckodjqgPnASNYDFuCkUAGjMT8MpJpJC" alt="1" width = 400px></td>    
   </tr> 
   <tr>
      <td><img src="https://drive.google.com/uc?export=view&id=1snk4FFNHdyghvBcBQ0uam_Zl-F82w67O" alt="3" width = 650px></td>
      <td><img src="https://drive.google.com/uc?export=view&id=1biuOsKzwus5In8cLqJbGgNJqkEDGb97-" align="left" alt="4" width = 650px></td>
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

Check the code in the Github Repository --> [Link to Repository](https://github.com/scostas54/Greenhouse_Project)
___
### [Total Flatness Analysis of Optical Element](https://github.com/scostas54/Optical-element-total-flatness-analysis)

This MATLAB program that I developed as my final project during my degree in mechanical engenieering, allows to determine the flatness of optical elements such as mirrors or reflectors. Starting from four phase distributions, it gives as a result the deviations with respect to an ideal plane for each surface.

Many of the different techniques that make up Optical Metrology provide information on the quantities being measured through phase differences encoded in turn in the form of spatial intensity variations, the so-called fringe patterns. The decoding process that provides the spatial distribution of the phase (phase map) using one or more of these fringe patterns is called "Phase Evaluation".

There are different phase evaluation methods, most of them assume a sinusoidal dependence between intensity and phase. In a series of these methods, the so-called Phase Shift Algorithms or PSAs are used as a tool to obtain the phase through an inverse trigonometric function whose argument is a combination of intensity values shifted in phase, obtained from one or various stripe patterns. (Sánchez, 2014)

In our case we use one of these algorithms, the so-called Schwider-Hariharan. It starts with five images, each is a pattern of stripes in which the phase is shifted 90º between each image.

<table>
  <tr>
    <td><img src="https://github.com/scostas54/Optical-element-total-flatness-analysis/blob/main/Original%20Images/AB90patron.jpg" alt="1" width = 600px></td> 
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
      <td><img src="https://github.com/scostas54/Optical-element-total-flatness-analysis/blob/main/Original%20Images/CAmapa.jpg"  alt="4" width = 600px></td>
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

```markdown
Syntax highlighted code block

# Resume Test 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and 

<img src="https://drive.google.com/uc?export=view&id=1lckodjqgPnASNYDFuCkUAGjMT8MpJpJC"
     alt="Markdown Monster icon"
     width="400"
     style="float: left; margin-right: 10px;" />

```
For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/scostas54/scostas54.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
