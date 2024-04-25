Some apps will require tinkering when you install them.

One of the applications I had to tinker with to get it working correctly is xdg-desktop-portal-gtk.<br/>
I use it to sync my system theme with browsers, but its also used as a file picker for when you upload files.<br/>
I hate the file picker with a burning passion. Luckily, it can be disabled.

To disable the file picker, follow these steps:
1. Run  `sudo micro /usr/share/xdg-desktop-portal/portals/gtk.portal`
2. On line 3, remove `org.freedesktop.impl.portal.FileChooser;` (including the semi-colon)
3. Save the file.

It should now look like this:
```
[portal]
DBusName=org.freedesktop.impl.portal.desktop.gtk
Interfaces=org.freedesktop.impl.portal.AppChooser;org.freedesktop.impl.portal.Print;org.freedesktop.impl.portal.Notification;org.freedesktop.impl.portal.Inhibit;org.freedesktop.impl.portal.Access;org.freedesktop.impl.portal.Account;org.freedesktop.impl.portal.Email;org.freedesktop.impl.portal.DynamicLauncher;org.freedesktop.impl.portal.Lockdown;org.freedesktop.impl.portal.Settings;
UseIn=gnome
```

# Clearing your Cache
If you're ever running out of storage space, chances are your pacman/paru cache is taking up a good amount of that space. To clear it, follow these steps:
1. Run `paru -Sc`
2. "Yes, no, yes, no". You want to answer the 4 questions in that order. This will remove cached files, but not remove important repos.

---
[Useful Application Launch Options](https://github.com/Mato1111/archguide/blob/main/Docs/Useful%20Application%20Launch%20Options.md)
