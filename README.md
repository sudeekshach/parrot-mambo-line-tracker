# 🛸 Line-Tracking with Parrot Mambo Drone (Simplified Vision-Based Control)

## 📘 Project Summary

This project demonstrates how a **Parrot Mambo mini drone** can autonomously follow a visual path using a **simple line-tracking algorithm** built in **MATLAB Simulink**. The drone uses its **downward-facing camera** to detect a line on the ground (like tape) and adjusts its direction to stay on track — without using GPS or complex mapping.

This is a **simplified version** of a more advanced model developed by Paolo Ceppi in his master's thesis. The goal of this project is to provide a working prototype that is **easy to understand, simulate, and extend** for educational or research purposes.

---

## 🎥 Demo Video

See the simplified line-following behavior in action:

👉 [Watch Demo on YouTube](https://youtu.be/7tgiYd_LUkM) *(replace this with your real link)*  
📁 Or view the included demo in the repo.

---

## 📂 What's Included

- A fully working **Simulink model** (`.slx`) for the line-following controller
- Image processing block to detect a line using **color thresholding**
- Path planning using **Stateflow logic**
- A **demo video** showing the drone in simulation
- A ZIP package with everything you need to run the model
- Reference to the original thesis that inspired this project

---

## 💾 Full Implementation Package

You can download the complete Simulink model, image processing files, and supporting scripts from:

📁 [`ParrotMambo_Simplified_Tracking.zip`](./ParrotMambo_Simplified_Tracking.zip)

After downloading, extract the ZIP and open the `.slx` file inside with MATLAB Simulink. Follow the setup instructions in the `README.txt` included in the ZIP for dependencies and simulation steps.

---

## 📦 How to Use the Project

### Requirements:

- **MATLAB** (preferably R2020a or later)
- **Simulink**
- **Computer Vision Toolbox**
- **Simulink Support Package for Parrot Minidrones**

### Steps:

1. Download and extract the ZIP file:  
   📁 `ParrotMambo_Simplified_Tracking.zip`

2. Open the `.slx` file inside using MATLAB.

3. Load or replace the camera input image (if simulating).

4. Run the simulation in **Model-in-the-Loop (MIL)** mode.

5. Observe how the drone tracks the path and turns based on what it sees.

---

## ⚙️ Key Parameters

| Parameter                | Description                    | Value                      |
|--------------------------|--------------------------------|----------------------------|
| `vel`                    | Drone speed constant           | `4.5e-4`                   |
| `z`                      | Altitude during flight         | `1.1 m`                    |
| Image Sub-region - Left  | Area for left pixel count      | Rows `1–39`, Cols `1–55`   |
| Image Sub-region - Right | Area for right pixel count     | Rows `1–39`, Cols `103–157`|
| Pixel Threshold          | Trigger to decide turning      | `140`                      |

---

## 🧠 Project Purpose

- To demonstrate how a **low-cost drone** can follow a path using **basic image processing**
- To provide a **teaching tool** for control systems, Simulink modeling, and robotics
- To show how **complex research** can be simplified for **practical implementation**

---

## 📚 Attribution

This project is inspired by and adapted from the thesis:

> Ceppi, P. (2020). *Model-based Design of a Line-tracking Algorithm for a Low-cost Mini Drone through Vision-based Control* (Master's thesis). University of Illinois at Chicago.

We thank Paolo Ceppi for the original model and approach. This version simplifies the system for educational use and faster simulation.

---

## 🛡️ License

This project is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

You are free to:

- **Share** — copy and redistribute the material  
- **Adapt** — remix and build upon the material for any purpose  

As long as you give **appropriate credit**.

---

## 📬 Contact

📧 Email: [sudeekshach@gmail.com]  
🔗 LinkedIn: [https://www.linkedin.com/in/sudeeksha-chagarlamudi/](https://www.linkedin.com/in/sudeeksha-chagarlamudi/) 

---
