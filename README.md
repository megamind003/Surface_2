# Surface_2
Flash and Install the rasperri os Image on (jailbroken) Surface 2 (NOT RT)



# Surface 2 RPIOS Installer

This repository provides a method to flash RPIOS Bookworm onto a Surface 2 device. **Use this method at your own risk.** The process will install RPIOS Bookworm to the internal EMMC and **completely wipe all existing data**.

## Prerequisites

- **Two USB Drives Required:**  
  - **Installer USB:** Contains the RPIOS Bookworm installer image.  
  - **Resizer USB:** Used to resize the EMMC partitions after installation.
- **Preferably USB 2.0:** For better compatibility, use USB 2.0 drives instead of USB 3.0.
- **FAT32 Formatting:**  
  - The resizer USB must be formatted as FAT32.
  - **Important:** On Linux, FAT32 formatting can differ. It is recommended to format this USB drive on a Windows system in FAT32.

## Installation Steps

1. **Download the RPIOS Installer Image**
   - Get the installer image from:  
     [Surface 2 EMMC RPIOS Installer](https://files.open-rt.party/Linux/Distro/rpi-bookworm-bootable-usb-winpe-installer-surface2.img.xz)
   
2. **Prepare the Installer USB Drive**
   - Use a tool such as Rufus (or an equivalent) to write the downloaded image to the installer USB drive.
   - Boot your Surface 2 from this USB drive.
   - The installer will automatically write RPIOS Bookworm to the internal EMMC.
   - **Warning:** This step will erase all data on the EMMC.

3. **Download and Prepare the Partition Resizer Tool**
   - After the installation completes, download the partition resizer tool from:  
     [Surface 2 Linux Resize Partition Tool](https://files.open-rt.party/Linux/Other/surface-2-linux-resizepart-emmc.zip)
   - Extract the contents to the resizer USB drive (which must be formatted in FAT32 as specified above).

4. **Resize the EMMC Partitions**
   - Boot your Surface 2 using the resizer USB drive.
   - The tool will automatically adjust the EMMC partitions to fit the device's actual storage size.

## Important Notes

- **Data Loss Warning:** The entire process will erase all data on your Surface 2's EMMC. **Back up any important data before proceeding.**
- **USB Drive Requirements:** Use two separate USB drives (preferably USB 2.0) as detailed above.
- **Formatting Caution:** Ensure the resizer USB is formatted as FAT32 on a Windows system to avoid compatibility issues that might arise with Linux formatting.

## Disclaimer

This method is provided "as is" without any warranty. The author is not responsible for any data loss or hardware damage resulting from the use of this tool.

---

Feel free to contribute, report issues, or provide feedback.
