# Robotics Portfolio: Fazal E Haq

**Robotics Design & Control Systems Engineer** · Islamabad, Pakistan

## Featured Research: MS Thesis

**Design and Control of a Modular and Flexible 7-DOF Robotic Manipulator**<br>
MS Electrical Engineering (Control Systems), SEECS, National University of Sciences and Technology (NUST), Islamabad, 2026<br>
Supervisor: Dr. Latif Anjum · Co-supervisor: Dr. Usman Ali · DAAD funded the actuators, power supply and workstation

<table>
<tr>
<td width="33%" align="center"><img src="assets/thesis/7dof_render.jpg" width="100%"><br><sub>7-DOF build, SolidWorks render</sub></td>
<td width="33%" align="center"><img src="assets/thesis/7dof_hardware_upright.jpg" width="100%"><br><sub>Upright build on the lab bench</sub></td>
<td width="33%" align="center"><img src="assets/thesis/7dof_hardware_inverted.jpg" width="100%"><br><sub>Inverted 6-DOF build under a workbench</sub></td>
</tr>
</table>

### Objective

Design and build, from scratch, one research platform that a university lab can reconfigure from a 7-DOF arm down to a 3-DOF arm. Students can learn control on a simple build and then scale up to the full 7-DOF arm with the same hardware.

### Design process

1. **Requirements and actuator limits.** The actuators arrived before the design existed, so I sized the link lengths and mass around their torque limits.
2. **CAD design.** I modelled the joint modules and aluminium extension rods in SolidWorks, so one module set assembles into several arms.
3. **Torque budget.** I built a gravity-aware torque budget from the CAD mass properties. The first prototype could not hold its own weight, so I shortened the links and added a 10:1 planetary gearbox at the shoulder.
4. **Fabrication.** I compared CNC, lathe and 3D printing, chose lathe-turned aluminium parts and released the drawings to the workshop.
5. **Electronics.** A 48 V supply and a CAN bus split across two controllers run the control loop at 100 Hz.
6. **Simulation.** I built URDF models of every build and tested them in CoppeliaSim and PyBullet before running the hardware.
7. **Assembly and commissioning.** I assembled the arm, tuned each joint drive and commissioned the builds step by step on the bench.

### Techniques applied

Forward and inverse kinematics · Jacobian and manipulability analysis · workspace analysis · rigid-body dynamics · computed torque control with PID and friction compensation · trajectory generation · simulation-to-hardware comparison

### Outcome

- One module set builds **eight arms from 3 to 7 DOF**, including an inverted arm mounted under a workbench.
- The 7-DOF build weighs 20.8 kg and reaches 0.85 m.
- One set of controller gains works on every build without retuning in simulation.
- Computed torque control runs on the hardware; gain tuning is in progress.
- Hardware and fabrication cost PKR 111,400, of which PKR 100,000 came from the MS research grant.

<table>
<tr>
<td width="40%" align="center"><img src="assets/previews/7dof_hardware_vs_simulation.gif" width="100%"><br><sub>Hardware and CoppeliaSim model reach the same waypoints</sub></td>
<td width="20%" align="center"><img src="assets/thesis/7dof_pick_and_place.gif" width="100%"><br><sub>Pick-and-place on the inverted build</sub></td>
<td width="40%" align="center"><img src="assets/thesis/7dof_circle_trajectory_torque_control.gif" width="100%"><br><sub>Circular trajectory under torque control in simulation</sub></td>
</tr>
</table>

### Next steps

Finish gain tuning of the torque controller on hardware, identify joint friction on the assembled arm, and apply redundancy resolution to the 7-DOF build. The arm is in the ROMI Lab, NUST. The full thesis is available on request.

---

## Portfolio

Mechanical design and robot modelling in **SolidWorks**, with **URDF / ROS** exports, simulation and built hardware. The projects below span serial arms from 3 to 7 DOF, adaptive grippers, heavy two-axis mounts and an automation cell.

> **Full project files are private.** Native SolidWorks and STEP models, URDF packages, 2D drawings, BOMs and full-length videos for every project are kept in a private repository. **Access is available upon request** (see [Request access](#request-access)).

**Skills shown:** SolidWorks part/assembly design · design for 3D printing and machining · URDF export and ROS packages (RViz, Gazebo) · mass properties and joint torque sizing · SolidWorks Simulation (FEA) · 2D manufacturing drawings · BOMs and fastener schedules · assembly animations · hardware prototyping and trajectory control

## Highlights

<table>
<tr>
<td width="50%" align="center"><img src="assets/previews/7dof_hardware_vs_simulation.gif" width="100%"><br><sub>7-DOF arm: hardware and simulation running side by side</sub></td>
<td width="50%" align="center"><img src="assets/previews/5dof_urdf_test.gif" width="100%"><br><sub>5-DOF extrusion-link arm: URDF joint test</sub></td>
</tr>
<tr>
<td align="center"><img src="assets/previews/scara_hardware.gif" width="80%"><br><sub>3-DOF SCARA: printed and assembled prototype</sub></td>
<td align="center"><img src="assets/previews/finray_gripper_demo.gif" width="55%"><br><sub>Fin Ray gripper conforming to objects</sub></td>
</tr>
</table>

## Projects

<table>
<tr>
<td width="33%" align="center" valign="top"><img src="assets/thumbs/arm_7dof.jpg"><br><b>7-DOF Modular Manipulator (MS Thesis)</b><br><sub>Designed from scratch; one module set reconfigures from 7 DOF to 3 DOF; 20.8 kg aluminium arm running computed torque control</sub></td>
<td width="33%" align="center" valign="top"><img src="assets/thumbs/so_arm_5dof.jpg"><br><b>5-DOF Extrusion-Link Arm (Modified SO-ARM)</b><br><sub>30 × 30 mm aluminium extrusion links, FEETECH STS3250 / STS3215 bus servos, 400 g payload target, URDF/ROS package</sub></td>
<td width="33%" align="center" valign="top"><img src="assets/thumbs/arm_6dof.jpg"><br><b>6-DOF Low-Cost Servo Arm</b><br><sub>MG996R / SG90 servos, rack-and-pinion gripper, 422.9 mm reach, joint torque budget from mass properties, URDF</sub></td>
</tr>
<tr>
<td align="center" valign="top"><img src="assets/thumbs/scara.jpg"><br><b>3-DOF SCARA Manipulator</b><br><sub>3D-printed SCARA with rack-and-pinion Z axis; FEA-checked brackets; fabricated and assembled with no redesign</sub></td>
<td align="center" valign="top"><img src="assets/thumbs/finray.jpg"><br><b>Fin Ray Effect Adaptive Gripper</b><br><sub>Compliant fingers, single servo with gear-synchronised motion, printed and tested on hardware</sub></td>
<td align="center" valign="top"><img src="assets/thumbs/so_arm_101.jpg"><br><b>SO-ARM 101 Modified: URDF Generation</b><br><sub>SolidWorks remodel of the follower arm, link frames and joint limits, exported and validated URDF</sub></td>
</tr>
<tr>
<td align="center" valign="top"><img src="assets/thumbs/m2_turret.jpg"><br><b>Heavy Two-Axis Turret Mount</b><br><sub>Slewing-bearing traverse with spur-gear reduction; BOM, fastener schedule, bearing spec and assembly animations</sub></td>
<td align="center" valign="top"><img src="assets/thumbs/pkm_turret.jpg"><br><b>Two-Axis Turret Mount: Manufacturing Package</b><br><sub>NEMA 34 geared drive; 43 parts, 19 manufacturing drawings, 27 printable STL parts, screw BOM</sub></td>
<td align="center" valign="top"><img src="assets/thumbs/workcell.jpg"><br><b>Vision-Guided Pick-and-Place Cell</b><br><sub>Cobot, belt conveyor and overhead camera mast on an aluminium-extrusion frame</sub></td>
</tr>
</table>

## What each private project folder contains

| Folder | Content |
|---|---|
| `media/` | Renders, photos, full-length MP4 videos |
| `cad/` | STEP assembly and native SolidWorks parts and assemblies |
| `urdf/` | ROS description package: URDF, meshes, RViz and Gazebo launch files |
| `drawings/` | 2D manufacturing drawings (PDF + SLDDRW) |
| `stl/` | Print-ready STL files |
| `docs/` | BOMs, fastener schedules, specifications |

## Request access

To review the full CAD, URDF and drawing files for any project, contact me with your **GitHub username** and I will add you to the private repository.

- **Email:** [fhaq.msee23seecs@seecs.edu.pk](mailto:fhaq.msee23seecs@seecs.edu.pk)
- **OR:**[fhengineer68@gmail.com](mailto:fhengineer68@gmail.com)
- **LinkedIn:** [Fazal E Haq](http://www.linkedin.com/in/fazal-e-haq-84b2b821b/)
- **Fiverr:** [fiverr.com/fazalehaq_123](https://www.fiverr.com/fazalehaq_123)
