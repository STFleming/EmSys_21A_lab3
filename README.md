# Lab3: Interacting with memory mapped GPIO 

This lab is intended to be a recap of the of the lecture 3 to help better cement the ideas around C pointers and memory mapped I/O.
You can review the contents of lecture 3 [[here](https://github.com/STFleming/EmSys_GPIO_and_Abstraction_Costs)]. [[Lecture recording](https://swanseauniversity.zoom.us/rec/play/A8RBclaX4TlrNoBCyfGxA9FXxaHdIP6-GjN7PJHwRoL8x9hDiV-yap2nf_K5txCV9KRnI9IjlwD638LV.DTG_IWEC32C_jvtH?startTime=1634215328000)].

In this lab we are going to revisit the lecture and try and toggle GPIO pins as fast as we can. This lab will essentially follow the lecture quite closely and recap it's contents. 

_Note: there might be some slight differences between the measurements I got in the lecture and what you get, this is normal and we expect some variation_ 

## Task 1: digitalWrite()

In Arduino we can use the ``pinMode()`` function to set a pin to be an output, for example, ``pinMode(23, OUTPUT)`` sets pin 23 to be an output. Once set to be an output we can then use the ``digitalWrite()`` function to write a logical value to the pins, for example, ``digitalWrite(23, HIGH)`` to write a 1 (+5/3.3V), and ``digitialWrite(23, LOW)`` to write a 0 (0v).  

__Using these two function write a program that will toggle a pin on your tinyPico as fast as possible, what is the maximum frequency that you can achieve? Include a screenshot in your logbook repository in__ ``lab3/task1``. 

## Task 2: digitalWrite() on multiple pins

__Using the__ ``pinMode()`` __and__ ``digitalWrite()`` __functions toggle 6 pins as fast as you can, what is the maximum frequency that you can achieve? Include a screenshot in your logbook repository in__ ``lab3/task2``.

