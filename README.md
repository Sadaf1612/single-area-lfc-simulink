# Single-Area Load Frequency Control (LFC) using Simulink

This project simulates a basic Load Frequency Control (LFC) system for a single-area power grid in MATLAB Simulink. The model shows how frequency deviates in response to a sudden load disturbance and how a manual PID controller can restore system stability.

This project was completed as a guided learning exercise using Onramp modules and simulation support.

---

## 🎯 Objective

To simulate a closed-loop frequency control system using basic Simulink blocks and demonstrate how PID feedback can bring the frequency deviation (Δf) back to zero after a load disturbance.

---

## 🧰 Tools Used

- MATLAB Simulink 
- Manual PID Controller (built using Gain, Integrator, Derivative blocks)
- Transfer Function Model for power system dynamics
- Scope block for frequency deviation visualization

---

## 🧱 Model Components

- **Step Load Disturbance**: Simulates sudden load increase (0.01 pu)
- **Transfer Function**: Models system response (`1 / (10s + 1)`)
- **Manual PID Controller**: Adjusts control action based on frequency error
- **Feedback Loop**: Constant reference (0) and frequency deviation compared using a Sum block
- **Scope**: Plots frequency deviation over time

---

## ⚙️ PID Gain Values

- **Proportional (P)**: 5  
- **Integral (I)**: 2  
- **Derivative (D)**: 0.5

These values were tuned manually to ensure the frequency returned to nominal smoothly and quickly.

---

## 📈 Output

The system response shows a frequency drop at time = 0 due to the step load, followed by a smooth recovery as the PID controller stabilizes the system.

![Scope Output](scope_output.png)

---

## 📁 Files Included

- `single_area_lfc.slx` – Simulink model file  
- `scope_output.png` – Screenshot of simulation result  
- `README.md` – This documentation

---

## ✍️ Author

Sadaf Tanvir  
Electrical and Electronics Engineering Student  
Guided self-project using MATLAB & Simulink

---

## 📜 Notes

This project was completed as a beginner-level simulation to build understanding of power system dynamics and control fundamentals.
