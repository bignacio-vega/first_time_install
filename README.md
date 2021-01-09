# First Time Install repo
Checklist for installing and configure a device with my tools and preferences.

# Chocolatey
Install chocolatey to automate the installation of most apps.

command:
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

# Chocolatey script for basic apps
Script for automation of installation of the apps below

# Browsers
- Chrome
- Brave
- Firefox

# Chat
- Discord
- Whatsapp
- Telegram

# Utils
- 7Zip
- Adobe Reader
- Silverlight
- .Net Framework
- Google Backup and Sync

# Media Players
- VLC Player
- Spotify

# Dev Tools
- Notepad ++
- Git
- Visual Studio Code
- Python 3.9
- NodeJS
- Fluent Terminal

Command:
choco install googlechrome brave firefox discord whatsapp telegram 7zip adobereader silverlight dotnetfx google-backup-and-sync vlc spotify notepadplusplus git vscode python nodejs fluent-terminal --yes
