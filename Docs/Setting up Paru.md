Paru is a better way to install packages to your system. Install Paru with `yay -S paru`, assuming you already have `yay`. If not, you can install `paru` by following [these instructions.](https://github.com/Morganamilo/paru?tab=readme-ov-file#installation) <br/>

Now run the command `sudo micro /etc/paru.conf`.<br/>
If micro is not installed, install it with `sudo pacman -S micro`<br/>
Next, remove the hashtag in front of the lines that say `BottomUp`, `SudoLoop`, `CombinedUpgrade`, and `UpgradeMenu`. This will make it behave more like `yay`, which is a bit more user friendly (for me at least). <br/>
You can now save it with `ctrl+s` and quit with `ctrl+q`. <br/>

---
[Installing Packages](https://github.com/Mato1111/archguide/blob/main/Docs/Installing%20Packages.md)
