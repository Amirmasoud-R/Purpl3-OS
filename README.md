# Purpl3 OS

![4](https://github.com/user-attachments/assets/f8dd1f07-cd7b-431a-a6b1-fc581a1a7415)

## History

Purpl3 OS Linux development started in Q2 2023 after spending some time at the Islamic Azad University Karaj Branch computer laboratory, I have noticed that the students and my mentor Dr. Harifi were having serious problems with the computers due to the extremally outdate hardware even Ubuntu 16.04 was not working properly. I suggested the idea of developing a distro from scratch as my final project to Dr. Harifi, They agreed but insisted on having the core of Ubuntu so I decided to modify the core of Ubuntu 20.04 LTS and make it as optimized as possible even for the lowest spec systems with modern interface at the same time. The development of Purpl3 OS finished in the Q3 2023 and immediately I upgraded all of the computers in the lab with Purpl3 OS, thus finally solving the lab problems once and for all.

Purpl3 OS was chosen as the best project for the Fall semester of 2023 at Islamic Azad University Karaj Branch.

I was also awarded a certifiaction of apperication for upgrading and improving the lab computers at October of 2023.


## Editions

- **Purpl3 OS** (Standard Home Edition)

- **KIAU Edition** (Extra optimized for the low spec hardware in Islamic Azad University Karaj Branch lab computers)

## Live Mode Credential

**Username:** username

**Password:** password

## Features

- Lightweight
- Ram optimizations
- CPU optimizations
- Storage optimizations
- Network optimizations
- GRUB optimizations
- User friendly
- Custom Terminal
- Modern and custom UI
- Easy GUI installation
- Live preview mode ability
- Comes in 2 variant of Home and Lab editions
- Comes with set of useful preinstalled packages
- Contains Doom I & II
- Contains awesome Eastereggs :)
- (try these commands: easteregg - purpl3 - harifi)
- (for more goodies go to the easteregg folder located at /user/share/EasterEgg)

## Optimizations

1) In order to improve the performance of the CPU frequency range has been changed intel_pstate to acpi-cpufreq by default.

2) The BIOS frequency limitation has been disabled by default in order to improve the performance of the CPU frequency range.

3) In order to improve the performance of the hard disk and boot time, the watchdog has been disabled by default.

4) Improving the performance of the hard disk by changing the I/O scheduler for SATA, HDD, and NVMe disks.

5) Improved CPU performance by changing the default kernel scheduler to a Linux-zen kernel.

6) Improving network and Internet performance by changing the Bottleneck Bandwidth and Round-trip propagation time (BBR).

7) Improved RAM memory function by changing the randomize_va_space status.

8) Improved virtual memory performance by replacing zswap instead of swap by default.

9) The hardware threads (physical CPU) for each CPU core have been enabled.

10) Improving the paralleling of tasks by allowing independent tasks (running threads) by sharing some processor resources.

11) Changed power saving mode to performance mode by default, in order to improve the performance of the disk and network IO.

12) All CPU governor frequency has switched in performance.

13) Reducing kernel log-level reports to a low level in order to improve kernel performance and increase security and create silent boot mode.

14) and also, improving TCP performance, increasing inode cache memory, disk cache, improving network and bandwidth parameters, etc.

15) Improved Blacklist for better system service optimizations.

## Known Issues

​
Due to networking issues present in some systems. There might be slow downs in boot up.

The slow downs are caused by services that might require internet connection or networking to function.​
The obvious one, like

``NetworkManager-wait-online.service.``


To fix them, manual intervention is required.

First we identify the services that cause that slow down.

``sudo systemd-analyze blame``


Then we mask them from starting in boot.

``sudo systemctl mask NetworkManage​r-wait-online.service``

