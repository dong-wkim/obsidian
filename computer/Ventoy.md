---
title: README
aliases:
tags:
  - computer
---
**Goal**: Set up triple OS (Windows, Linux, macOS) live-boot from USB with a shared drive to access files, apps and documents to use on three operating systems. 

## Create live triple-boot from USB drive

- [x] install Ventoy onto USB Drive
- [x] download and copy over Windows 11 LTSC 2024 (windows_11_ltsc_2024.iso)
- [ ] download and copy over Linux (TailsOS, Ubuntu, Debian-Med)
- [ ] install macOS using hackintosh
- [x] install Windows 11 LTSC 2024 using Ventoy

## Set up for Windows

- [x] download and install Lenovo Software Drivers
- [x] install Chocolatey 
- [x] install Google Drive
- [x] install Microsoft Office LTSC 2024

```powershell

Set-ExecutionPolicy AllSigned
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
choco feature enable -n allowGlobalConfirmation
choco install googlechrome
choco install googledrive

```

## Set up for Linux