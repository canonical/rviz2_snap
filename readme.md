# RViz 2 snap

A [classic confinement](https://snapcraft.io/docs/classic-confinement) snap of [RViz 2](https://github.com/ros2/rviz),
the 3D visualization tool for ROS 2 (Jazzy).

## Install

```bash
sudo snap install rviz2 --classic
```

This installs from the `jazzy/stable` channel.

## Usage

```bash
rviz2
```

Because this is a **classic** snap,
it runs in the host namespace and uses the
host's ROS 2 graph and graphics stack.
If you source your ROS 2 Jazzy installation or a local Jazzy workspace before launching, 
RViz 2 will discover and load the plugins available in that environment:

```bash
source /opt/ros/jazzy/setup.bash   # or your workspace's install/setup.bash
rviz2
```
