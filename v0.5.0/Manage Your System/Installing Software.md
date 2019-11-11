---
title: "Installing Software"
excerpt: ""
---
In order for you to use your system you need to know how to install software. The basics will be covered here. In case you need to know more you can always look up pacman [wiki](https://wiki.archlinux.org/index.php/Pacman)
[block:api-header]
{
  "type": "basic",
  "title": "Tos package manager"
}
[/block]
Open up a terminal and type in the following
[block:code]
{
  "codes": [
    {
      "code": "tos -Ss <query> # where query is the application to lookup",
      "language": "shell",
      "name": "bash"
    }
  ]
}
[/block]
You will get a reply containing all matches to your query. Find the correct application name and the type the following
[block:code]
{
  "codes": [
    {
      "code": "tos -Syu <name> # where name is the name of your application.",
      "language": "shell",
      "name": "bash"
    }
  ]
}
[/block]
Lets take a look at a simple example.
We will be trying to install gimp.  For those who don't know what gimp is. Its a editor for picutres much like photoshop.
[block:code]
{
  "codes": [
    {
      "code": "tos -Ss gimp # gimp will most likely be named gimp\n>extra/xsane-gimp 0.999-3 (248.1 KiB 772.0 KiB)\n>    XSane Gimp plugin\n>extra/xsane 0.999-3 (1.5 MiB 4.8 MiB)\n>    A GTK-based X11 frontend for SANE and plugin for Gimp.\n>extra/potrace 1.16-1 (85.0 KiB 246.0 KiB) (Installed)\n>    Utility for tracing a bitmap (input: PBM,PGM,PPM,BMP; output: >EPS,PS,PDF,SVG,DXF,PGM,Gimppath,XFig)\n>extra/gimp 2.10.14-1 (18.9 MiB 104.3 MiB) (Installed)\n>    GNU Image Manipulation Program\n\ntos -Syu gimp # install gimp",
      "language": "shell",
      "name": "bash"
    }
  ]
}
[/block]
As we can see above the package is named gimp `extra/gimp 2.10.14-1 (18.9 MiB 104.3 MiB) (Installed)` We can see that it is inside the `extra` repository and that the download size is `18.9MiB` with an install size of `104.3MiB`
[block:callout]
{
  "type": "info",
  "title": "Mastering the package manager is very powerfull",
  "body": "You can do much more. For example see what is already installed, update your system, remove packages and more."
}
[/block]

[block:api-header]
{
  "title": "Keep your system up to data"
}
[/block]
All you need to do is run `tos -Syu` often enough to keep your system up to date
[block:callout]
{
  "type": "danger",
  "title": "Update",
  "body": "It is important that you update frequently. Since tos is a rolling release distribution you will need to update at least once a week otherwise your updates will become very large."
}
[/block]