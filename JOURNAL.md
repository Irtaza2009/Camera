---
title: "PiShot"
author: "Irtaza"
description: "A Raspberry Pi Zero 2W Camera with an LCD display, buttons, and a custom case!"
created_at: "2025-07-26"
---

### July 25th: Research + Wiring Diagram
The plan is to make a Camera with a custom 3d case (with a tripod, grip, and viewfinder), using the Raspberry Pi Zero 2W, and the Pi camera module 3, and the ST7789 LCD, that stores the photos on an SD card, and you can view the last photo (and explore all the shoots) on the display!! It will be in the Cyber-shot form factor!!

Started by looking up all the different Pi Camera modules and comparing their results! Settled on the Camera module 3, as it has auto focus! I will be using the Pi Zero 2W as the MCU, as it is the lowest-performance MCU that supports the camera. 
Then I made a list of all the components I would need! I decided to go with a 1500mAh 3.7V LiPo battery with an MT3608 boost converter, and a TP4056 module (with protection) to charge it! (At first, I was considering a power bank or an 18650 cell, but those are too bulky!)
For the display, I will be using the ST7789 TFT-LCD. And a metal momentary push button (similar to [this](https://www.adafruit.com/product/558), but without the LED ring!) for the shutter button! And I will also place an SPDT slide switch to turn it on and off!

I decided that I won't be using a PCB, so it's easier to place all the components in the case. So I will make a wiring diagram instead! Thus, I opened up [Cirkit Designer](https://app.cirkitdesigner.com/), and got to work!! [This](https://app.cirkitdesigner.com/project/cb34b867-8320-4c2c-972f-24cbd0726ab1) is what I came up with!

<img width="3000" height="2114" alt="circuit_image" src="https://github.com/user-attachments/assets/a3ad78c9-99e0-4964-ba3e-49aed0464589" />

**Total time spent: 3.5 hours**

### July 26th: Started 3d Case Design

I began by finding and downloading 3D models of all the components I would be using. This process took a significant amount of time, as I had to search extensively to locate every part! After that, I started designing the case in Shapr3D on my iPad. I first created a rectangular base for the body, including a removable back. Next, I added a square hole in the centre for the camera module, and a hole at the top for the shutter button. The challenging part was designing a grip that could slide into the case and be removed easily. Developing the sliding mechanism took quite a while, but I think it turned out pretty cool!

<img width="285" height="427" alt="image" src="https://github.com/user-attachments/assets/cd110c81-74df-4898-acd5-777e4fd10602" />
<img width="606" height="427" alt="image" src="https://github.com/user-attachments/assets/4ad3debe-dd22-40c2-8b97-52c015f95244" />

I began by placing each component into the interior of the case, ensuring that they were properly secured. I created holes on the sides and bottom for the SD card and the USB port of the Raspberry Pi. I also made an opening in the back cover for the LCD screen and added supports for all the components. However, I did not create a hole for the USB-C port, as I was still unsure about where to place it. 

<img width="520" height="385" alt="image" src="https://github.com/user-attachments/assets/99a0b39e-65e3-422b-8b96-b6b040019c25" />
<img width="474" height="385" alt="image" src="https://github.com/user-attachments/assets/f7afa6d4-ed17-4548-8d65-b04642f0acfe" />

<img width="520" height="425" alt="image" src="https://github.com/user-attachments/assets/ed7024ea-5300-4f40-8aba-95963028e34a" />
<img width="478" height="425" alt="image" src="https://github.com/user-attachments/assets/fc9df2a5-7879-43af-b704-9b1fc7ae334f" />

**Total time spent: 7 hours**
