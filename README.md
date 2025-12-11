SerixOS

A lightweight, modular Linux-based OS layer designed to run on top of Debian/Ubuntu systems.
SerixOS provides:

Unified command support for Debian, Ubuntu, and SerixOS custom tools.

Auto-branding (Neofetch + /etc/os-release).

Optional Web UI available at port 3000 when installed on VPS/VM.

Optional desktop interface when installed on physical hardware (planned).

Features
✓ Cross-Distro Command Support

SerixOS maintains compatibility with major Linux bases:

Works on Debian 10+

Works on Ubuntu 20.04+

✓ Web Interface (Port 3000)

If SerixOS detects it is running in a VPS/VM environment, it launches a web dashboard at:

http://<server-ip>:3000


The dashboard includes:

File explorer

App launcher

“Store” to download packages

System info panel (CPU, RAM, disk details)

✓ Branding Layer

SerixOS automatically:

Modifies /etc/os-release

Adds custom ASCII logo (crescent moon)

Injects SerixOS theme into neofetch

Installation
1. Download the installer
git clone https://github.com/pro-samanyu/SerixOS
cd SerixOS

2. Run the installer
sudo bash serix.sh


The script:

Detects Debian/Ubuntu

Installs required packages

Applies SerixOS branding

Sets up web interface (Node.js or Python) on port 3000

Reboots the system

SerixOS Commands
System Commands
Command	Description
serix --version	Show installed SerixOS version
serix --fetch	Show SerixOS neofetch-style logo
serix --repair	Repair OS branding & components
serix --reinstall-webui	Reinstall/repair port-3000 web interface
serix --check-environment	Detect if running on VPS/PC
