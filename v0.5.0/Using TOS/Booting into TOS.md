---
title: "Booting into TOS"
excerpt: "This page will help you get started with booting into TOS. You'll be up and running in a jiffy!"
---
[block:api-header]
{
  "title": "Prepare Disk"
}
[/block]
Download the latest version of TOS GNU/Linux [here](https://tos.pbfp.xyz/downloads).
[block:callout]
{
  "type": "warning",
  "title": "Images",
  "body": "Note that the image used here is the awesome edition. This edition is the fully supported version."
}
[/block]
## Find your usb stick
[block:code]
{
  "codes": [
    {
      "code": "lsblk # before inserting your stick\n#now insert the usb stick\nlsblk # the new entry is your usb stick",
      "language": "shell",
      "name": "list device"
    }
  ]
}
[/block]
## Burn the iso to your usb stick
[block:code]
{
  "codes": [
    {
      "code": "dd if=~/Downloads/toslive-awesome.iso of=/dev/sdb # where sdb is the name of your stick",
      "language": "shell",
      "name": "burn"
    }
  ]
}
[/block]

[block:api-header]
{
  "title": "Boot into TOS GNU/Linux"
}
[/block]
Reboot your system and enter the bios. If you don't know how to use the bios or enter it. Try to search for help online since the procedure depends on the manufacturer of your device.
[block:callout]
{
  "type": "info",
  "title": "Booting into TOS",
  "body": "Pressing F12 or F2 when booting is a common way to enter the bios. It doesn't always work. If it doesn't you will need to search online how to enter your bios (depends on the manufacturer)"
}
[/block]
When you are booting into tos you will see a bootloader. Just select the first option (boot into TOS).
This will start the bootup sequence. After a few seconds/minutes you will be presented with the TOS environment.
[block:callout]
{
  "type": "info",
  "title": "USB speeds",
  "body": "Depending on the type of usb port/key the bootup sequence can take longer. Since older usb's are rather slow."
}
[/block]
When using the awesome edition you will be presented with a tutorial. It is recommended that you follow this tutorial to the letter. For more information about our `awesome` edition please visit the navigation section