# Analysis-of-the-Disk-Structure-using-Sleuth-Kit
### Reg no: 212222100024
### Name: LOKESH RAHUL V V
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
![WhatsApp Image 2025-05-22 at 17 57 09_9701cb78](https://github.com/user-attachments/assets/1c772fe8-7481-4d66-9d4d-2b0cca70b22a)
## Create Disk
![image](https://github.com/user-attachments/assets/d6785ef2-0c56-407c-9acf-d81b77070a81)
### mmls
```
mmls disk.dd
```

### fls
```
fls -f fat -o 0 disk.dd
```
![WhatsApp Image 2025-05-22 at 17 53 37_17e3a1b7](https://github.com/user-attachments/assets/e7dfa92c-f864-4f57-a217-84371b7ccba8)

## RESULT:
The analysis was performed successfully using Sleuth Kit, and the disk structure was understood in detail.
