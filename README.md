<h1 align="center">
  <a href=https://www.archlinux.org/>Archlinux</a> System Automated Installer (ASAI)
</h1>
<h4 align="center">Easing Installation & Configuration of Archlinux</h4>
<p align="center">
  <img src="https://img.shields.io/badge/Maintained%3F-Yes-green?style=for-the-badge">
  <img src="https://img.shields.io/github/license/mfgbhatti/asai?style=for-the-badge">
  <img src="https://img.shields.io/github/issues/mfgbhatti/asai?color=violet&style=for-the-badge">
  <img src="https://img.shields.io/github/stars/mfgbhatti/asai?style=for-the-badge">
  <img src="https://img.shields.io/github/forks/mfgbhatti/asai?color=teal&style=for-the-badge">
</p>

---

### Note
* You can first try it in a `VirtualMachine`

### Prerequisites

- A working internet connection
- Logged in as 'root'
## Create Arch ISO or Use Image

Download ArchISO from <https://archlinux.org/download/> and put on a USB drive with [Etcher](https://www.balena.io/etcher/), [Ventoy](https://www.ventoy.net/en/index.html), or [Rufus](https://rufus.ie/en/)

## Download ASAI
You can clone
```
git clone https://github.com/mfgbhatti/asai

```
then
```
cd asai
./asai
```
## Features
ASAI offers the following:
### Partition Layouts
1. btrfs
2. LVM
3. LVM + LUKS
4. Use user already existed boot and root partitions

#### Btrfs Subvolume
ASAI allows users to customize subvolume names and numbers.

### Variety of Filesystems
ASAI is offering these file systems
1. Btrfs
2. Ext2
3. Ext3
4. Ext4
5. F2fs
6. Jfs
7. Nilfs2
8. Ntfs
9. Vfat
10. Xfs

### Desktop Env or Desktop Managers
Asai offers these mainline DEs or DMs
1. Gnome
2. KDE
3. XFCE
4. Mate
5. LXQT
6. Minimal
7. Awesome
8. OpenBox
9. I3
10. I3-Gaps
11. Deepin
12. Budgie

### Bootloaders
In addition to Grub, ASAI offers
- Systemd boot
- EFISTUB

### Kernel Selection
You can select from 
1. linux
2. linux-lts
3. linux-zen
4. linux-hardened
---

## Troubleshooting

__[Arch Linux Installation Guide](https://github.com/rickellis/Arch-Linux-Install-Guide)__

### No Wifi

You can check if the WiFi is blocked by running `rfkill list`.
If it says **Soft blocked: yes**, then run `rfkill unblock wifi`

After unblocking the WiFi, you can connect to it. Go through these 5 steps:

#1: Run `iwctl`

#2: Run `device list`, and find your device name.

#3: Run `station [device name] scan`

#4: Run `station [device name] get-networks`

#5: Find your network, and run `station [device name] connect [network name]`, enter your password and run `exit`. You can test if you have internet connection by running `ping google.com`, and then Press Ctrl and C to stop the ping test.

## Credits
- This is a fork of [ArchTitus](https://github.com/ChrisTitusTech/ArchTitus) by [Chris Titus Tech](https://github.com/ChrisTitusTech).
