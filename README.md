<h1 align="left">💻HP 14-r010tu Hackintosh</h1>

<hr>

This repository and project hosts the files necessary to boot for the HP 14-r010tu laptop running macOS Monterey.

>[!WARNING]
**EFI only works on macOS Monterey and not on higher versions.**

>[!NOTE]
**Currently conducting tests on the Sequoia version.**

>[!WARNING]
**NOT SURE WORK OR TESTED ON OTHER LAPTOP/DESKTOP**

<hr>

### 📃DISCLAIMER:
THIS INFORMATION/RESEARCH HAS BEEN DONE AND SHARED PURELY FOR EXPERIMENTAL AND RESEARCH PURPOSES, AND IS IN NO MAY MEANT TO PROMOTE CIRCUMVENTING OF ANYTHING THAT IS SOMEONE ELSE'S CORPORATE PRIVATE PROPERTY. THE INFORMATION LISTED HERE IS PURELY FOR EDUCATIONAL PURPOSES AND SHOULD YOU CHOOSE TO UTILIZE IT IN ANY WAY, I AM IN NO WAY RESPONSIBLE FOR ANY INJUNCTIONS/PROBLEMS THAT MAY OR MAY NOT ARISE AND/OR BE BROUGHT AGAINST ANOTHER FOR THEIR CHOOSING TO HAVE DONE SO.

<hr>

### 😇Acknowledgements:

- Acidanthera for [OpenCore Bootloader](https://github.com/acidanthera/OpenCorePkg)

- Dortania for [OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)

- Corpnewt for [SSDT Time](https://github.com/corpnewt/SSDTTime)

- USBToolbox for [USBToolbox](https://github.com/USBToolBox)

- And many awesome people in the hackintosh community!

<hr>

### Download:

[**EFI Monterey**](https://github.com/Thebinhdx/Hackintosh-HP14-r010tu/blob/main/EFI.7z)

[**EFI Sequoia** (Memory Panic Stackshot](https://drive.google.com/file/d/19IJIkK5WoACoarBayHbA0EIQbfx4Xt6A/view?usp=sharing)

>[!NOTE]
**I need help fixing EFI Folder for Sequoia!**

>[!NOTE]
**Once you have the EFI folder, you need to go into config.plist and edit the serial number, ROM, UUID, etc., to be different from the original. Save the changes and place them in your EFI partition so you can boot into macOS.**

<hr>

<details>
<summary><strong>Hardware specifications:</strong></summary>

<br />

| Components      | Name                               | Brand Links                       |
| --------------- | -----------------------------------| ----------------------------------|
| **CPU**         | Intel® I5-4210U                    | Intel                             |
| **IGPU**        | Intel® HD 4400                     | Intel                             |
| **RAM**         | DDR3 4GB / 1600MHz                 | Unknown                           |
| **Storage**     | 224GB SSD (Replace old HDD 500GB)  | Kingston                          |
| **Ethernet**    | Realtek PCIe FE Family Controller  | Realtek                           |
| **Audio**       | Realtek High Definition Audio      | Realtek                           |
| **Wifi**        | Ralink RT3290 (NOT SUPPORTED)      | Mediatek                          |
| **SD**          | Realtek PCIE CardReader            | Realtek                           |
| **Camera**      | HP Truevision HD                   | ?                                 |
| **CDROM**       | ?                                  | ?                                 |

**NOTE: Change wifi card with intel card like AX210, AC 7260, ...**

</details>

<details>
<summary><strong>Problem:</strong></summary>

<br />

**Note: This is only available if you haven't made too many deep modifications to my config.plist.**

## Monterey:

### 💡Backlight issues:

- The backlight will dim when the Apple logo appears. Even with the toggle switch, it won't work unless you put the computer to sleep and wake it up, then it will return to normal.
- If you want to use it, change the `platform-id` to `0A026006`. Besides the trade-offs, you'll experience lag with 4MB of graphics card usage and you won't be able to adjust the brightness, although it will turn on instantly when you use it.

## Ventura and Newer:

**Note: EFI Folder is in testing.**

-Currently encountering the error `In Memory Panic Stackshot succeeded`. I will try to find a way to fix it.

</details>
