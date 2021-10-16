# Lab3: Interacting with memory mapped GPIO 

This lab is intended to be a recap of the of the lecture 3 to help better cement the ideas around C pointers and memory mapped I/O.
You can review the contents of lecture 3 [[here](https://github.com/STFleming/EmSys_GPIO_and_Abstraction_Costs)]. [[Lecture recording](https://swanseauniversity.zoom.us/rec/play/A8RBclaX4TlrNoBCyfGxA9FXxaHdIP6-GjN7PJHwRoL8x9hDiV-yap2nf_K5txCV9KRnI9IjlwD638LV.DTG_IWEC32C_jvtH?startTime=1634215328000)].

In this lab we are going to revisit the lecture and try and toggle GPIO pins as fast as we can. This lab will essentially follow the lecture quite closely and recap it's contents. 

_Note: there might be some slight differences between the measurements I got in the lecture and what you get, this is normal and we expect some variation_ 

## Task 1: digitalWrite()

In Arduino we can use the ``pinMode()`` function to set a pin to be an output, for example, ``pinMode(23, OUTPUT)`` sets pin 23 to be an output. Once set to be an output we can then use the ``digitalWrite()`` function to write a logical value to the pins, for example, ``digitalWrite(23, HIGH)`` to write a 1 (+5/3.3V), and ``digitialWrite(23, LOW)`` to write a 0 (0v).  

__Using these two function write a program that will toggle pin 18 on your tinyPico as fast as possible, what is the maximum frequency that you can achieve? Include a screenshot of pulseview in your logbook repository and commit it in__ ``lab3/task1``. 

## Task 2: digitalWrite() on multiple pins

__Using the__ ``pinMode()`` __and__ ``digitalWrite()`` __functions toggle pins 18,5,22,21,32,33 as fast as you can, what is the maximum frequency that you can achieve? Include a screenshot of pulseview in your logbook repository and commit it in__ ``lab3/task2``.

## Task 3: memory-mapped registers

As discussed in the lecture we can of course also use C pointers and memory mapped hardware registers to control our GPIO pins. 

__Using the GPIO memory-mapped hardware registers create a program that toggles pin 18, what is the maximum frequency that you can achieve now? Include a screenshot of pulseview in your logbook repository and commit it in__ ``lab3/task3``. 

## Task 4: memory-mapped registers multiple pins 

__Using the GPIO memory-mapped hardware registers create a program that toggles pins 18,5,22,21,32,33 what is the maximum frequency that you can achieve now? Include a screenshot of pulseview in your logbook repository and commit it in__ ``lab3/task4``. 


