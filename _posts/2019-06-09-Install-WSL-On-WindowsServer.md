---
layout: post
title: Install Windows Subsystem for Linux on Windows Server
---

Here's the steps that I have taken to install WSL. This is like a summary of the documentation that could be found on this [link](https://docs.microsoft.com/en-us/windows/wsl/install-on-server).

1. Enable Windows Subsystem for Linux

```PowerShell
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```

2. Restart you machine.

3. Download a linux distribution of your choice. You can see the guide [here](https://docs.microsoft.com/en-us/windows/wsl/install-manual).

4. Rename the downloaded linux distro from <distro-name>.appx to <distro-name>.zip.

```PowerShell
Rename-Item .\Ubuntu.appx .\Ubuntu.zip
```

5. Unzip the package to your desired installation folder location.

```PowerShell
Expand-Archive .\Ubuntu.zip .\Ubuntu
```

6. Run the distro luncher. The launcher the executable file found inside installation folder and named <distro-name>.exe.
  
7. You can then add the the distro installation folder to the Windows environment path.

```Powershell
$userenv = [System.Environment]::GetEnvironmentVariable("Path", "User")
[System.Environment]::SetEnvironmentVariable("PATH", $userenv + "C:\Users\Administrator\Ubuntu", "User")
```
