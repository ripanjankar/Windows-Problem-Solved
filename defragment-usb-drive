# Disk Partition and Format Instructions

Follow these steps to partition and format a disk using PowerShell or Command Prompt:

1. Hold the `Windows` key and press `X`, then select **PowerShell (Admin)**. Confirm by selecting **Yes** to the pop-up. You can also use **Command Prompt**.
2. In the PowerShell interface, type `diskpart` to enter the disk partition tool.
3. Type `list disk`. This command will list the hard drives installed on the machine. Pay close attention not to choose the wrong hard drive.
4. Type `select disk X`, replacing `X` with the number of the hard drive you want to format.
5. Type `clean` to remove all partitions and data on the selected disk.
6. Type `create partition primary` to create a new primary partition on the disk.
7. Type `select partition 1` to select the partition you just created.
8. Type `active` to mark the partition as active.
9. Type `format fs=ntfs quick` to format the partition using the NTFS file system.
10. Type `assign` to assign a drive letter to the partition.
11. Type `exit` to leave the disk partition tool.
12. Type `exit` again to close the PowerShell or Command Prompt window.

> **Warning:** Ensure that you select the correct disk, as this process will erase all data on the selected drive.
