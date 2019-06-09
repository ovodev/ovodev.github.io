---
layout: post
title: Install Windows Subsystem for Linux on Windows Server
---

This is a summary of documentation that could be found on this link:
[https://docs.microsoft.com/en-us/windows/wsl/install-on-server](https://docs.microsoft.com/en-us/windows/wsl/install-on-server)

1. Enable Windows Subsystem for Linux
```PowerShell
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```