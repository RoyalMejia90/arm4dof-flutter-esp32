# arm4dof-flutter-esp32

4-DOF robotic arm controlled via ESP32, Flutter app and Python visualizer.
Biomechanics course project — Yachay Tech University, Ecuador.

---

## About

This project is an improvement of an existing Arduino-based robotic arm. It migrates the control to an **ESP32**, adds wireless Bluetooth control through a **Flutter mobile app**, and includes a **Python 3D visualizer** that shows the arm movement in real time alongside the physical arm.

---

## Hardware

- Acrylic structure based on SolidWorks design
- 4× MG90S servo motors — one per degree of freedom (base, shoulder, elbow, gripper)
- ESP32 as main microcontroller

---

## Flutter App — Control Modes

| # | Screen | Description |
|---|---|---|
| 1 | Inverse kinematics | Control by joint angles (0–180°) or XYZ position |
| 2 | Recorded movements | Predefined demo sequences; record and replay new ones |
| 3 | Motion control (IMU) | Move the phone in your hand to control the arm via accelerometer and gyroscope |

---

## Project Structure

| Module | Description |
|---|---|
| `firmware/` | ESP32 code — servo control, BLE, PID, transformation matrices |
| `app/` | Flutter app — mobile control interface |
| `visualizer/` | Python script — real-time 3D visualization |
| `hardware/` | SolidWorks files and physical design reference |

---

## Progress

- [x] Mechanical design (SolidWorks + acrylic cut)
- [x] Inverse kinematics (Arduino base project)
- [ ] ESP32 firmware migration
- [ ] Flutter app
- [ ] Python 3D visualizer

---

## Credits

Based on the MeArm robotic arm project by **Mario Youchia**:

- 3D Model: [MeArm Robotic Arm — GrabCAD](https://grabcad.com/library/mearm-robotic-arm-1)
- YouTube: [@marioyouchia](https://www.youtube.com/@marioyouchia)
- GitHub: [Mario-Youchia](https://github.com/Mario-Youchia)
- Base project: [MeArm-Robotic-Arm-Control](https://github.com/Mario-Youchia/MeArm-Robotic-Arm-Control)

---

## Institution

**Yachay Tech University** — Urcuquí, Ecuador
Biomechanics Course — Group Project

Team members: *(to be added)*

---

## License

MIT
