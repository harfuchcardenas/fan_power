The purpose of this repository is to enable the control of a 12V DC 0.12A fan using power electronics, with the
control logic managed by the Nordic nRF7002DK development kit. Additional technical details can be found in the
datasheet: https://www.nordicsemi.com/Products/Development-hardware/nRF7002-DK


The workflow of the project involves the following steps:
                                                          - power electronics, implementing the fan control
                                                          through an RTOS, over the nRF7002-DK to regulate the
                                                          fan speed in response to humidity levels captured by
                                                          the humidity sensors.

The motivation for this project comes from the high levels of hummidity in the developer's room.
stems from the need to address the high humidity levels in the developer's room.


The first step is to design the power electronics for a motor running on:

Voltage: 12
Current: 0.125
Power: 1.5
Or simply run the command Fan-details. Source code for this you can find it here.

Fan with electronics with control from a nRF-7002DK from nordic.
More info on the Datasheet pls visit: https://www.nordicsemi.com/Products/Development-hardware/nRF7002-DK

We'll start from the Power Electronics, then to the control over RTOS, the captured humidity we'll control the fan accordingly. 

REASON:
There is too much humidity in my room.
