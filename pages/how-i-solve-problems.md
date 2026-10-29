# How I Solve Problems

[← Back to home](../README.md)

### The Challenge
During a ESP Lesson with Pete, I Had issues with Solid State Drives not showing up on our Workstations when trying to add them to a storage pool.
### What We Did to Fix It
First I checked the connections of the sata and power to the drives to ensure they are plugged in correctly, after this I moved onto looking if they were being recognized in DISKPART and Disk Management which they were.
At this point I have checked if the drive is present physically and recognized. The next course of action in to see what is on the drive which could be the reason why it is not being detected in the Windows Server Software, which was precisely the issue. After getting to this point i went ahead and clean/formatted the drives to NTFS which made them recognized in the software. This also has made the reason why the drives were not showing up at the clear. It was because these drives had previously had another type of format on them which made them recognized but not everywhere or usable.

### Looking Back at it Now
I should have skipped looking at the cables but I did anyways which wasted time but apart from that checking if they were recognized and then performing a format on the drives seems like a reasonable approach to this problem.
