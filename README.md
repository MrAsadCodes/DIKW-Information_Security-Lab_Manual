# Lab 1 – DIKW Framework

## Walkthrough Task
This lab demonstrates the **DIKW Framework** (Data → Information → Knowledge → Wisdom) and applies it to security logs.

### Process
- **Data**: Raw log entries stored in `auth.log`.
- **Information**: Structured output generated using `walkthrough.py`.
- **Knowledge**: Identifying suspicious activity such as multiple failed login attempts = brute-force attack.
- **Wisdom**: Taking action:
  - Block IP with iptables
  - Restrict log file permissions
  - Generate SHA-256 hash for file integrity

### Files
- `auth.log` → simulated login attempts
- `walkthrough.py` → Python script to parse logs
- `README.md` → notes for Lab 1

### Commands Used
- Restrict file permissions (Confidentiality):
  ```bash
  chmod 600 auth.log
