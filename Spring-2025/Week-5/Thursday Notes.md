Thursday Notes:

On a high-level, we are going to program the STM32 to find where the peak of the rising pulse is (1.2V) and take that as the timestamp for the time.
We then compare the times between the hydrophones, and send it to the Raspberry PI.

In terms of timings, we have a rising peak of 10 microseconds. During that peak it will move from ~0V to 1.7V. We are taking a threshold at ~1.2V. 
There will be reflections after the pulse happens, so we will only measure after we have detected that there is a minimum voltage for 100ms (so that we know we are fully done with the last pulse).

In terms of technical implementation, we think we want to use i2C to communicate to the Raspberry PI synchronously. We are programming a STM32F767ZI using Stm32CubeIDE. We will be using C.


Full State Diagram

ROS2 State signaled to find direction to hydrophone

|
v

Raspberry PI signals to the STM32 that we are ready for a reading

|
v

STM32 Runs script to find the time differences (see above)

|
v

STM32 returns the time differences


|
v

Raspberry PI runs a script with the time differences to localize the vector (Pushed python code for this under Hydrophones git)

|
v

Raspberry PI has direction (yay!)
