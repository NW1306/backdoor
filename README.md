# Windows Remote Access & Keylogger (For Educational Use Only)

> ⚠️ **Disclaimer:** This project is intended strictly for educational purposes and should only be used in lab environments or with explicit permission from the system owner. Unauthorized access to devices is illegal and unethical.

## Overview

This project demonstrates the basics of remote access tools (RATs) and keylogging on a Windows machine, designed for learning about how attackers might compromise systems. It emphasizes the importance of securing your systems against such techniques.

Components

1. `server.py`
- Acts as the control center (attacker’s machine).
- Accepts incoming connections from a client.
- Allows file upload/download, command execution, and screenshot capture.
- Integrates keylogger control functions.

2. `keylogger.py`
- A Python-based keylogger script for Windows.
- Logs keystrokes to a file located in the `AppData` directory.
- Can be started, dumped, and stopped via commands from `server.py`.

 Features

- Remote shell command execution
- File upload/download
- Screenshot capture
- Keylogger control (start, dump, stop)
- Basic persistence setup via registry (educational example)

Usage (In a Controlled Environment)

 Server (Attacker Machine)
```bash
python server.py
