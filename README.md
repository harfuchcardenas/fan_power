The purpose of this repository is to enable the control of a 12V DC 0.12A fan using power electronics, with the
control logic managed by the Nordic nRF7002DK development kit. Additional technical details can be found in the
datasheet: https://www.nordicsemi.com/Products/Development-hardware/nRF7002-DK To this same board is to be a humidity sensor to be read with a semaphore of RTOS every 1s for 2 seconds (10 samples), then make the average and finally send it over UART (serial) to be possible to see the values on the terminal of my computer. I am running on Linux Ubuntu as Not possible with fedora because of memory errors. Any additionals or modifications are welcomed.


The workflow of the project involves the following steps:
                                                          - power electronics, implementing the fan control
                                                          through an RTOS, over the nRF7002-DK to regulate the
                                                          fan speed in response to humidity levels captured by
                                                          the humidity sensors.

The motivation for this project comes from the high levels of hummidity in the developer's room.
stems from the need to address the high humidity levels in the developer's room.


The first step is to design the power electronics for a motor running on:

Voltage: 12 V
Current: 0.125 mA
Power: 1.5 W

Or simply run the command Fan-details. Source code for this you can find it here.

Fan with electronics with control from a nRF-7002DK from nordic.
More info on the Datasheet pls visit: https://www.nordicsemi.com/Products/Development-hardware/nRF7002-DK

We'll start from the Power Electronics, then to the control over RTOS, the captured humidity we'll control the fan accordingly. 

REASON:
There is too much humidity in my room.

Next section is about the PCB design which has been generated with open source tools and the Documentation from Texas Instruments(please visit: www.ti.com

![Circuit_design_with_ULN2003A](https://github.com/user-attachments/assets/2cda7798-3130-4098-83a7-d7947cc95b55)

Figure 1: Connections between ULN2003A (Darlington Bridge created by Texas Instruments)
