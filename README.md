# SimDial AI: official downloads

This repository publishes the **official customer downloads of SimDial AI**, a phone system for a USB LTE modem on a Windows PC. It answers and places calls, lets an AI voice agent talk on them, can hand a call to a person, runs outbound campaigns, handles SMS and records calls, all from a local web dashboard.

It contains **release files only**. There is no source code here.

## Download

Go to the [**Releases**](../../releases) page and download the setup program of the version you want, for example `SimDialAI-Setup-0.1.8.exe`.

## Before you run the setup program

1. **Check the checksum.** Each release lists the SHA-256 of its setup program and ships a `SHA256SUMS.txt`. In PowerShell:
   ```powershell
   Get-FileHash .\SimDialAI-Setup-0.1.8.exe -Algorithm SHA256
   ```
   The result must be identical to the value published with the release. If it differs, do not run the file.
2. **Windows SmartScreen.** Setup programs are not code-signed yet, so Windows may show "Windows protected your PC". If the checksum matches, choose **More info**, then **Run anyway**.
3. **The modem driver is not included.** Install the Windows driver from your modem's maker first.

## Requirements

- Windows 10 or Windows 11, 64-bit.
- A supported USB LTE voice modem and a SIM card with voice service.
- For the AI voice agent: your own accounts and API keys for the speech and language providers you choose.

## Installing and updating

SimDial AI installs for the current Windows user and does not ask for administrator rights. Your data is kept on the drive you choose during setup. To move to a newer version, download its setup program and run it. Read the notes of each release: they state exactly what was tested and what is known to be missing, including whether automatic in-app updates are available for that version.

## About this repository

Releases are published here by SIZH IT Solutions. Release notes describe what changed and the known limitations of each version.
