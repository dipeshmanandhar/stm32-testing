# STM32 Testing

Testing using CAN with interrupts instead of polling.

The current configuration uses a periodic interrupt to send CAN messages and an edge-triggered interrupt to read CAN messages. Currently, this requires RTOS features of Mbed OS to be turned off (to use the CAN class in an ISR context).

There may be a workaround to this in the future if Mbed fixes an issue with the CAN class: [GitHub Issue](https://github.com/ARMmbed/mbed-os/issues/6714)
