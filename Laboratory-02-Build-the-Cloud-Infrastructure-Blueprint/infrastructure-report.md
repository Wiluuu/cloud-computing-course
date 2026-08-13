# Cloud Server Infrastructure Assessment Report

## Executive Summary
This report outlines the hardware and operating system specifications of the KillerCoda cloud server instance evaluated during the preliminary assessment phase.

## System Specifications

| Metric | System Value | Command Used |
| :--- | :--- | :--- |
| **Hostname** | *(Ilagay ang output ng hostname mula sa KillerCoda)* | `hostname` |
| **Operating System** | *(Ilagay ang OS mula sa cat /etc/os-release)* | `cat /etc/os-release` |
| **Kernel Version** | *(Ilagay ang kernel version)* | `uname -r` |
| **CPU Model** | *(Ilagay ang CPU model)* | `lscpu` |
| **CPU Cores** | *(Ilagay ang CPU cores)* | `lscpu` |
| **Total RAM** | *(Ilagay ang RAM size)* | `free -h` |
| **Disk Capacity** | *(Ilagay ang disk capacity)* | `df -h` |
| **IP Address** | *(Ilagay ang IP address)* | `hostname -I` |

## Mounted File Systems
Below is the output of the file system analysis showing disk utilization and mount points:

```text
Filesystem      Size  Used Avail Use% Mounted on
/dev/root        30G  4.2G   25G  15% /
tmpfs           2.0G     0  2.0G   0% /dev/shm
