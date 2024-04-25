Some apps will require tinkering when you install them.

One of the applications I had to tinker with to get it working correctly is xdg-desktop-portal-gtk.
I use it to sync my system theme with browsers, but its also used as a file picker for when you upload files.
I hate the file picker. With a burning passion. Luckily, it can be disabled.

To disable the file picker, follow these steps:
1. Run  `sudo micro /usr/share/xdg-desktop-portal/portals/gtk.portal`
2. On line 3, remove `org.freedesktop.impl.portal.FileChooser;` (including the semi-colon)
3. Save the file

---
[Useful Application Launch Options](https://github.com/Mato1111/archguide/blob/faddade510de20d9b827b5734581aee4b6d1569f/Docs/Useful%20Application%20Launch%20Options.md)
