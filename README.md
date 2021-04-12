# gnss_comm

**Authors/Maintainers:** CAO Shaozu (shaozu.cao AT gmail.com)

The *gnss_comm* package contains basic definitions and utility functions for GNSS raw measurement processing. 

## 1. Prerequisites

### 1.1 C++11 Compiler
This package requires some features of C++11.

### 1.2 ROS
This package is developed under [ROS Kinetic](http://wiki.ros.org/kinetic) environment.

### 1.3 Eigen
Our code uses [Eigen 3.3.3](https://gitlab.com/libeigen/eigen/-/archive/3.3.3/eigen-3.3.3.zip) for matrix manipulation. After downloading and unzipping the Eigen source code package, you may install it with the following commands:

```
cd eigen-3.3.3/
mkdir build
cd build
cmake ..
sudo make install
```

### 1.4 Glog
We use google's glog library for message output. If you are using Ubuntu, install it by:
```
sudo apt-get install libgoogle-glog-dev
```
If you are on other OS or just want to build it from source, please follow [these instructions](https://github.com/google/glog#building-glog-with-cmake) to install it.


## 2. Build gnss_comm library
Clone the repository to your catkin workspace (for example `~/catkin_ws/`):
```
cd ~/catkin_ws/src/
git clone https://github.com/HKUST-Aerial-Robotics/gnss_comm.git
```
Then build the package with:
```
cd ~/catkin_ws/
catkin_make
source ~/catkin_ws/devel/setup.bash
```

## 3. Acknowledgements
Many of the definitions and utility functions in this package are adapted from [RTKLIB](http://www.rtklib.com/).

## 4. License
The source code is released under [GPLv3](https://www.gnu.org/licenses/gpl-3.0.html) license.
