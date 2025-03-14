# Raspian OS Installation on Surface 2

This repository provides a guide for flashing Raspian OS on a Surface 2 device (an almost obsolete device). **Warning:** This process will completely wipe all data on the device’s EMMC.

## Prerequisites

- **Two USB Drives Required:**
  - **First USB Drive:** To flash the image.
  - **Second USB Drive:** To be inserted after the first reboot. It must contain the extracted image (without the `.xz` compression) directly in the root folder.
- **Preferably USB 2.0:** For better compatibility, it is recommended to use USB 2.0 drives instead of USB 3.0.
- **FAT32 Formatting:**
  - The second USB drive **must** be formatted as FAT32.
  - **Note:** On Linux, FAT32 formatting can behave differently; it is advisable to format this drive on a Windows system.

## Procedure

1. **Download the Image**
   - Obtain the Surface 2 EMMC RPIOS Installer image from the following link:  
     [Surface 2 EMMC RPIOS Installer](https://files.open-rt.party/Linux/Distro/rpi-bookworm-bootable-usb-winpe-installer-surface2.img.xz)

2. **Flash the Image to the First USB Drive**
   - Use a tool such as Rufus (or a similar utility) to write the image to the first USB drive.
   - Flashing the image will create two partitions: one for boot and one for root.

3. **Boot the Surface 2**
   - Insert the flashed USB drive into your Surface 2 and power on the device.
   - The system will load the image and, after the boot process is complete, the device will automatically reboot.

4. **Insert the Second USB Drive**
   - After the reboot, insert the second USB drive.
   - This drive, formatted as FAT32, should contain the extracted image (i.e., the image file without the `.xz` extension) in its root directory.

5. **Install Raspian OS**
   - The device will boot from the second USB drive and proceed with the installation of Raspian OS.

## Jailbreak Tools

- Jailbreak tools (such as "golden keyes" and "yahsallo") are readily available online.
- Follow the specific instructions to install these tools and complete the Surface 2 jailbreak.

## Important Notes

- The semi-automatic installation system for Linux on Surface 2 is based on ARM32 and Tegra 4.
- **Open Surface RT Projects:** For more information and related projects, visit the [Open Surface RT Projects](https://opensurfacert.org/) website.
- Please note that the Discord channel is no longer available. This change is one of the reasons this semi-automatic Linux installation system was created.

---

Contributions, issue reports, and feedback are welcome.
ig : dario.corona_
