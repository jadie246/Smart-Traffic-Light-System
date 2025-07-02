# 🚦 Smart Traffic Light System in C

This project simulates a **smart traffic light system** using the C programming language. It features:

- A normal red-yellow-green light cycle.
- Emergency vehicle detection using randomized probability.
- Dynamic override to green light when an emergency is detected.

---

## 📌 Features

- ⏱ Simulated timing using `Sleep()` from `windows.h`
- 🎲 Randomized emergency detection using `rand()` with floating-point range
- 💡 Clear output showing current light state
- 🔁 Infinite loop to simulate a real-time traffic light system

---

## 🧠 How It Works

- The light cycles through:
  - 🔴 Red for 5 seconds
  - 🟢 Green for 5 seconds
  - 🟡 Yellow for 2 seconds
- Every cycle, the system generates a random float in the range [0.0, 1.0]
- If the generated value is less than **0.2 (20%)**, it assumes an **emergency vehicle is approaching**
- The system **immediately overrides the cycle**, turning the light green for 5 seconds
