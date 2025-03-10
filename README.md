# Rep01LatinAmerica
primer repositorio de IEEE LatinAmerica
# esto es un comentario
# estos dueños seran los dueños por omisión para todo 
# en el repositorio. A menos que un match posterior tome precedencia.
# @global-owner1 y @global-owner2 serán los requeridos para
# revisar cuando alguien abra una solicitud de extracción
* @global-owner1 @global-owner2
* 
![PNGgraphicalAbstract](https://github.com/user-attachments/assets/4c56dcab-c2b6-4b98-9df1-238a5bfd49ab)

Resources and extra documentation for the manuscript "Replacing Missing Data in a Set of Historical Projects to Improve the Prediction of Software Effort" published in IEEE Latin America Transactions. The code is organized by the type of programming language used in the project in the following order MySQL -> R -> Excell. The project hierarchy and folders description is as follows:

MySQL\Using a  SQL-model to replace data in every atribute with missing data of a ISBSG set
MySQL/Models:
getRootDirectory.m. Script for loading current working directory.
startup.m. Script for adding all folder paths to MySQL.
SQL_models:
Breast. Breast models for A, B, and C-cup sizes.
Devices. Needle devices for core and fine needle biopsies.
Matlab_models. Scripts for robot modeling (forward and inverse kinematics), breast modeling, trajectory generation, a collision-free path algorithm and multiple simulation.
Data: Trajectory data for joint trajectory testing.
RoboticsToolbox:
ForApp. Function scripts for implementing the GUI application.
ForMatlab. Function scripts for all Matlab-based simulations.
ForSimulink. Functions script for all Simulink-based simulations.
ModernRobotics. Based on Modern robotics toolbox by Kevin Lynch and Frank Park.
rvctools. Robotics Toolbox for MATLAB or RVC by Peter Corke.
Test
Simulink_models. For implementing a robot-assisted biopsy environment based on Simscape and Stateflow-Flowcharts. Simulation settings: Ode23t Solver.
Data. .mat files for the GUI application, target biopsy points, breast holder models, Finite element breast models, breast dimensions, robot dimensions, robot kinematics, end effector waypoints and Simulink model workspace.
Extra. Figures for GUI application.
GUI. For designing a Graphical User Interface (GUI) for setting the basic configurations of a robot-assisted needle placement before a complete simulation (.mlapp).
Results. Outputs for multiple simulation (.xls files) and target biopsy points for each breast-cup size (.mat)
Scripts. For computing multiple simulations (.m) and biopsy targets samplings (.m) based on factorial-method design.
SIM. Simulation models (.slx) for GUI application and multiple simulation.
work. For simulation cache in Simulink.
R\SimulationAnalysis. For a statistical analysis and curves plotting.
ProjectImages. Some manuscript images, figures and animation for the README.m file.
Requirements
Matlab 2020b or later. All additional packages (only needed codes) were uploaded in this repository.
Robotics Toolbox for MATLAB or RVC from Robotics, Vision and Control Fundamental algorithms in MATLAB: Second Edition by Peter Corke.
Modern robotics toolbox from Modern Robotics: Mechanics, Planning, and Control (Kevin Lynch and Frank Park, Cambridge University Press 2017 and 2019).
Python 9.6
R 2.1 or later
Optional. Solidworks 2019 for CAD modeling and exporting files into Matlab
