# Port Scanner Script

A lightweight, zero-dependency Bash script to scan a range of TCP ports on a target IP address or domain using Bash's built-in `/dev/tcp`.

## Usage

Run the script in Bash shell (Linux, macOS, WSL, or Git Bash on Windows):

```bash
bash port_scanner.sh <TARGET> <START_PORT> <END_PORT>
```

### Example

To scan ports 20 to 85:

```bash
bash port_scanner.sh scanme.nmap.org 20 85
```

### Output Example

```
Scanning scanme.nmap.org from port 20 to 85...
Port 22 is OPEN
Port 80 is OPEN
Done!
```

## Requirements

- **A Bash shell environment:**
  - **Linux / macOS:** Pre-installed by default in the system terminal.
  - **Windows:** Requires **Git Bash** (comes with [Git for Windows](https://git-scm.com/downloads)) or **WSL (Windows Subsystem for Linux)**. *(Does not run in Windows Command Prompt or PowerShell).*
- **No external packages required** (does not need `netcat` or `nmap` installed).

## Notes

- Some ports might be blocked by a firewall.
- Ensure your script filename matches the command (e.g., `port_scanner.sh` or `scan.sh`).

## License

This script is free to use and modify.
