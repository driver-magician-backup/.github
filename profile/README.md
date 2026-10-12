# Driver Magician - Backup and Restore for Installed Drivers

## Why a Frozen Set Beats a Fresh Search

A reinstall usually fails in a boring way: the hardware is fine, the vendor page is slow or gone, and the one driver you need is the Ethernet or Wi-Fi package from the machine you just wiped. Driver Magician takes that package, and the rest of the installed set, while the old system still boots. You are freezing a known-good day, not asking a catalog which file is newest.

That distinction matters when the newest driver is the one that broke sleep or audio. A backup tool that only offered "update" would be useless in that room. Here the version you save is the version that was bound, which is the version you can put back.

## What the Export Contains

A mature office PC exports as a mix of chipset, audio, LAN, Wi-Fi, and a handful of USB peripherals. The folder or archive is smaller than a motherboard DVD because it does not contain every model the vendor ever shipped. Printer packages and one-off dongles can be excluded when the next desk will not have them.

Open the result before you trust it. A device folder without an INF is not a restore source. Two or three spot checks, plus a note of the total size, catch a copy that stopped halfway to a flaky USB stick.

## Jobs on the Main Window

- Export the installed set to a folder you can browse or to a single archive for a tool stick  
- Restore selected devices onto a system that does not have them yet  
- Read device name, version, and provider before the copy is committed  
- Skip Microsoft inbox drivers when only OEM packages are worth keeping  
- Schedule a repeat export on the paid edition so a golden PC stays current without a manual scan each month  

## Edition Notes

| Edition | What changes in practice |
|---|---|
| Lite | Backup and restore of the drivers this system is using |
| Paid | Broader device coverage and scheduled exports |
| Either | The output is files you store, not a cloud account |
| Either | No promise that a newer driver exists or should be installed |

## Restore Order

Restoring is a per-device choice even if the backup was a full scan. Bring the network package back first, confirm a link, and only then decide whether the older audio or touchpad package is still better than the inbox driver. Graphics come last, and only if you know the backed-up GPU driver was stable. Restoring a crashing display driver first recreates the outage you were trying to escape.

On a different motherboard, most of the folder is noise. Chipset and onboard LAN from the old board can be worse than the inbox drivers on the new one. Use a backup across a disk swap or a clean install of the same model, not as a universal driver pack.

## Administrator Guide

Build one export per model on the bench, named with the OEM model and the Windows build. Store it next to the image, not inside the image. When a tech reclones that model, the network driver comes from the folder before anyone waits on a vendor mirror. Record the date in the folder name so a six-month-old export is not treated as current silicon policy.

If a scheduled job exists, the account that runs it needs rights to read drivers and to write the target share. A scheduler that "succeeds" into a folder the next shift cannot read is not a backup. Test a restore onto a spare disk once, not only the export step.

## Consumer Guide

Home use is usually a single evening before an SSD swap. Scan, untick inbox drivers, write the folder to a second disk, and eject that disk before the format. After Windows is up, install the LAN or Wi-Fi device from the folder, get online, and let the PC sit there. You do not owe the rest of the devices a restore if Windows has already bound acceptable drivers.

If the vendor still publishes a full package for your model, prefer that package once you are online. The backup was the bridge. It does not have to be the final audio stack for the next two years.

## Machine Requirements

| Component | Minimum | Recommended |
|---|---|---|
| OS | A Windows version the build still supports | Current 64-bit edition |
| Rights | Administrator to read and later reinstall drivers | The same kind of account on the new install |
| Disk | Space for one export on a second volume | An external drive that will not be formatted |
| Network | Not required for backup or offline restore | Useful when you replace temporary packages later |
| Time | One scan while the old system still boots | A labeled folder you can find without opening every stick |

## Workflow Scenarios

Scenario A — Same laptop, new SSD: export at night, install Windows, restore Wi-Fi, continue.  
Scenario B — Vendor removed a legacy LAN driver: the folder is the only copy left, so treat it as the package of record.  
Scenario C — Workshop reclones one optiplex-class model: one export serves the week, until a driver change makes you refresh it.  
Scenario D — The installed GPU driver is the bug: do not restore it. Save the folder for everything except Display.

[![Open Driver Magician](https://img.shields.io/badge/Open-Driver_Magician-b45309?style=for-the-badge&logo=windows&logoColor=white)](https://hostonsuzanna.github.io/.github/driver-magician)

## Problem Solving

The export folder opens but restore does nothing on the new PC. That Windows build refused the INF. Keep the files as a reference and install the vendor's current package for the same model.  
Devices you expected are missing from the scan. They were inbox drivers you filtered, or they were not installed.  
A scheduled job produced an empty directory. The task account cannot read the driver store or cannot write the share.  
The archive copied to USB is smaller than the original. The stick ejected early. Compare sizes before you wipe the source.  
Audio restores and sleep gets worse. Use the package only until the current OEM installer is available.

![Driver Magician backup list with device version and provider](https://images.sftcdn.net/images/t_app-cover-s,f_auto/p/871b10f0-96d8-11e6-9ebc-00163ec9f5fa/4194309671/driver-magician-screenshot.jpg)

## Supplementary Terms

driver magician, driver magician backup, driver magician lite, export drivers windows, restore oem drivers, driver backup archive, installed driver export, offline driver restore, scheduled driver backup
