# STA Timing Report Analysis (Dummy)

This repository demonstrates my understanding of Static Timing Analysis (STA) by analyzing a dummy timing report and explaining how to fix setup and hold violations.

## 🔧 Setup Violation Example

**Path:** REG_A (launch) → REG_B (capture)  
**Violation:** Slack = -0.6ns

### 🧠 How to Fix
- Increase clock period
- Reduce data path delay (optimize logic or placement)
- Add pipeline register in long path
- Improve clock tree skew (use clock latency balancing)

## 🧠 STA Concepts

### Reg-to-Reg Path
- A sequential timing path where data is launched from a **flip-flop register** on one clock edge and captured by another register on the next edge.

### Slack
- Slack = Required Time − Arrival Time
- **Negative slack** indicates a timing violation.

## 📊 Visualization

**Timing Diagram for Setup Violation:**

![Timing Diagram](reg-reg_path_diagram)


## 📁 Files
- `dummy_sta_report.txt` – Sample report
- `README.md` – Analysis and fixes


## ✨ Future Work
- Add hold violation example
- Script to parse timing report and highlight violations
