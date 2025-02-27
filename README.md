# WSL-Installation
**Requirements: Windows 10 version 2004 and higher (Build 19041 and higher) or Windows 11(type and click on winver at the search bar to find your windows version)**
1. You must first enable the "Windows Subsystem for Linux" optional feature before installing any Linux distributions on Windows.

2. Open PowerShell as Administrator (Start menu > PowerShell > right-click > Run as Administrator) and enter this command:

```PowerShell
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```  
and:

```PowerShell
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

3. After running this command restart your machine

4. Install ubuntu from the following [link](https://apps.microsoft.com/detail/9NZ3KLHXDJP5?hl=en-us&gl=GR&ocid=pdpshare)

5. From the distribution's page, select "Download".

The first time you launch a newly installed Linux distribution, a console window will open and you'll be asked to wait for a minute or two for files to de-compress and be stored on your PC. All future launches should take less than a second.

6. You will then need to create a user account and password for your new Linux distribution

    * Once the process of installing your Linux distribution with WSL is complete, open the distribution (Ubuntu by default) using the Start menu. You will be asked to create a User   Name and Password for your Linux distribution.

    * This User Name and Password is specific to each separate Linux distribution that you install and has no bearing on your Windows user name.

    * Please note that whilst entering the Password, nothing will appear on screen. This is called blind typing. You won't see what you are typing, this is completely normal.

    * Once you create a User Name and Password, the account will be your default user for the distribution and automatically sign-in on launch.

    * This account will be considered the Linux administrator, with the ability to run sudo (Super User Do) administrative commands.

    * Each Linux distribution running on WSL has its own Linux user accounts and passwords. You will have to configure a Linux user account every time you add a distribution, reinstall, or reset. 

7. Finally, go to Powershell, open as administrator and run the following commands:

```PowerShell
wsl --update
```
```PowerShell
wsl --set-default-version 2
```
```PowerShell
wsl --set-default Ubuntu-24.04
```
