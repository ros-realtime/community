# Test environment

This document describes a test environment used for the ROS2 real-time tests

## Hardware

Two hardware platforms:
* Hardware architecture
    * Intel x86_64
    * ARM v8
* Number of CPU cores => 4
* Amount of RAM => 8 GB
* supports Ubuntu 20.04 LTS release

### ARM

* [Raspberry Pi 4 8 GB RAM, 4 CPU cores](https://www.raspberrypi.org/blog/8gb-raspberry-pi-4-on-sale-now-at-75) or similar

### Intel

* any Intel PC with 8 GB RAM, 4 CPU cores
* [UP squared 8 GB RAM, 4 CPU cores](https://up-shop.org/up-squared-board-pentium-quad-core-8gb-memory-64gb-emmc.html)

## Software

We use ROS2 Foxy release and Ubuntu 20.04 which is a Tier 1 platform as described in the [Release information](https://docs.ros.org/en/foxy/Releases/Release-Foxy-Fitzroy.html#supported-platforms).

### ROS2 foxy release 

* Prebuilt Debian packages from [Installing ROS 2 via Debian Packages](https://docs.ros.org/en/foxy/Installation/Linux-Install-Debians.html)

### Latest Ubuntu 20.04 LTS (ISO image)

* [Raspberry Pi4](https://ubuntu.com/download/raspberry-pi)
* [Intel UP squared](https://wiki.up-community.org/Ubuntu)
* [Intel Ubuntu 20.04.2.0 LTS](https://ubuntu.com/download/desktop)

### Latest Stable PREEMPT_RT Kernel

* PREEMPT_RT Kernel is built using [these instructions](https://github.com/ros-realtime/rt-kernel-docker-builder)

