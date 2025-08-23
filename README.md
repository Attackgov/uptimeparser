# 🕒 Uptime Parser by Attack

A Windows monitoring tool that checks the uptime and status of specific services and processes.  
It detects restarts, delayed starts after system boot, and missing processes/services - updating the console in real time with colored output.

---
## 📋 Patchnotes
- **[+]** Ignores delayed services caused by late startup

## ✨ Features
- 🔒 **Admin check** – Auto-restarts with elevation if not run as administrator  
- 🖥️ **Monitors services & processes** – Configurable list of system-critical components  
- ⏱️ **Uptime tracking** – Reports how long each service/process has been running  
- 🚨 **Detection system** – Flags missing, restarted, or late-started services/processes  
- 🎨 **Colored console output** – Easy-to-read real-time table  
- 🔄 **Auto-refresh** – Console view updates every second  

---

## 📌 Monitored Targets (Default)
- **Services:**  
  `dps`, `dnscache`, `sysmain`, `pcasvc`, `diagtrack`, `eventlog`, `bam`  
- **Processes:**  
  `explorer.exe`

---

## 🛠️ Requirements
- Windows 10/11  
- Administrator privileges (auto-requested if not elevated)  
- Console environment (CMD or PowerShell)  

---

## 🚀 Usage
1. Run the executable.  
2. If not elevated, the program will request admin privileges.  
3. The console displays a live status table of monitored services/processes.  

**Detection messages include:**  
- `<name> not running`  
- `<name> started after boot`  
- `<name> Restarted`  

---

## 📖 Notes
- System uptime is displayed at the bottom of the console.  
- Program runs continuously until manually closed.  
- Screen refreshes every second to keep output clean.  

---

## 👤 Author
**Attack**
