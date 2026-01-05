# 🚁 Web-Based Drone Flight Simulator

![Project Status](https://img.shields.io/badge/Status-Active_Development-green)
![Tech](https://img.shields.io/badge/Built_With-Three.js_|_WebGL-black)
![License](https://img.shields.io/badge/License-MIT-blue)

A realistic, physics-based drone flight simulator that runs entirely in your web browser. Built with **Three.js** and the **Web Gamepad API**, this project simulates the flight dynamics of a quadcopter, complete with procedural audio, day/night cycles, and FPV capability.

**Made by Subham**

## ✨ Features

* **🎮 Real-Time Joystick Support:** Plug-and-play support for Xbox/PlayStation/Generic USB controllers via the Web Gamepad API.
* **⚛️ Physics Engine:** Custom rigid-body physics simulating thrust, gravity, drag, and inertia for a "heavy," realistic flight feel.
* **🔊 Procedural Audio Engine:** Real-time synthesized drone motor sounds that react to throttle input (pitch and volume modulation).
* **🎥 Dual Camera Modes:** Switch instantly between **3rd Person Follow** and **FPV (First Person View)**.
* **📊 Live Telemetry HUD:** Real-time graphing of Throttle, Yaw, Pitch, and Roll inputs.
* **🏙️ Procedural Environment:** Randomly generated cityscapes and forests every time you reload.
* **🌗 Day/Night Cycle:** Toggle between a dark "Night Ops" mode and a bright "Day" mode.

## 🕹️ Controls (Mode 2 Standard)

This simulator follows the standard **Mode 2** transmitter layout used by most real-world FPV and DJI pilots.



| Input | Action | Description |
| :--- | :--- | :--- |
| **Left Stick Y** | **Throttle** | Up to ascend, Down to descend. |
| **Left Stick X** | **Yaw** | Rotate the drone Left or Right. |
| **Right Stick Y** | **Pitch** | Move Forward or Backward. |
| **Right Stick X** | **Roll** | Move Left or Right (Strafe). |
| **Button A (X)** | **Start / FPV** | Launches the drone / Toggles Camera Mode. |
| **Button B (O)** | **Reset** | Resets drone to home position (0,0,0). |
| **Button X (□)** | **Theme** | Toggles Light/Dark mode. |

## 🚀 How to Run

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/MSubham06/drone-simulator.git](https://github.com/MSubham06/drone-simulator.git)
    ```
2.  **Open the Project:**
    Since this project uses ES6 Modules (Three.js), you should run it on a local server to avoid CORS errors.
    * **VS Code:** Right-click `index.html` and select **"Open with Live Server"**.
    * **Python:** Run `python -m http.server` in the terminal and go to `localhost:8000`.
3.  **Connect a Controller:**
    Connect a USB gamepad. Press any button to wake it up. The status light in the HUD will turn **Green**.

## 🛠️ Tech Stack

* **HTML5 / CSS3:** UI Overlay and HUD styling.
* **JavaScript (ES6):** Core logic, physics loop, and DOM manipulation.
* **Three.js:** 3D Rendering, Lighting, and Geometry.
* **Web Audio API:** Oscillator-based engine sound synthesis.
* **Gamepad API:** Hardware input handling.

## 🗺️ Roadmap: Skill Mastery Missions

We are actively developing a campaign mode featuring **10 Specialized Skill Tracks**. Each track is designed to teach a specific aspect of drone flight dynamics using the simulator's physics engine.

### 1. Basic Stabilization & Hover
* **Skill Focus:** Throttle management and micro-adjustments.
* **Operating Area:** **The Training Square** (A 2x2m marked zone on the grass).
* **Mission:** "Hold the Line" - The pilot must maintain the drone's position within the green box for 30 seconds while the simulator introduces randomized wind gusts.

### 2. Precision Landing
* **Skill Focus:** Deceleration inertia and depth perception.
* **Operating Area:** **The Bullseye** (Concentric rings painted on concrete).
* **Mission:** "Touchdown" - Ascend to 20m, fly 50m away, return, and land exactly on the center 'H' marker. Points are deducted for landing speed > 1m/s or drifting off-center.

### 3. Coordinated Turns (Bank & Yank)
* **Skill Focus:** Mixing Yaw (Rudder) and Roll (Aileron) for smooth curves.
* **Operating Area:** **The Slalom Field** (A row of 10 vertical flags).
* **Mission:** "Serpentine" - Weave through the flags in a Figure-8 pattern without stopping. The camera must remain forward-facing (coordinated turn) rather than sliding sideways.

### 4. Gap Shooting (Proximity Flight)
* **Skill Focus:** Spatial awareness and confidence.
* **Operating Area:** **The Construction Site** (Concrete pipes and scaffolding).
* **Mission:** "Thread the Needle" - Fly through a series of narrowing concrete pipes and under low-hanging scaffolding bars. Requires FPV mode.

### 5. Point of Interest (POI) Orbiting
* **Skill Focus:** Multi-axis coordination (Yaw Left + Roll Right + Pitch Forward).
* **Operating Area:** **The Radio Tower** (Center of the map).
* **Mission:** "The Cinematic Shot" - Keep the nose of the drone pointed at the tower while flying a perfect 360° circle around it at a constant altitude.

### 6. High-Speed Racing (Gate Running)
* **Skill Focus:** Pitch management (Forward Velocity) and reflex timing.
* **Operating Area:** **Neon Ring Course** (Floating glowing rings in the sky).
* **Mission:** "Time Attack" - Complete 3 laps of the aerial track. Maintain a pitch angle > 30° to keep speed up while making sharp 180° hairpin turns at the ends.

### 7. Verticality & Elevation
* **Skill Focus:** Throttle punch-outs and free-fall management.
* **Operating Area:** **The Skyscraper District** (Tall city buildings).
* **Mission:** "Rooftop Delivery" - Pick up a package at street level, ascend rapidly up the side of a 50m building, and land on a small AC unit on the roof.

### 8. Structural Inspection (Grid Patterns)
* **Skill Focus:** Slow, methodical movement and stability.
* **Operating Area:** **The Suspension Bridge** (Large red steel bridge).
* **Mission:** "Inspector" - Fly autonomously close to the bridge pillars. The pilot must scan 5 specific rivets (checkpoints) by hovering within 0.5m of them for 3 seconds each.

### 9. Night Operations (Instrument Flight)
* **Skill Focus:** Relying on HUD telemetry over visual cues.
* **Operating Area:** **Blackout City** (Night Mode with zero ambient light).
* **Mission:** "Ghost Recon" - Navigate from Spawn to a lit extraction zone using only the Altimeter and Artificial Horizon on the HUD. Visuals will be limited to drone headlights.

### 10. Cinematic Tracking (Smoothness)
* **Skill Focus:** Eliminating "jerky" stick inputs.
* **Operating Area:** **The Forest Path** (Dense trees).
* **Mission:** "The Dolly Zoom" - Fly backward through a dense forest path at a consistent speed of 2m/s without varying altitude or hitting trees.

## 🔗 Connect

* [**GitHub**](https://github.com/MSubham06)
* [**LinkedIn**](https://www.linkedin.com/in/msubham/)
* [**Instagram**](https://www.instagram.com/irl.subhhh/)

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/MSubham06/drone-simulator/issues).

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
*Created with ❤️ by Subham*
