# Portfolio
Portfolio for CS304

This project instructs a small robot to perform several task at once while running the code provided in this repository on a microcontroller called an Arduino. Because of the controller's single threaded processor, I was forced to design the program for the robot in an unusual way. I treated the Arduino as a state machine, meaning that once one task was running on the thread I had to change the state of that task before I could begin another one. This unorthodox approach to programming brought on several challenges, such as having to organize my code in a more uniform fashion in order to keep track of what processes were running at certain times. If two tasks were being performed at the same time I would only see one executed by the robot, which made handling any run time errors fairly difficult. 
  Accompanying the Arduino are several other pieces of hardware that make the robot able to perform more intelligent operations. Two vital components,the motor controllers, are mounted towards the rear of the chassis. These simply do what their name suggests and control one of two motors using a analog signal. Next, the line follower array allows me to read a digital signal sent by the sensors which tells me where the robot is when it is following a line. If the robot starts to veer off in any direction, I can tell the controller to turn the motors in the opposite direction and the robot will be guided back on track autonomously. The 8-channel receiver and transmitter, an RC plane controller in our case, allow me to manually take control of the robot. The receiver sends a value in the form of an analog signal to the Arduino and, depending on the value, the motor controller tells the motors to turn forwards or backwards. To make handling the many errors I encountered easier I included a sixteen by two, sixteen being the number of characters per row and two being the number of rows, LCD display. After installing the LCD, I was able to print strings to it to tell me if any problems occured during run time. To power all of these peripherals I installed a 8.6 volt nickel metal hydride battery and designed a simple parallel circuit to ensure the power was equally distributed and no component received too much power. Finally, I included a switch to control when power was allowed to flow into the robot and so the battery did not have to be manually disconnected from the circuit. 
  From the time I started this project until the end, I was presented with many different problems. I plan to continue this project in my spare time and add several more features to make the robot more intelligent, such as voice recognition. This project as a whole has made me a much better programmer because it taught me to try and take a different approach when I am facing a hard situation. 

  
