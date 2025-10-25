# SysSnap
## Linux System & Network Management Script

A dumb dialog-based bash shell script to manage system updates, Snap packages, and network/system information.


### 📋 Main Menu
```
├── 0) Show Disk Space
├── 1) System Info
│    ├── 1) Memory Usage
│    ├── 2) CPU Info
│    ├── 3) System Load
│    └── 4) Back
├── 2) Network Tools
│    ├── 1) Check Public IP
│    ├── 2) View Active Connections
│    ├── 3) Show Local IPs
│    └── 4) Back
├── 3) Get Updates
├── 4) Install updates
├── 5) Show All Snap Versions
├── 6) Remove Disabled Snaps
├── 7) Empty Snap Cache Directory
└── 8) Exit
```

### 🗂️ Menu Options

* Show Disk Space – Displays disk usage of the main filesystem.
* System Info – Opens a submenu for memory, CPU, and system load info.
* Network Tools – Opens a submenu for public IP, active connections, and IPs for all active network profiles.
* Get Updates – Scans for available APT package updates and closes.
* Install updates - Select to update individual or all available updates from the list.
* Show All Snap Versions – Lists installed Snap packages (excluding disabled ones).(If snap is found)
* Remove Disabled Snaps – Cleans up disabled Snap versions.(If snap is found)
* Delete Snap Cache – Shows cache size and allows deletion.(If snap is found)
* Exit – Closes the script.

### ⚙️ Requirements

* dialog package installed
* nmcli (NetworkManager CLI) for network info
* curl (for public IP)
* sudo privileges for system updates