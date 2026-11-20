# Grass Watch — agricultural mobile robot in simulation

**Technology:** ROS 2 (Humble / Iron), Gazebo Classic, Nav2, RViz2, Python, URDF, NumPy, Pillow.

A simulated agricultural mobile robot with keyboard teleoperation, autonomous return-to-start behavior, and systematic lawnmower-style coverage.

**Pipeline:** `grass_world.world` → `farm_robot` (`assembly.urdf`) → Nav2 + RViz2 → autonomous behaviors.

**Reported workspace structure:** `Robot/src/my_robot/` (ROS packages), `Robot/maps/` (PGM/YAML occupancy maps), `Dataset/`, `scripts/`, and `generate_map.py`.

**Source availability:** This page documents the portfolio project; its complete workspace has not been provided to this GitHub repository. Related ROS 2 code: [ROS projects](https://github.com/ayman2218?tab=repositories).
