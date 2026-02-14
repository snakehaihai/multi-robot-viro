# VIRO EPDOP+HVCE Package 🚀

## 📦 Package Information

**Package Name:** `viro_epdop_hvce`

**Description:** Multi-Robot Visual-Inertial-Ranging Odometry with EPDOP screening and HVCE re-weighting

**Maintainer:** VIRO Team

**License:** GPL-2.0

## 📂 Package Structure

```
viro_epdop_hvce/
├── launch/              # ROS launch files
│   ├── viro_epdop_hvce.launch
│   └── multi_robot.launch
├── config/              # Configuration files
│   └── viro_params.yaml
├── scripts/             # Python scripts
│   └── placeholder.py
├── docs/                # Documentation
│   ├── README.md
│   ├── EPDOP.md
│   └── HVCE.md
├── include/             # C++ header files
│   └── viro_epdop_hvce/
│       └── viro_core.h
├── src/                 # C++ source files
│   ├── viro_core.cpp
│   └── viro_node.cpp
├── CMakeLists.txt       # CMake build configuration
└── package.xml          # ROS package manifest
```

## 🎯 Key Features

- 🎯 **EPDOP Screening**: Geometric quality-based measurement screening
- ⚖️ **HVCE Re-weighting**: Uncertainty-aware measurement re-weighting
- 🤖 **Multi-Robot Support**: Distributed state estimation across multiple robots
- 📡 **Sensor Fusion**: Visual, inertial, and ranging measurements
- 🔧 **Configurable**: Extensive parameter tuning options

## 🛠️ Dependencies

### ROS Packages
- `roscpp`
- `rospy`
- `std_msgs`
- `sensor_msgs`
- `geometry_msgs`
- `nav_msgs`
- `tf`
- `cv_bridge`
- `image_transport`

### System Dependencies
- `Eigen3`
- `OpenCV`

## 🚀 Quick Start

### Building the Package

```bash
cd ~/catkin_ws/src
git clone https://github.com/snakehaihai/multi-robot-viro.git
cd ~/catkin_ws
catkin_make
source devel/setup.bash
```

### Running Single Robot

```bash
roslaunch viro_epdop_hvce viro_epdop_hvce.launch
```

### Running Multi-Robot System

```bash
roslaunch viro_epdop_hvce multi_robot.launch num_robots:=3
```

## ⚙️ Configuration

Configuration parameters can be adjusted in `config/viro_params.yaml`:

- **EPDOP Parameters**: Screening thresholds and adaptive settings
- **HVCE Parameters**: Re-weighting factors and covariance options
- **Visual Parameters**: Feature detection and tracking settings
- **IMU Parameters**: Noise characteristics and biases
- **Ranging Parameters**: UWB/ranging measurement settings
- **Multi-Robot Parameters**: Number of robots and communication settings

## 📖 Documentation

Detailed documentation is available in the `docs/` directory:

- [Main Documentation](docs/README.md)
- [EPDOP Algorithm](docs/EPDOP.md)
- [HVCE Algorithm](docs/HVCE.md)

## 🔬 Research

This work is currently under review at IEEE Transactions on Instrumentation and Measurement (TIM).

**Citation:** (Will be provided upon acceptance)

## 📝 Notes

⚠️ This is a placeholder implementation. The full system implementation will be released publicly upon paper acceptance.

## 📧 Contact

For questions or collaboration opportunities, please contact the maintainers through the GitHub repository.

## 📄 License

This project is licensed under the GPL-2.0 License - see the [LICENSE](../LICENSE) file for details.
