Overview
This repository contains a high-fidelity Simulink model for simulating a rocket with thrust vector control (TVC) in a 6 Degrees of Freedom (6DOF) environment. The model is designed to help study the dynamics and control of rockets, simulating realistic flight dynamics and enabling the testing of control algorithms for trajectory optimization and stabilization.

The project is part of a thesis that explores thrust vector control systems and trajectory optimisation for precision landing of rockets. This simulation provides a foundation for understanding the coupled rotational and translational dynamics of a rocket and serves as a testing ground for control systems such as Model Predictive Control (MPC).

Features
6DOF Dynamics: Models the full 6DOF translational and rotational motion of a rocket.
(SOON)Thrust Vector Control (TVC): Includes a TVC mechanism for dynamic control of the rocket's orientation.
Aerodynamic Modeling: Integrates aerodynamic forces and moments based on angle of attack (AOA) and sideslip angle (beta).
Environment Effects: Accounts for environmental conditions such as gravity and wind disturbances.
VisualiSation: Provides a visual output of the rocket's flight path and orientation through 3D visualization tools.
Trajectory and State Estimation: Computes the velocity, position, and angular orientation (roll, pitch, yaw) over time.
Model Structure
Key Components
Rocket Block: Handles parameters such as mass, inertia, and thrust. This block incorporates the dynamic changes in rocket mass due to fuel consumption.
Environment Block: Models environmental inputs including wind velocity and gravitational force acting on the rocket.
Aerodynamics Block: Calculates aerodynamic forces (lift, drag) and moments based on AOA and beta, using lookup tables and coefficients.
(SOON)_TVC Dynamics: Controls the direction of thrust for stabilization and trajectory control, simulating a gimballed engine.
Equations of Motion (EOM): Core dynamic equations that integrate forces and moments to yield translational and rotational accelerations.
Rotation and Transformation Block: Converts between body and inertial frames, ensuring accurate representation of the rocket’s orientation and motion in the simulation.
Visualisation Block: Outputs the rocket’s trajectory and orientation, enabling 3D visualization of its flight path.
