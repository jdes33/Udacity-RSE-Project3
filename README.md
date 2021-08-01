# Udacity-RSE-Project3
This is the third project of the Udacity Robotics Software Engineer nanodegree.
The files in Project3 folder are what should be in the src folder of a catkin workspace.

## Outline of project
 - utilise pgm map creator to generate a map of gazebo world
 - use amcl (adaptive monte carlo localisation) node to localise robot in a known map
 - configure rviz to display map, robot, laser scan and particles using in amcl
 - allow robot to move either with teleoperation or ROS's move_base package


Here is an image of rviz when at the start before the robot starts moving. We can see the initial particle cloud as a bunch of purple arrows. Each arrow/particle is a guess for where the robot could be.
![Alt text](media/initial_particles.png?raw=true "Initial particle cloud.")

This is after the robot has been localised.
Here we can see that the particle cloud has converged after moving the robot a few steps.
![Alt text](media/final_localised_whole_map.png?raw=true "Particle cloud after a few steps.")
![Alt text](media/final_localised_zoomed.png?raw=true "Particle cloud after a few steps.")