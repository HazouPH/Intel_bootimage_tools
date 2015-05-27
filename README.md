Intel bootimage tools

Intel bootimage tools for the Razr I. This set of tools let u extract and pack a bootimage in linux. I used them often to just change some small settings in the ramdisk to test rather then compile the whole bootimage again through source.

What can be done with this package:
- Change the content of the ramdisk
- Change the kernel that's inside
- Change recoveryimage and it's content and kernel

What do the directory's mean:

- Kernel: the kernel directory contains the extracted kernel from the current used boot.img.
- Ramdisk: the ramdisk directory contains 3 things:
-- 'modify' directory which contains the content of the extracted ramdisk
-- 'ramdisk' file is the extracted ramdisk from the current boot.img
-- 'modifiedramdisk' file is the recompiled ramdisk from the 'modify' folder
- Tools: the tools directory contains the actual extracting and packing tools

How to use:
Extracting:
- Put a boot.img (with that name "boot.img") in the root of the intel bootimage tools directory.
- Execute the script: 'extract' by double-clicking or by terminal
- The extracted kernel can be found in the kernel directory, the ramdisk and its content can be found in the ramdisk directory

Packing
- When done the changed u want (e.g. changing kernel image, changing ramdisk content), execute 'create'
- A new bootimage will be created with the name: 'Modifiedboot{date-time}.img'
