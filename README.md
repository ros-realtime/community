# ROS 2 Real-Time Working Group

This document defines the scope and governance of the ROS 2 Real-Time Working Group.

The Real-Time Working Group's mission is to advocate for and work on memory management, real-time pub/sub, real-time DDS, and tools that allow tracing, profiling and optimizing.

## Subprojects

This Working Group owns and maintains the following Subprojects.
Its meetings and membership are largely focused on the direction, design, and work on the projects.

### Subproject List

The following subprojects are owned by Real-Time Working Group:

- rt-kernel-docker-builder
  - Description:  Build and setup RT kernel for the ROS2 testing
  - Repositories
    - https://github.com/ros-realtime/rt-kernel-docker-builder

#### Related Projects

Performance measurements

- performance_test
  - Description: Tool to test the performance of pub/sub based communication frameworks
  - Repositories
    - https://gitlab.com/ApexAI/performance_test
- ros2-performance
  - Description: iRobot ROS 2 performance evaluation framework
  - Repositories
    - https://github.com/irobot-ros/ros2-performance
- buildfarm_perf_tests
  - Description: Performance tests which run regularly on the ROS 2 buildfarm
  - Repositories
    - https://github.com/ros2/buildfarm_perf_tests   
- TwoWaysMeasurement
  - Description: Tool to test the real-time performance in a ping-pong scenario
  - Repositories
    - https://github.com/y-okumura-isp/TwoWaysMeasurement
- ros2_timer_latency_measurement
  - Description: Tool to measure the accuracy of the ROS 2 timer
  - Repositories
    - https://github.com/hsgwa/ros2_timer_latency_measurement
- ros2_benchmarking
  - Description: Tool to compare ROS and ROS 2 communications.
  - Repositories
    - https://github.com/piappl/ros2_benchmarking
- adlink_ros2_tools
  - Description: ADLINK's performance evaluation tool. Centered around Opensplice DDS implementation.
  - Repositories
    - https://github.com/Adlink-ROS/adlink_ros2_tools
- ros2_latency_evaluation
  - Description: Forked from ros2-performance. Tool for evaluating ROS 2 latencies.
  - Repositories
    - https://github.com/Barkhausen-Institut/ros2_latency_evaluation


Real-time utilities

- realtime_support
  - Description: Minimal real-time testing utility for measuring jitter and latency
    - rttest: rttest is a minimal tool for instrumenting and running tests for synchronous real-time systems
    - tlsf_cpp: C++ stdlib-compatible wrapper around tlsf allocator and ROS2 examples
  - Repositories
    - https://github.com/ros2/realtime_support
- ros2_tracing
  - Description: Tracing tools for ROS 2
  - Repositories
    - https://gitlab.com/ros-tracing/ros2_tracing
    - https://gitlab.com/ros-tracing/tracetools_analysis
- osrf_testing_tools_cpp
  - Description: This repository contains testing tools for C++, and is used in OSRF projects. The memory_tools API lets you intercept calls to dynamic memory calls like malloc and free, and provides some convenience functions for differentiating between expected and unexpected calls to dynamic memory functions.
  - Repositories:
    - https://github.com/osrf/osrf_testing_tools_cpp
- apex_test_tools
  - Description: The package Apex.OS Test Tools contains test helpers
  - Repositories:
    - https://gitlab.com/ApexAI/apex_test_tools
- apex_containers
  - Description: A collection of C++ containers suitable for real time systems
  - Repositories:
    - https://gitlab.com/ApexAI/apex_containers
- realtime_tools
  - Description: Contains a set of tools that can be used from a hard realtime thread, without breaking the realtime behavior
  - Repositories:
    - https://github.com/ros-controls/realtime_tools/tree/foxy-devel

Real-time demos

- pendulum_control
  - Description: Real-time inverted pendulum control demo
  - Repositories
    - https://github.com/ros2/demos/tree/master/pendulum_control
    - https://docs.ros.org/en/foxy/Tutorials/Real-Time-Programming.html
- pendulum
  - Description: Inverted pendulum demo inspired by pendulum_control
  - Repositories
    - https://github.com/ros2-realtime-demo/pendulum
- e2e_demo
  - Description: End-to-end latency demo
  - Repositories
    - https://github.com/hsgwa/e2e_demo

### Meetings

* Regular WG Meeting: every other Tuesday at 7 AM Pacific time, see the [ROS Events calendar](https://calendar.google.com/calendar/embed?src=agf3kajirket8khktupm9go748%40group.calendar.google.com&ctz=America%2FLos_Angeles)
* To receive meeting invitations, join [ros-real-time-working-group-invites](https://groups.google.com/forum/#!forum/ros-real-time-working-group-invites)
* Meeting notes are kept under [ROS 2 Real-time Working Group Agenda](https://docs.google.com/document/d/1zBKwDUDeWvJNyCvjzYriaZQoZO2VYGWe1uxw5Xxn5cY/edit?ts=5ec9aabe#heading=h.rwvriogv081)
* Meetings are recorded and available in [ROS 2 Real-time Working Group Agenda](https://docs.google.com/document/d/1zBKwDUDeWvJNyCvjzYriaZQoZO2VYGWe1uxw5Xxn5cY/edit?ts=5ec9aabe#heading=h.rwvriogv081).
* Meetings are open to the public, and anyone is welcome to join

### Communication Channels

- ROS discourse tag [wg-real-time](https://discourse.ros.org/tag/wg-real-time)
- Chat in the [Real-time WG Room on Matrix](https://matrix.to/#/#ros-realtime:matrix.org?via=matrix.org)

### Governance

See the [governance](governance.md) document for more information.

### How to Contribute

See the [contributing](CONTRIBUTING.md) document for more information.

