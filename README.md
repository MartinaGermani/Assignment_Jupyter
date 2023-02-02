# Assignment_Jupyter
## Introduction
Starting from the third assignment of the RT1 course, I created a jupyter notebook to replace the user interface, which should allow to:
- autonomously reach a x,y coordinate inserted by the user,
- let the user manually drive the robot with the keyboard,
- let the user manually drive the robot using the keyboard but with some controls in order to avoid collision.

## How to run the code?
The main code is called 'JUPY_UI', where you can find the user interface with some buttons for handling the three different guide modalities, followed by different plots. This interface requires the following packages:
- 'final_assignment'
- 'slam_gmapping'

In order to visualize the guide simulation during the execution, you need to run:
- roslaunch final_assignment simulation_gmapping.launch
- roslaunch final_assignment move_base.launch

At this point you are ready for starting the guide, by simpling open jupyter notebook and run the 'JUPY_UI'.

## Description of the code
Through the use of this user interface, the user is able to switch between the following three guide modalities:
1. the first one is the 'Automatic Guide', where the user will set a target position and the robot will try to get the goal. Moreover, in this modality there is also the possibility of canceling the goal via the proper button
2. the second one is the 'Manual Guide', where the user can manually guide the robot in the desired position through the use of the keyboard. In particular, in this case it is expected a simple pad which allows to control the robot in space by simply clicking on the desired button
3. the third one is the 'Controlled Guide', which is structured as the second modality, but there are also some controls in order to avoid collisions.
