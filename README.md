# Linux Default Apps
A script to install some applications on new debian-based Linux installations.

The script install:
* Google Chrome - Browser
* DBEaver - Database manager for multiples DBMS
* Visual Studio Code
* Yakuake - Quake style terminal
* Git - source control tool
* Python
* Transmission - Torrent client
* vim - Text editor
* PostgreSQL - Open source database
* VLC - Media player

The script removes:
* Firefox

---

Google Chrome:
* sudo apt-get install libxss1 libappindicator1 libindicator7
* wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
* sudo apt install -y ./google-chrome*.deb

DBEaver:
* wget https://dbeaver.io/files/dbeaver-ce_latest_amd64.deb
* sudo apt install -y ./dbeaver-ce_latest_amd64.deb

Visual Studio Code
* sudo apt install -y software-properties-common apt-transport-https wget
* wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
* sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
* sudo apt update
* sudo apt install -y code

GIT
* sudo apt install -y git

Transmission
* sudo apt install -y transmission

PostgreSQL
* sudo apt install -y postgresql

Yakuake
* sudo apt install -y yakuake


---
How to use

Just run ./main.sh.
This script will execute all others scripts in applications directory.








