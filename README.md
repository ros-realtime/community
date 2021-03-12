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
  - Description: iRobot ROS2 performance evaluation framework
  - Repositories
    - https://github.com/irobot-ros/ros2-performance
- TwoWaysMeasurement
  - Description: Tool to test the real-time performance in a ping-pong scenario
  - Repositories
    - https://github.com/y-okumura-isp/TwoWaysMeasurement
- ros2_timer_latency_measurement
  - Description: Tool to measure the accuracy of the ROS 2 timer
  - Repositories
    - https://github.com/hsgwa/ros2_timer_latency_measurement

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

### Standards for subprojects

Subprojects must meet the following criteria (and the WG agrees to maintain them upon adoption).

* Build passes against ROS 2 master
* The ROS 2 standard linter set is enabled and adhered to
* If packages are part of nightly builds on the ROS build farm, there are no reported warnings or test failures
* Quality builds are green (address sanitizer, thread sanitizer, clang thread safety analysis)
* Test suite passes
* Code coverage is measured, and non-decreasing level is enforced in PRs
* Issues and pull requests receive prompt responses
* Releases go out regularly when bugfixes or new features are introduced
* The backlog is maintained, avoiding longstanding stale issues

### Adding new subprojects

To request introduction of a new subproject, add a list item to the "Subprojects" section and open a Pull Request to this repository, following the default Pull Request Template to populate the text of the PR.

PR will be merged on unanimous approval from Approvers.

### Subproject changes

Modify the relevant list item in the "Subprojects" section and open a Pull Request to this repository, following the default Pull Request Template to populate the text of the PR.

PR will be merged on unanimous approval from Approvers.

### Deprecating subprojects

Projects cease to be useful, or the WG can decide it is no longer in their interest to maintain.
We do not commit to maintaining every subproject in perpetuity.

To suggest removal of a subproject, remove the relevant list item in the "Subprojects" section and open a Pull Request in this repository, following instructions in the Pull Request Template to populate the text of the PR.

PR will be merged on unanimous approval from Approvers.

If the repositories of the subproject are under the WG's GitHub organization, they will be transferred out of the organization or deleted at this time.

## Governance

See the [WG section of the ROS 2 Project Governance page](https://index.ros.org/doc/ros2/Governance/#working-groups-wgs).

### Meetings

* Regular WG Meeting: every other Tuesday at 7 AM Pacific time, see the [ROS Events calendar](https://calendar.google.com/calendar/embed?src=agf3kajirket8khktupm9go748%40group.calendar.google.com&ctz=America%2FLos_Angeles)
* To receive meeting invitations, join [ros-real-time-working-group-invites](https://groups.google.com/forum/#!forum/ros-real-time-working-group-invites)
* Meeting notes are kept under [ROS 2 Real-time Working Group Agenda](https://docs.google.com/document/d/1zBKwDUDeWvJNyCvjzYriaZQoZO2VYGWe1uxw5Xxn5cY/edit?ts=5ec9aabe#heading=h.rwvriogv081)
* Meetings are recorded and available on Discourse: [wg-real-time](https://discourse.ros.org/tag/wg-real-time).
* Meetings are open to the public, and anyone is welcome to join

### Communication Channels

This working group uses Discourse: [wg-real-time](https://discourse.ros.org/tag/wg-real-time).

<!--
### Backlog Management

{{Is any project management software/site used to track work for this Working Group? How can new members discover the highest impact tasks they could take on? GitHub Projects, ZenHub, etc.}}
-->

### Membership, Roles and Organization Management

Working Group members may act in one or more of the following roles:

* **Member**
  * Prerequisite: Attend at least one out of the last three Working Group meetings
  * Responsible for triaging issues
* **Reviewer**
  * All reviewers are members
  * Prerequisite: Proven track record of high-quality reviews to WG Subprojects
  * Responsible for reviewing pull requests
* **Approver**
  * All approvers are reviewers
  * Prerequisite: Proven track record of high-quality contributions and reviews to WG Subprojects
  * Responsible for approving and merging pull requests
  * Responsible for vetting and accepting new projects into the Working Group
* **Lead**
  * TSC member or their delegate
  * Responsible for organizing and moderating working group meetings
  * Responsible for posting meeting materials (minutes, recordings, etc.)
  * Responsible for breaking ties

To become a member or change role, create an issue in this repository using the appropriate issue template.
Such applications are accepted upon unanimous agreement from Approvers, and are typically based on the applicant's history with the subprojects of the Working Group.
The Lead role cannot be applied for, as it is an appointee of the ROS 2 TSC.

### Modifying this governance document

Changes to this document will be made via Pull Request.
The PR will be merged on unanimous agreement from Approvers.
