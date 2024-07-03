# A Priority-Based Multi-Robot Search Algorithm for Indoor Source Searching

## Source code

*The source code will be uploaded after the paper is accepted.*

Robot simulations were conducted using the [Gazebo](https://gazebosim.org/home) simulation environment on the [ROS](https://www.ros.org/) platform. The source search is performed by the [TurtleBot3](https://emanual.robotis.com/docs/en/platform/turtlebot3/overview/) Burger robot, equipped with a single-line lidar, MOX concentration sensor, and anemometer. The ROS version is [Noetic](https://wiki.ros.org/noetic).

1. Download the source code and put it in `~/catkin_ws/src`.
2. Run `catkin_make` in `~/catkin_ws`.
3. Run the launch file.

## Dataset

The dataset is designed for the task of multi-robot indoor source search. It builds upon our [previous research](https://github.com/mwanggh/An-Exploration-Enhanced-Search-Algorithm-for-Robot-Indoor-Source-Searching). Several new scenarios have been created and simulated. 

The case names are formatted as House$X_1$-$X_2$-$X_3$-$X_4$-$X_5 X_6$, where $ X_1 $ represents the house number, $ X_2 $ represents the airflow inlets, $ X_3 $ represents the airflow outlets, $ X_4 $ represents the airflow speed, $ X_5 $ represents the space where the source is located (B for Bathroom or K for Kitchen), and $ X_6 $ indicates whether the source is in the airflow (I for In or O for Out). For example, House07-1-3-04-KI signifies the scenario in House07 with airflow inlet 1, airflow outlet 3, airflow speed of 0.4 m/s, and a source located in the kitchen within the airflow. If $ X_4 $ is omitted, it implies the four cases for all airflow speeds.

- [CAD files.](https://huggingface.co/datasets/WangHaaa/SourceSearchingDatasetCAD) The 3D models were created by the [RobotAtVirtualHome](https://github.com/DavidFernandezChaves/RobotAtVirtualHome) project and converted into CAD models.
- [CFD data.](https://huggingface.co/datasets/WangHaaa/SourceSearchingDatasetCFD) CFD simulations were conducted using the [OpenFOAM](https://openfoam.org/) 11 software. The solver used is the simpleFOAM solver, and the model used is the $k-\epsilon$ model.
- [Source diffusion simulation data.](https://huggingface.co/datasets/WangHaaa/SourceSearchingDatasetGADEN) The diffusion of substances throughout the environment is simulated using [GADEN](https://github.com/MAPIRlab/gaden). You need to replace the absolute paths in the launch files with the paths of the corresponding files on your computer.

## Videos

*Coming soon!*

## Cite this paper

*Paper information will be updated after the paper is accepted.*
