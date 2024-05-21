## System Packages
System packages, or just packages, are the main way that apps, drivers, and utilities are installed on a Linux system. Arch Linux uses `pacman` as it's package manager. I will be using `paru` to install packages through pacman.

For example: `paru vivaldi` will search for packages with a name or description containing "Vivaldi." You can then select then which package you want by typing in the number(s) next to the name(s) and hitting enter. <br/>

When installing something from the AUR, it will show you the `PKGBUILD` file. This is a safety feature that lets you review the install script before running it, just in case its trying to something crazy, such as removing the home directory. To get past this preview/wall of text, press `q`, then `enter`.<br/>
 
If it says that 2 packages are conflicting and asks if you want to remove the old one, type "y" and hit enter ONLY if you actually want to replace the old package with the new one you are installing. If this happens during an update, it should be okay to just hit enter, as `Y` should be the default option and it is most likely being replaced by a newer version of the package, but under a different name.<br/>

Using `paru -S <package-name>`, you can install any specific package that you already know the name of and you wont have to pick from a list of options.<br/>

For example `paru -S spotify`. This will install Spotify directly without showing you a long list of other options.<br/>

To uninstall packages, run `paru -R <package-name>`<br/>

## Flatpaks
Flatpaks are an alternative way of installing apps on Linux. These are usually installed from Flathub, which you can access by opening Discover from the application launcher. <br/>
They are generally easier to install and use for new users, and are the default on immutable distros.<br/>

To install a Flatpak, just open Discover, search for the app you want to install, and click the install button.<br/>

The reason I don't personally use Flatpaks is because they often need extra configuration using `Flatseal` in order for stuff like system theming and cursors to apply. This has gotten better over time, and isn't an issue for a lot of apps. In fact, I use the Flatpak for OBS.<br/>

---
[Updating your System](https://github.com/Mato1111/archguide/blob/main/Docs/Updating%20your%20System.md)
