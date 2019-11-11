# MPU 6050 library for STM32

## Using STM32CubeMX and some Embedded Developement Tools 

### Windows
* STM32CubeMX you can download it [here](https://drive.google.com/open?id=1N8bS0Hrovc6rC6EXCmpEYRuLo2L5LAkY)
* And Keil C [MDK-528A](https://drive.google.com/open?id=17sjN0DzB7I-pPuRy-l-LpnSjZ-4o4s-3)
* STLink driver [here](https://drive.google.com/open?id=1J7AiBV88Fnsd9TBRAAKmvBKSD9iBqoiu)
### Linux
* Get STM32CubeMX [here](https://drive.google.com/open?id=1ghoMddfOygAv4Riyuj9axoAC0LPkqIlH)
* System Workbench for STM32 - SW4STM32 [here](https://drive.google.com/open?id=16IZvkdUKKK0QfxI6qu8FygTKRyDq-17Q)
* STLink driver [here](https://github.com/texane/stlink)
## Installation
* First, you have to download the MPU6050.c and MPU6050.h file 
* Then Open Keil C or what ever your Embedded Developement tools peripheral 
* Add these 2 files to your project 
* Add these line to your code 
```c
/* USER CODE BEGIN Includes */
    #include "stdio.h"
    #include "MPU6050.h"
/* USER CODE END Includes */
```
```c
  /* USER CODE BEGIN 2 */
	char buf[4];
	MPU6050_init();
  /* USER CODE END 2 */
```
## HOWTO
```c
    MPU6050_init()
```
This piece of code will initialize the MPU6050
```c
    MPU6050_Read_Accel()
```
This will read the accelerator data from MPU6050
```c
    MPU6050_Read_Gyro()
```
This will read the accelerator data from MPU6050