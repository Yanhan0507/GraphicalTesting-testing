# GraphicalTesting

It is the final project of Software Testing, which is a graduate course taught by Prof. Sarfraz Khurshid at UT Austin.
This course introduces the basics of software testing theory and practice, and then presents some recently
developed techniques for systematically finding bugs in programs and improving their reliability. 

This project will help developers to test their GUI. Given the software implementation, criteria(what is correct and what is wrong), and control singals, the system can out put the result. If everything goes well, it will return true, otherwise, it returns false, and highlight objects with wrong behaviors at each frame.

## Functionality description

There are mainly two parts of this project: driver and image processing part.

### Driver

Driver is designed to simulate the control signal, and these signals can be viewed as the input from player.
Also, driver will print all of the control signal in a text file, which can be utilized to check the correctness of UI in the future.

### Image processing
This part is using some computer vision methods to test the UI correctness at each frame.
Firstly, we need to get definition from game developers.
For example, in this project, I will test the TankWar game. The definitions are as below:
The red cycle, with radius of 25pixels, will be viewd as player's tank. The path of player's tank should correspond to the input of text file.
The black cycle, with radius of 25pixels, will be viewed as player's tank. It cannot keep still in the continous 6 frames.
The black rectangle, with size larger than 100*200 pixels, will be viewed wall. It should keep still all the time.

### Output

The project will output a boolean value which indicates the correctness of the project, and highlight the objects with wrong behaviors at each frame.
