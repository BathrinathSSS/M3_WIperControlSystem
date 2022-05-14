# ABSTRACT :




A wiper is a necessary component that cleans raindrops or any other liquid off the vehicle's windscreen. The prior system required manual wiper activation,by changing the frequency As its results the operation of bringing up the wiper speed is varied . The project's goals are to improve ageing cars' systems by giving automated transmission.wiping system, to improve the system by incorporating a sensor and actuator, and to create a simple software that would completely operate with the system.the framework This proposed wiper system's principle is comparable to those of other existing conventional wipers. Despite the fact that,this system will be upgraded to an automatic control system using a Peripheral Interface to remove water from the windscreen.




# INTRODUCTION :


The operational speed of a wiper is controlled by a wiper speed control system in accordance with frequencies. The pulse signal is digitally processed to provide a control signal. A wiper driver circuit receives the control signal and adjusts the operational speed or timing in line with it.





# SOFTWARE USED : 

1) STM32 CUBE IDE


# COMPONENTS : 

1) STM32F4O7VG MICROCONTROLLER BOARD


# DESCRIPTION

# STM32F407VG :



The STM32F407 Kit takes advantage of the high-performance STM32F407 microcontrollers' capabilities to make it simple for users to create audio-based applications.It comes with an ST-LINK embedded debug tool, an ST-MEMS digital accelerometer, a digital microphone, an audio DAC with integrated class D speaker driver, LEDs, pushbuttons, and a USB OTG micro-AB connector.Ethernet connectivity, an LCD display, and other features have been added to the STM32F4 DISCOVERY kit. The STM32F405xx and STM32F407xx families are built around the high-performance Arm® Cortex®-M4 32-bit RISC core, which runs at up to 168 MHz.



# FEATURES OF STM32F407VG MICROCONTROLLER : 

* In a LQFP100 package, the STM32F407VGT6 microcontroller has a 32-bit ARM Cortex-M4 with FPU core, 1-Mbyte Flash memory, and 192-Kbyte RAM.

* On-board ST-LINK/V2 or ST-LINK/V2-A on STM32F4 DISCOVERY (old reference) or STM32F407G-DISC1 (new order code)

* USB ST-LINK with three separate interfaces and re-enumeration capability.

* Virtual Com port Debug port (with new order code only)

* Large-scale storage (with new order code only)

* Board power is supplied through USB or an external 5 V supply source.

* 3 V and 5 V external application power supply.



# USES OF STM32F407VG MICROCONTROLLER : 


* This Microcontroller is utilised in printing and scanning machines ,heat ventilation, air conditioning, and security systems.

* This module can be found in a variety of household products.







# OVERVIEW OF STM32F407VGT6 MICROCONTROLLER :


![image](https://user-images.githubusercontent.com/74197288/168224735-419f707c-4042-419e-a927-35ec715f4b1e.png)


* The STM32F407 Discovery board uses STM32F407VGT6 Microcontroller which has ARM Cortex-M4F Processor, which is capable of running upto 168Mhz. This MCU has many peripherals such as GPIO ports, TIMERS, ADCs, DACs, Flash Memory, SRAM, SPI, UART ect. The processor and peripherals talk via BUS-Interface. There are three busses available

* I-BUS (Instruction Bus) D-BUS (Data Bus) S-BUS (System Bus) I-BUS This bus connects the Instruction bus of the Cortex®-M4 with FPU(Floating point unit) core to the BusMatrix. This bus is used by the core to fetch instructions. The target of this bus is a memory containing code (internal Flash memory/SRAM or external memories through the FSMC/FMC).

* D-BUS This bus connects the databus of the Cortex®-M4 with FPU to the 64-Kbyte CCM data RAM to the BusMatrix. This bus is used by the core for literal load and debug access. The target of this bus is a memory containing code or data (internal Flash memory or external memories through the FSMC/FMC).

* S-BUS This bus connects the system bus of the Cortex®-M4 with FPU core to a BusMatrix. This bus is used to access data located in a peripheral or in SRAM. Instructions may also be fetched on this bus (less efficient than ICode). The targets of this bus are the internal SRAM1, SRAM2 and SRAM3, the AHB1 peripherals including the APB peripherals, the AHB2 peripherals and the external memories through the FSMC/FMC.

* So instructions and data use I-bus and D-bus respectively, All the other peripheral uses System bus. The Cortex-M4 processor contains three external Advanced High-performance Bus (AHB)-Lite bus interface and one Advanced Peripheral Bus (APB) interface. The GPIOs are connected to AHB1 bus which has a maximum speed of 150Mhz and is divided into two buses as APB1 and APB2. APB1 runs at 42Mhz(max) and APB2 runs at 82Mhz(max). The different peripherals such as SPI, UART, TIMERs, ADCs, DACs, etc are connected to either APB1/APB2 buses. And the AHB2(168Mhz max) is connected to Camera and USB OTG interfaces, AHB3 is connected to External memory controller.






# WORKING PRINCIPLE :
Assuming that the automobile is the microcontroller(STM32F407VG). If the button is pressed , the first led (red) will turn on, Clicking again the wiper will starts , and the second led (blue) will turn on for a desired rate. If the button is pressed again , the third led (green) will turn on, and the wiper's speed will be increased in comparison to the previous one. The fourth press will turn on the fourth led (orange) , and the wiper speed will be increased in accordance with the previous one. The microcontroller (vehicle) is turned off after the fifth click of the button.



# ENGINE_ON STATE : 





![ENGINE_ON STATE](https://user-images.githubusercontent.com/74197288/168262367-3097b9ae-ed68-4423-b25f-104a3c40cb95.png)



# WIPER STARTS & RUNS AT MODERATE SPEED : 



 

![WIPER STARTS   RUNS AT 70%(MEDIUM)](https://user-images.githubusercontent.com/74197288/168262575-bb0dd897-fcec-4b27-988d-0688288a9550.png)





# ENGINE_OFF STATE :






![ENGINE_OFF STATE](https://user-images.githubusercontent.com/74197288/168263299-aa56a1cd-a998-46f2-98f6-dcf8e25d2853.png)




