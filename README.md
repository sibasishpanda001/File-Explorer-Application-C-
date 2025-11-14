# File-Explorer-Application-C-
Here is a clean, professional, GitHub-ready README.md for your System Monitor Tool (C++) project — with proper formatting, sections, tables, emojis, and screenshot placeholders.

You can copy–paste directly into your repository.


---

🖥️ System Monitor Tool (C++)

A lightweight real-time System Monitor written in C++17, inspired by the Linux top command.
It displays live information about CPU usage, memory usage, running processes, and allows interactive process control using an ncurses UI.

This project was built progressively over 5 days, with one major feature added each day.


---

⭐ Features

✅ Display system uptime, memory usage, and load average

✅ List running processes with CPU and memory metrics

✅ Sort processes by CPU or memory usage

✅ Kill processes interactively (SIGTERM or SIGKILL)

✅ Real-time refresh like top

✅ Ncurses-based interactive UI

🔄 Smooth real-time updates every few seconds



---

🎯 Project Objective

Objective:
Build a C++ system monitoring tool that behaves similarly to the Linux top command—showing real-time CPU/memory usage and providing process-level control.


---

📅 Day-wise Progress

Day 1 — UI Layout & System Data

Displayed uptime, load average, and memory details.


Day 2 — Process Listing

Listed running processes, CPU jiffies, and RSS memory usage.


Day 3 — Sorting Feature

Added sorting by CPU or memory:

--sort=cpu

--sort=mem



Day 4 — Process Control

Added interactive kill:

k — SIGTERM

K — SIGKILL



Day 5 — Real-Time Ncurses UI

Full ncurses interface

Real-time CPU % calculation

Live refresh + keyboard controls



---

🛠️ Installation

Prerequisites

Linux system

C++17 compiler (g++)

Ncurses library


Install Ncurses (Ubuntu/Debian)

sudo apt update
sudo apt install g++ libncurses-dev


---

🔧 Build & Run

Build (Day-5 final version)

g++ -std=c++17 sysmon.cpp -o sysmon -lncurses

Run

./sysmon 2

➡️ Refreshes every 2 seconds
➡️ Press q to exit


---

🎮 Usage Controls

Keyboard Commands

Key / Command	Function

s	Toggle sorting (CPU ↔ Memory)
k	Prompt PID → kill process (SIGTERM)
K	Prompt PID → force kill (SIGKILL)
q	Quit program


CLI Options

Argument	Description

--sort=cpu	Sort by CPU (default)
--sort=mem	Sort by memory


Example:

./sysmon --sort=mem


---

📘 Git Commit Log (Example)

git init
git add sysmon.cpp
git commit -m "Day 1: Basic UI layout and system info"
git commit -m "Day 2: Process listing with CPU jiffies and memory"
git commit -m "Day 3: Added sorting by CPU/memory"
git commit -m "Day 4: Interactive process kill functionality"
git commit -m "Day 5: Real-time ncurses-based system monitor"


---

🖼️ Screenshots

> 📌 (Upload your actual images in the repository and replace the placeholders below.)



Day 1 – Basic System Info

![Day1 Output](screenshots/day1.png)


---

Day 2 – Process Listing

![Day2 Output](screenshots/day2.png)


---

Day 3 – Sorted Process List

![Day3 Output 1](screenshots/day3-1.png)
![Day3 Output 2](screenshots/day3-2.png)


---

Day 4 – Process Kill Feature

![Day4 Output 1](screenshots/day4-1.png)
![Day4 Output 2](screenshots/day4-2.png)
![Day4 Output 3](screenshots/day4-3.png)


---

Day 5 – Real-Time Ncurses Monitor

![Day5 Output 1](screenshots/day5-1.png)
![Day5 Output 2](screenshots/day5-2.png)
![Day5 Output 3](screenshots/day5-3.png)
![Day5 Output 4](screenshots/day5-4.png)


---

📄 License

This project is released under the MIT License.


---

👨‍💻 Author

Hiranmaya Panda
Final Year B.Tech (Computer Science)
Passionate about backend development, system programming, system design, C++ & Java.


---

If you want, I can also:
✨ Add stylish GitHub badges
✨ Add ASCII logo or banner
✨ Generate a PDF version of this README

Just tell me!
