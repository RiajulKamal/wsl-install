# Simple wsl Installation process in windows machine
:point_right: ### Step 1: Enable WSL in Windows 10
For enable WSL in Windows 10, just open PowerShell as an administrator and run the following command:
##
    dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
:point_right: ### Step 2: Install WSL in your Windows machine
Now install WSL, just open a new PowerShell window as an administrator and run the following command:
##
    wsl --install
:point_right: ### Step 3: Set WSL 2 as Default
You have to set WSL 2 as the default version of WSL,for this just open PowerShell as an administrator and run the following command:
##
    wsl --set-default-version 2
:point_right: ### Step 4: Now Install Kali Linux
To install Kali Linux, you just run the following command in a PowerShell window:
##
    wsl --install -d kali-linux




# Now if you want to Install GUI

:point_right: ### Step 5: Update Your PC
To update your PC, You just run following command in kali:

##
    sudo apt update && sudo apt upgrade -y

:point_right: ### Step 6: Install GUI
For install GUI or desktop environment, just run following command in kali:

##
    sudo apt install kali-desktop-xfce -y

:point_right: ### Step 7: Install XRDP
To run desktop environment, you need to install xrdp using following command:

##
    sudo apt install xrdp -y

:point_right: ### Steo 8: Start GUI using RDP
To start GUI service using RDP, just use the following command:

##
    sudo service xrdp start
