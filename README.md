# ZenOptimize

**ZenOptimize** is a lightweight Windows optimization tool focused on improving gaming performance, responsiveness, and system consistency.  
It safely applies tuning adjustments and includes a full structured backup/restore system.

<p align="center">
  <a href="https://ko-fi.com/sidfps" target="_blank">
    <img src="https://ko-fi.com/img/githubbutton_sm.svg" alt="Support me on Ko-fi">
  </a>
</p>

> **Note:** The PowerShell source code is private. Only the compiled binary is distributed publicly.

---

## 🚀 Features (v1.1 – Enhanced Gaming Experience)

### 🎮 Core Gaming Optimizations
- **Windows Game Mode** – Automatically enables for optimal resource allocation
- **Hardware-Accelerated GPU Scheduling (HAGS)** – Reduces latency on supported GPUs (auto-detected)
- **Gaming performance adjustments**:
  - SystemProfile responsiveness tuning
  - SystemProfile\Tasks\Games CPU/GPU priority tweaks
- **Disable GameDVR & GameBar** (lower overhead / input latency)

### 🔕 Distraction-Free Gaming
- **Focus Assist & Notification Suppression** – Prevents interruptions during gameplay
- **Xbox Services Optimization** – Disables non-essential services while preserving controller support

### 🌐 Network Optimizations
- Auto-detect active network adapter
- TCPNoDelay, TcpAckFrequency optimization for lower latency

### ⚡ System Performance
- **Visual effects performance mode**
- **Limit background UWP apps** for better gaming performance
- Explorer/Search optimization (DisableSearchBoxSuggestions)

### 🛡 Safety & Reliability
- Automatic **Administrator elevation** (seamless, no manual intervention)
- **Comprehensive logging** (ZenOptimize.log) for troubleshooting
- **Structured backup** of all modified registry values
- Full **Restore Defaults** feature (type-aware restoration)
- Interactive restart prompt when system restart required (HAGS)

### 🎨 User Experience
- Simple interactive menu (Apply / Restore)
- Clear step-by-step progress indicators
- Clean status messages and branding

---

## 📦 Downloads
Get the latest **ZenOptimize.exe** from the Releases section.

📁 Current binary:
`ZenOptimize_v1.1.exe`

---

## 🛠 How to Use
1. Download the latest EXE from Releases  
2. Run as **Administrator**  
3. Choose:  
   - **[1] Apply Optimizations**  
   - **[2] Restore Defaults**

---

## 📄 Documentation
- **CHANGELOG.md** — version history  
- **ROADMAP.md** — upcoming versions  
- **LICENSE.md** — usage rights for v1.x  

---

## 🔐 Source Code
The optimization logic (`.ps1` source) is **not included** in this repository.  
ZenOptimize is currently distributed as a **binary-only utility**.

---

## 🛡 Security & Privacy
ZenOptimize modifies system registry values.  
Use responsibly and always read the documentation before applying changes.

---

## ❤️ Support the Project
If you find ZenOptimize helpful, consider supporting further development:

<p align="center">
  <a href="https://ko-fi.com/sidfps" target="_blank">
    <img src="https://ko-fi.com/img/githubbutton_sm.svg" alt="Support me on Ko-fi">
  </a>
</p>

---

## 💬 Feedback / Issues
Open an issue on GitHub to report bugs or suggest improvements.
