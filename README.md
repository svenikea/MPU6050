# MPU 6050 library for STM32

## Using STM32CubeMX and some Embedded Developement Tools 

### Windows
* STM32CubeMX you can download it [here](https://www.st.com/en/development-tools/stm32cubemx.html)
* And Keil C [here](http://www.keil.com/)
* STLink driver [here](https://www.st.com/en/development-tools/st-link-v2.html)
### Linux
* Get STM32CubeMX [here](https://www.st.com/en/development-tools/stm32cubemx.html)
* System Workbench for STM32 - SW4STM32 [here](https://www.openstm32.org/HomePage) (If you like Eclipse)
* Platformio [here](https://github.com/platformio/platformio-core) (Optional)
* STM32PIO [here](https://github.com/ussserrr/stm32pio) (Highly recommended if you're using Platformio)
* STLink driver [here](https://github.com/texane/stlink)
* You can also get all of these from arch based system with **AUR**
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
## HOW TO
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
