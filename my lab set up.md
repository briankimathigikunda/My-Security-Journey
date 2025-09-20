# My-Security-Journey
# My Home Lab Setup Guide

## Objective
To create a safe, isolated environment for practicing ethical hacking and penetration testing techniques.

## Hardware & Software
*   **Host Machine:** MacBook Pro (2020, M1)
*   **Virtualization Software:** UTM
*   **Guest VMs:** Kali Linux, Ubuntu Server, Windows 10/11

## Network Configuration
I set up a **Host-Only Network** in UTM to isolate my VMs from my main network but allow them to communicate with each other.

## Step-by-Step Installation
1.  **Downloaded Kali Linux ISO:** [I got it from the official Offensive Security website.](https://www.kali.org/get-kali/)
2.  **Created a New VM in UTM:**
    *   Selected `Virtualize` -> `Linux`
    *   Allocated 4 GB RAM and 2 CPU Cores
    *   Created a 50 GB disk image stored on my external "HOT-LAB" drive
    *   Mounted the Kali ISO and installed the OS
3.  **Post-Installation Setup:**
    *   Ran `sudo apt update && sudo apt full-upgrade -y`
    *   Installed essential tools: `git`, `python3`, `pip3`

## Lessons Learned
*   Using UTM on Apple Silicon is much faster than VirtualBox.
*   Allocating VM storage to an external drive keeps my main laptop fast.

## Future Upgrades
*   Integrate a vulnerable web app (OWASP Juice Shop).
*   Configure a Windows target VM.
