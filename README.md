# Aplication Note - Configuração da árvore de clock em tempo de execução em um STM32F103rb Nucleo

## Introduction

The STM32F103RB features a series of clocks intended for various functionalities organized in the clock tree. Its proper configuration is essential for the predictability and correctness of the program. This [Application note -  Configuração da árvore de clock em tempo de execução em um STM32F103rb Nucleo](https://github.com/pietrolzanetti/.pdf) aims to guide the initial configuration of the clock tree of an STM32F103RB through the STM32CubeMX graphic interface and the subsequent change of clock values during execution. To exemplify the concepts covered, an assembly was elaborated, in which the internal LED of the STM32 board flashes at various frequencies throughout the execution, as the GIF shown in the sequency.

![](AP_GIF.gif)

This AN was developed by Pietro Zanetti and Pedro Bahia as a work in the discipline of Embedded Systems Programming at UFMG - Prof. Ricardo de Oliveira Duarte - Department of Electronic Engineering.

The present code contains an example of using the theme covered in this AP.

## Hardware and software requirements
* STM32F103xb microntroller;
* PC;
* STM32CubeMX;
* SW4STM32 - System Workbench for STM32;
  
## Exemple reproduction
1. Conect STM32F103xb to your machine;
2. Open the project into Eclipse or equivalent;
3. Build and program chip.

## Functions in exemple
 ```C
 void makeItGoSlow(uint8_t div);
 ```
Change the division factor of the AHB clock.

Parameters:
  * ```div```: Correspondent bit of wanted division factor ;
 
 


