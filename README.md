# First Time Install repo
Checklist for installing and configure a device with my tools and preferences.

### Chocolatey
Install chocolatey to automate the installation of most apps.

**command:**
`Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))`

### Chocolatey script for basic apps
Script for automation of installation of the apps below

### Browsers
- Chrome
- Brave
- Firefox

### Chat
- Discord
- Whatsapp
- Telegram

### Utils
- 7Zip
- Adobe Reader
- Silverlight
- .Net Framework
- Google Backup and Sync

### Media Players
- VLC Player
- Spotify
- Twitch

### Dev Tools
- Notepad ++
- Git
- Visual Studio Code
- Python 3.9
- NodeJS
- Fluent Terminal

### Break Reminder
- Stretchly

**Command:**
`choco install googlechrome brave firefox discord whatsapp twitch telegram 7zip adobereader silverlight dotnetfx google-backup-and-sync vlc spotify notepadplusplus git vscode python nodejs fluent-terminal stretchly --yes`

### GPO and Windows settings
Script to automate the GPO changes and windows settings listed below:
- Disable Proxy
- Disable Cortana
- Hide search bar
- Disable Update delivery optimization
- Add and set the ultimate performance power profile
- Hide Desktop Icons
- Disable UAC

**Command:**
`$URI = "https://raw.githubusercontent.com/bignacio-vega/first_time_install/main/systemConfig.ps1"
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString($URI))`

### Windows Store Apps
Install the Apps listed below from the Windows Store
- Notepads
- TransculentTB
- Microsoft Remote Desktop

### Install the Ubuntu Subsystem
Script to Install the Ubuntu Subsystem for Linux
**Command:**
`dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart

dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart

Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi'))

wsl --set-default-version 2`


