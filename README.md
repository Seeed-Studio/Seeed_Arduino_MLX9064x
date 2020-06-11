# Seeed Arduino MLX90640  [![Build Status](https://travis-ci.com/Seeed-Studio/Seeed_Arduino_MLX90640.svg?branch=master)](https://travis-ci.com/Seeed-Studio/Seeed_Arduino_MLX90640)

The inspiration for this product came from  [Melexis's mlx90640](https://github.com/melexis/mlx90640-library/) and [Melexis's mlx90641](https://github.com/melexis/mlx90641-library/).   This relies on the driver written by Melexis.

## Introduction

[Grove - Thermal Imaging Camera](https://www.seeedstudio.com/Grove-Thermal-Imaging-Camera-IR-Array-MLX90640-110-degree-p-4334.html) is a thermal sensor which carries MLX90640 IR Array. The camera can present dynamic thermal images and detect the surrounding temperature from -40℃~300℃. The camera with narrow-angle/wide-angle has an FOV(Field of View) of 55°x35°/110°x75°.

The IR thermal camera carries a 32x24 array of thermal sensors (MLX90640), it can detect the temperature of objects from feet away with the accuracy of ±1.5℃. In order to obtain the thermal image easily, I2C protocol is used to get the low-resolution image from the camera.

This module connects the MCU with the I2C interface. However, it needs an MCU which has over 20000 bytes of RAM to drive the camera. As a matter of fact, Dev board like Arduino Uno can not be used with this Sensor camera due to its lower ability of calculation. We recommend you to choose Arch Mix as an MCU to control the camera because it really has a good performance to process the complex data from the IR sensor camera.
![](https://raw.githubusercontent.com/SeeedDocument/IR-thermal-imaging-sensor-MLX90640-/master/114020142-previewbig.jpg)

## Note:
- **Visualization** The visual effect is as follows, you can use the following command to install his upper computer on the raspberry PI or PC
```
pip3 install seeed_python_ircamera

#PortName is like COM1,COM2 in Windows system.
#MLX90640 is an optional chip type , MLX90640 or MLX90641 can be supported for now.
ircamera PortName MLX90640
``` 

![](https://raw.githubusercontent.com/SeeedDocument/IR-thermal-imaging-sensor-MLX90640-/master/20191121_173909.gif)



_______________
This software is written by Baozhu baozhu.zuo@gmail.com for seeed studio
and is licensed under The MIT License. Check License.txt for more information.

Contributing to this software is warmly welcomed. You can do this basically by
forking, committing modifications and then pulling requests (follow the links above
for operating guide). Adding change log and your contact into file header is encouraged.
Thanks for your contribution.

Seeed Studio is an open hardware facilitation company based in Shenzhen, China.
Benefiting from local manufacture power and convenient global logistic system,
we integrate resources to serve new era of innovation. Seeed also works with
global distributors and partners to push open hardware movement.
