### Disk Partition and Format Instructions

Follow these steps to partition and format a disk using PowerShell or Command Prompt:

1. Hold the `Windows` key and press `X`, then select **PowerShell (Admin)**. Confirm by selecting **Yes** to the pop-up.
   You can also use **Command Prompt**.( Hold the `Windows` key and press `R`, **Run** dialog box opens,
   type `cmd` and press `ctrl` + `shift` + `enter`  to open **Command Prompt** in admin mode )
3. In the PowerShell interface, type `diskpart` to enter the disk partition tool.
4. Type `list disk`. This command will list the hard drives installed on the machine. Pay close attention not to choose the wrong hard drive.
5. Type `select disk X`, replacing `X` with the number of the solid state drive/ usb drive you want to format.
6. Type `clean` to remove all partitions and data on the selected disk.
7. Type `create partition primary` to create a new primary partition on the disk.
8. Type `list part` to list the partitions of usb (Most likely you will have a single partition).
9. Type `select partition 1` to select the partition you just created.
10. Type `active` to mark the partition as active.
11. Type `format fs=ntfs quick` to format the partition using the NTFS file system.
12. Type `assign` to assign a drive letter to the partition.
13. Type `exit` to leave the disk partition tool.
14. Type `exit` again to close the PowerShell or Command Prompt window.

> **Warning:** Ensure that you select the correct disk, as this process will erase all data on the selected drive.
