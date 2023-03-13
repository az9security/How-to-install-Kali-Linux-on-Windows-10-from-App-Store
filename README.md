# How-to-install-Kali-Linux-on-Windows-10-from-App-Store



=====Commands=====



-----INSTALL WSL 2----- 
1. RUN POWERSHELL as administrator 
2. Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
-----RESTART-----
3. dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart 
4. dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart 
-----RESTART-----
5. Download Linux Kernel - https://docs.microsoft.com/en-us/wind... 
-----SET DEFAULT TO WSL 2-----
6. wsl --set-default-version 2 
-----INSTALL GUI-----
7. sudo apt update && sudo apt upgrade -y 
8. sudo apt install kali-desktop-xfce -y 
-----Setup XRDP-----
9. sudo apt install xrdp -y 
10. sudo service xrdp start

