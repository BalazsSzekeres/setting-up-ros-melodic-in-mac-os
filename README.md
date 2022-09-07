# Setting up ROS Melodic in Mac OS

This repo provides a tutorial on how to setup ROS Melodic in Mac OS using Ubuntu 18.04 via Parallels 17.

The pre-requisites are:
- macOS Monterey
- Parallels 17

This tutorial should work both with Intel based Mac's as well as with Apple Silicone.

## Setting up Ubuntu 18.04 with Parallels 17
1. Download the Ubuntu mini iso: `http://ports.ubuntu.com/ubuntu-ports/dists/bionic-updates/main/installer-arm64/current/images/netboot/`
2. Install the ISO in Parallels with the default settings, and optionally select a GUI during the installation.

## Install ROS Melodic in the Virtual Machine
1. `sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'`
2. `sudo apt install curl`
3. `curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -`
4. `sudo apt update`
5. `sudo apt install ros-melodic-desktop-full`
6. `sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential`
7. `pip3 install --upgrade setuptools`




