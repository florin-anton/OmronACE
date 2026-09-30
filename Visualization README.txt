This script allows you to enable simulation in Omron ACE 3.8.3.250, in this way you will be able to see how the robot handles Box type objects.

In order to use the script you must create a new folder under SmartController 1 having the exact name: Visualization Parameters.

After the folder was created right click on it and select Import Workspace File, select the file that you have downloaded from https://github.com/florin-anton/OmronACE (Visualization.awp) and select open.

All the objects that you want to manipulate must be of Box type and they should be present in the folder SmartController 1, the names of the objects should respect the format: Object_NameNumber, like for example Box1, Box2, Box3, etc. (the numbers should be consecutive numbers)

Inside the Visualization Parameters forlder you will find some varibles that should be set:

name: is the base name of the object (for example if you have the objects Box1, Box2, Box3, the base name is Box)
first: the number of the first object (for example if you have the objects Box1, Box2, Box3, the varible first is 1) 
last: the number of the last object (for example if you have the objects Box1, Box2, Box3, the varible last is 3)
grippers: the list of gripper that will interact with the objects, the list should end with ";", also ";" is used to separate the grippers in the list (for example: /SmartController 1/Gripper R1 Viper650;/SmartController 2/Gripper R1 Viper650;)
reset3D: this varible is used only when the script is running in order to place the objects in the initial position.

After setting the varibles: name, first, last, and grippers you can execute the Visualization script and execute the robot application. 

After executing the robot application, don't forget to reset the position of the objects by setting the value of the reset3D varible to 1.

Please see the following video tutorial for additional information:

 