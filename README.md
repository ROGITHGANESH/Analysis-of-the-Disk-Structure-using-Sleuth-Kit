# Name:ROGITH GANESH.R
# REGISTER NUMBER: 212223100046
# Analysis-of-the-Disk-Structure-using-Sleuth-Kit
## AIM:
To analyze the disk structure of a given disk image using Sleuth Kit tools in Kali Linux.

## DESIGN STEPS:
### Step 1:
Obtain or create a disk image file (e.g., disk.dd) to analyze. Open the terminal in Kali Linux.

### Step 2:
Use Sleuth Kit tools like mmls, fsstat, and fls to examine the partition layout, file system details, and file listing.

### Step 3:
Interpret the output of the tools to understand the disk structure, including partitions, sectors, and files.

## PROGRAM:
Sleuth Kit Disk Analysis Commands
✅ Option 1: Create a Sample Disk Image (for Testing)

Let’s create a 10MB blank disk image and simulate file system activity:

```
cd ~/Downloads

# Step 1: Create an empty disk image
dd if=/dev/zero of=disk.dd bs=1M count=10

# Step 2: Format it with a file system (like FAT32)
mkfs.vfat disk.dd
```
## OUTPUT:

![WhatsApp Image 2025-04-25 at 03 44 28_0f130355](https://github.com/user-attachments/assets/750dfe6f-a567-43bc-bab5-4999c469fb8e)

# Create Disk:
![image](https://github.com/user-attachments/assets/f14771ed-58db-4ca8-b256-7ab9ea42ea47)

# mmls
```
mmls disk.dd
```
# fls
```
fls -f fat -o 0 disk.dd
```
![image](https://github.com/user-attachments/assets/b8cabdf9-9c6a-488f-855a-9231bd161b66)
![image](https://github.com/user-attachments/assets/86647ad5-d612-4f44-9e5f-d5fe10cca69e)



## RESULT:
The analysis was performed successfully using Sleuth Kit, and the disk structure was understood in detail.
