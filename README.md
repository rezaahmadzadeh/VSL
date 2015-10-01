# VSL
A Demo of Visuospatial Skill Learning (VSL) Approach



This source code is the implementation of the algorithm described in Chapter 4 of the book “Handling Uncertainty and Networked Structure in Robot Control”, Lucian Busoniu and Levente Tamas (eds.), Springer, 2015.

Author: Reza Ahmadzadeh, 2015
http://www.ahmadzadeh.info


This demo provides a very simple implementation of the Visuospatial Skill Learning approach. In this demo, the workspace contains four labelled objects. The robot has no a priori knowledge about the objects. The tutor demonstrates a pick-and-place action by picking an object and placing it near a landmark. The robot captures a set of observations and uses them to learn the spatial relationship between the object and its surroundings. Starting from a new initial configuration the robot can reproduce the skill by finding the object in the new workspace, picking it and placing it at the place demonstrated by the tutor. This way the robot can reach the goal of the task. Therefore, unlike many trajectory-based methods, VSL can be categorized as a goal-based approach that focuses on the goal of the task.

For more information, please refer to the corresponding chapter.




------------------------------------------------------------------
					Citation
------------------------------------------------------------------
This source code is given for free! However, I would be grateful if you refer to the book (or corresponding articles) in any academic publication that uses this code or part of it. Here are the corresponding BibTex references: 

	@inproceedings{ahmadzadeh2013interactive,
	  title={Interactive Robot Learning of Visuospatial Skills},
	  author={Ahmadzadeh, Seyed Reza and Kormushev, Petar and Caldwell, Darwin. G.},
	  booktitle={Advanced Robotics (ICAR) 2013, 16th International Conference on},
	  pages={1--8},
	  year={2013},
	  organization={IEEE}
	}

	@inproceedings{ahmadzadeh2013visuospatial,
	  title={Visuospatial Skill Learning for Object Reconfiguration Tasks},
	  author={Ahmadzadeh, Seyed Reza and Kormushev, Petar and Caldwell, Darwin G.},
	  booktitle={Intelligent Robots and Systems ({IROS}), 2013 {IEEE/RSJ} International Conference on},
	  pages={685--691},
	  year={2013},
	  organization={IEEE}
	}




------------------------------------------------------------------
					Getting started
------------------------------------------------------------------
    1- Unzip the archive into a directory of your choice.
    2- Start up Matlab, point it to the directory where you unzipped the file
    3- Run demonstration.m script to see the demonstration phase of the VSL approach. The comments in the demos should provide enough information for you to get started with using the demo. 
	4- after the demonstration phase is finished, Run the reproduction.m script to see the reproduction phase of the VSL approach. The comments in the demos should provide enough information for you to get started with using the demo. 
    5- The expected result of running both script are published in the html folder. 
    6- The image folder, includes the images captured during a real-world experiments.
    7- After the reproduction phase is finished a trajectory generation module can use the obtained pick and place coordinates to generate a trajectory. The trajectory can later be executed on a robot. 




------------------------------------------------------------------
					Software requirements
------------------------------------------------------------------
This demo requires MATLAB 7.13 (R2011b) or later, with the following toolboxes:

    - Computer Vision System Toolbox
    - Image processing Toolbox




------------------------------------------------------------------
					Contact
------------------------------------------------------------------
If you get stuck anywhere using the code, chance upon bugs or missing functions, or have any questions, comments, or suggestions, please contact me. I'll be glad to hear from you!

Reza Ahmadzadeh, September 2015
reza.ahmadzadeh@iit.it



------------------------------------------------------------------
					Final notes
------------------------------------------------------------------
This software is provided as-is, without any warranties. I have only tested the toolbox in Windows 7 and Ubuntu, but it should also work in other operating systems, with some possible minor issues due to, e.g., the use of backslashes in paths. The main algorithm and problem files are thoroughly commented, and should not be difficult to understand given some experience with Matlab. 
