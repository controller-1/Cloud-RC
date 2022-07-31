# Cloud-RC

The Cloud RC project is an endeavour to explore cloud computing and remote control of a small four wheeled vehicle. 

The motivation behind this project is purely for learning purposes. 

## How it Works:
The vehicle is controlled by an onboard ARM Cortex M4 microcontroller, which handles a multitude of tasks including monitoring and sampling of the infrared and photoelectric encoder sensors, processing sensor data, computation of a real-time PID control loop, control of four BLDC motors, servicing incoming/outgoing network messages, and the system status LED indicators. An RTOS is used, FreeRTOS, to manage and run all of these tasks concurrently. 

From the server side, a wifi module on the vehicle is used to establish a connection with the server. AWS cloud infrastructure services are used to implement the cloud computing and web hosted application to deliver commands to the vehicle. 


## Hardware:
- STM32F407G-DISC1
- [RC Chassis](https://www.amazon.com/perseids-Chassis-Encoder-Wheels-Battery/dp/B07DNXBFQN/ref=sr_1_53?crid=1V33CM1RM40A2&keywords=diy%2Brc%2Bcar&qid=1659301647&sprefix=diy%2Brc%2Bcar%2Caps%2C128&sr=8-53&th=1)
- [HC-020K Photoelectric Encoder Sensors](https://www.amazon.com/gp/product/B00EERJDY4/ref=ppx_yo_dt_b_asin_title_o03_s00?ie=UTF8&psc=1)
- [Motor Drivers](https://www.amazon.com/gp/product/B07BK1QL5T/ref=ppx_yo_dt_b_asin_title_o02_s00?ie=UTF8&psc=1)
- [IR Sensors](https://www.amazon.com/Infrared-Aideepen-Avoidance-Reflective-Photoelectric/dp/B09X39QZ45/ref=sr_1_4?crid=2IRMCLS5WV0Z3&keywords=infrared+sensors&qid=1659301925&sprefix=infrared+sensor%2Caps%2C146&sr=8-4)
- [ATWINC1500 WiFi Module](https://www.adafruit.com/product/2999)
- Miscell.: e.g., 9V batteries, mini breadboard, LEDs, etc.


