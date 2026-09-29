# Aconit AD-1 – Autonomous Flying-Wing Interceptor Drone

<p align="center">
  <img src="images/aconit.jpg" alt="Aconit AD-1" width="700">
</p>

Aconit AD-1 is an autonomous flying-wing drone designed to detect and intercept other drones.
It is developed as a fourth-year engineering project at Polytech Nice Sophia (Robotics and Autonomous Systems),
and covers the full development cycle: airframe design, electronics, flight control and embedded vision.

## Purpose

The growing use of small drones raises new security challenges for airports, public events and sensitive sites.
This project explores a low-cost interception approach: a fast, fixed-wing platform able to detect a target drone
with its onboard camera and guide itself towards it autonomously.

## Key Figure

| Parameter | Value |
|---|---|
| Maximum interception speed | approx. 150–160 km/h (design estimate, not yet flight-tested) |

## System Overview

| Subsystem | Description |
|---|---|
| Airframe | Double-delta flying wing, designed in Fusion 360 and 3D-printed, powered by an electric ducted fan |
| Power electronics | Custom power distribution board designed in KiCad |
| Flight controller | ESP32-S3 based board with inertial measurement unit, barometer and radio link |
| Flight control | In-house control laws: PID controllers and control-surface mixing matrices, without an off-the-shelf autopilot |
| Embedded vision | Real-time target detection with YOLO on an RDK X5 board, integrated with ROS 2 |

<p align="center">
  <img src="images/architecture.png" alt="System architecture" width="600">
</p>

## Gallery

<p align="center">
  <img src="images/cad.jpg" alt="CAD model" width="320">
  <img src="images/printed-wing.jpg" alt="3D-printed airframe" width="320">
</p>

## Project Status

🟢 Completed  ·  🟠 In progress  ·  ⚪ Planned

| Status | Task |
|:---:|---|
| 🟢 | Airframe design and 3D printing |
| 🟢 | Power distribution board design and manufacturing |
| 🟠 | Flight controller and control laws (PID, control-surface mixing matrices) |
| 🟠 | Target detection on RDK X5 and ROS 2 integration |
| ⚪ | Final assembly and first flight |

## Tools and Technologies

Fusion 360 · 3D printing · KiCad · ESP32-S3 · C/C++ · Python · ROS 2 · YOLO · RDK X5

## Author

**Vladimir Grigoriev** – Robotics engineering student, Polytech Nice Sophia
[LinkedIn](https://www.linkedin.com/in/vladimir-grigoriev-nice) · [GitHub](https://github.com/grigoriev-vladimir)

---

*Design files and flight software are not published in this repository.*
