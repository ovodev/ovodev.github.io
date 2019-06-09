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

4. Rename the download linux distro from <distro-name>.appx to <distro-name>.zip.
  ```PowerShell
  Rename-Item ~/Ubuntu.appx ~/Ubuntu.zip
  Expand-Archive ~/Ubuntu.zip ~/Ubuntu
  ```
