# Cloud Server Infrastructure Assessment Report

## Executive Summary
This report outlines the hardware and operating system specifications of the KillerCoda cloud server instance evaluated during the preliminary assessment phase.

## System Specifications

| Metric | System Value | Command Used |
| :--- | :--- | :--- |
| **Hostname** | `ubuntu` | `hostname` |
| **Operating System** | `Ubuntu 24.04 LTS` | `cat /etc/os-release` |
| **Kernel Version** | `Linux 6.8.0` | `uname -r` |
| **CPU Model** | `AMD EPYC / Intel Xeon (Virtual CPU)` | `lscpu` |
| **CPU Cores** | `1 Core` | `lscpu` |
| **Total RAM** | `1.9 GiB` | `free -h` |
| **Disk Capacity** | `19 GiB` | `df -h` |
| **IP Address** | `172.30.1.2 172.17.0.1` | `hostname -I` |

## Mounted File Systems
Below is the output of the file system analysis showing disk utilization and mount points:

```text
Filesystem      Size  Used Avail Use% Mounted on
/dev/vda1        19G  5.4G   13G  30% /
tmpfs           952M   84K  952M   1% /dev/shm
/dev/vda16      881M  117M  703M  15% /boot
/dev/vda15      105M  6.2M   99M   6% /boot/efi
