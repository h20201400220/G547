GPIO pins or General-purpose Input Output pins are digital signal pins of the raspberry pi board which can be used as input pins, output pins or interrupt pins. The GPIO pins can be configured to act as desired using the GPIO hardware registers. In this project we have designed a GPIO device driver by controlling these hardware registers. Although the raspberry pi kernel has a GPIO device class, we will make our own device class and object to learn more about the actual hardware access. We have written a driver to toggle an LED connected to a GPIO pin. The period with which the LED toggles is modified using the user-mode application via the “sysfs” interface. The system uses the software timers available in the linux kernel to toggle the LED. 
