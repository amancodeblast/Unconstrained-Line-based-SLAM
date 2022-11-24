# ENPM667: Controls Mid-Term Project - SLAM

Anukriti Singh - 119288306, Aman Sharma - 119085431


## Submission Files
* [Mid Term Project Report](https://github.com/amancodeblast/Unconstrained-Line-based-SLAM/blob/master/667_Midterm_UVSLAM.pptx)
* [PPT Presentation](https://github.com/amancodeblast/Unconstrained-Line-based-SLAM/blob/master/667_Midterm_UVSLAM.pptx) 
* [Results](https://github.com/amancodeblast/Unconstrained-Line-based-SLAM/blob/master/667_Midterm_UVSLAM.pptx)
* [Original Paper](https://github.com/amancodeblast/Unconstrained-Line-based-SLAM/blob/master/667_Midterm_UVSLAM.pptx)
## Results 
![Result1](/output/result1.png)
![Result2](/output/result2.png)
![Result3](/output/result3.png)
![Result4](/output/result4.png)

## Installation
### 1. Requirements and Prerequisites
-  Ubuntu 18.04
- [ROS melodic](http://wiki.ros.org/ROS/Installation)
- OpenCV 3.2.0 (under 3.4.1)
- [Ceres Solver](http://ceres-solver.org/)

### 2. Build
```
cd ~/controls_ws/src
git clone --recursive https://github.com/amancodeblast/Unconstrained-Line-based-SLAM.git
cd ..
catkin_make
source ~/controls_ws/devel/setup.bash
```

## Run on EuRoC datasets
Download [EuRoC MAV Dataset](http://projects.asl.ethz.ch/datasets/doku.php?id=kmavvisualinertialdatasets).
Open three terminals and launch the vins_estimator, rviz, and play the bag file, respectively.
The files that were specifically downloaded are [easy, medium and Hard rosbag files](http://robotics.ethz.ch/~asl-datasets/ijrr_euroc_mav_dataset/machine_hall/)

```
roslaunch uv_slam euroc.launch
roslaunch uv_slam vins_rviz.launch
rosbag play MH_04_difficult.bag
```

## Related Links
Official page of *"UV-SLAM: Unconstrained Line-based SLAM Using Vanishing Points for Structural Mapping"*, which is published in IEEE RA-L with ICRA'22 presentation option.
For more details, please refer to: https://doi.org/10.1109/LRA.2022.3140816