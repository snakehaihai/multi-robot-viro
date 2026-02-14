🚧 This repository currently provides the project structure and baseline configuration/scripts for reproducibility; the full implementation will be released publicly upon acceptance (TIM, under review).

# Multi-Robot VIRO 🤖🔬

[![ROS Version](https://img.shields.io/badge/ROS-Noetic-blue.svg)](http://wiki.ros.org/noetic)
[![Build Type](https://img.shields.io/badge/Build-Catkin-green.svg)](http://wiki.ros.org/catkin)
[![License](https://img.shields.io/badge/License-GPL--2.0-orange.svg)](LICENSE)

## 📖 Overview

**VIRO** (Visual-Inertial-Ranging Odometry) is a multi-robot localization system that combines:

- 📷 **Visual Odometry**: Feature-based visual tracking
- 🎯 **Inertial Measurements**: IMU-based motion estimation  
- 📡 **Ranging Measurements**: UWB inter-robot distance measurements
- 🔍 **EPDOP Screening**: Geometric quality-based measurement screening
- ⚖️ **HVCE Re-weighting**: Uncertainty-aware measurement re-weighting

## 🚀 Features

- ✅ Multi-robot distributed state estimation
- ✅ Robust measurement screening (EPDOP)
- ✅ Adaptive measurement weighting (HVCE)
- ✅ ROS1 (Catkin) integration
- ✅ Configurable parameters
- ✅ Modular architecture

## 📦 Package Structure

```
multi-robot-viro/
└── viro_epdop_hvce/          # Main VIRO package
    ├── launch/                # Launch files
    ├── config/                # Configuration files
    ├── scripts/               # Python scripts
    ├── docs/                  # Documentation
    ├── include/               # C++ headers
    ├── src/                   # C++ source
    ├── CMakeLists.txt         # Build configuration
    ├── package.xml            # Package manifest
    └── README.md              # Package documentation
```

## 🛠️ Installation

### Prerequisites

- ROS Noetic (or ROS Melodic)
- C++14 compiler
- CMake 3.0.2+
- Eigen3
- OpenCV

### Build Instructions

```bash
# Create catkin workspace
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/src

# Clone repository
git clone https://github.com/snakehaihai/multi-robot-viro.git

# Build
cd ~/catkin_ws
catkin_make

# Source workspace
source devel/setup.bash
```

## 🎯 Quick Start

### Single Robot Launch

```bash
roslaunch viro_epdop_hvce viro_epdop_hvce.launch
```

### Multi-Robot Launch

```bash
roslaunch viro_epdop_hvce multi_robot.launch num_robots:=3
```

### Configuration

Adjust parameters in `viro_epdop_hvce/config/viro_params.yaml`

## 📚 Documentation

For detailed documentation, see:
- [Package Documentation](viro_epdop_hvce/README.md)
- [EPDOP Algorithm](viro_epdop_hvce/docs/EPDOP.md)
- [HVCE Algorithm](viro_epdop_hvce/docs/HVCE.md)

## 🔬 Research & Citation

This work is currently under review at **IEEE Transactions on Instrumentation and Measurement (TIM)**.

Citation information will be provided upon acceptance.

## ⚠️ Status

**Note:** This repository currently contains the project structure and baseline configuration/scripts. The full implementation will be released publicly upon paper acceptance.

## 📄 License

This project is licensed under the **GPL-2.0 License** - see the [LICENSE](LICENSE) file for details.

## 📧 Contact

For questions, issues, or collaboration:
- 🐛 [Open an Issue](https://github.com/snakehaihai/multi-robot-viro/issues)
- 📫 Contact maintainers via GitHub

## 🙏 Acknowledgments

Special thanks to all contributors and reviewers.

---

**Maintained with ❤️ by the VIRO Team**