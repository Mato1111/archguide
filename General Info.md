## File Structure
The Linux file structure is a bit different from Windows.
All of your user data is stored in the `/home/username/` folder. 
Most settings are stored in the `/home/username/.config/` folder. When you make changes to app settings, or if you to change the "config file" for an app, you'll likely find it located in that folder. 

## Sudo
When using the terminal, some commands may ask for a 'sudo' password. This is the same as giving admin permissions on Windows, but requires a password.

## Y/N
When you are asked a yes or no question in the terminal, the upper case letter is the default option and you can just hit enter to select it.
Example: `Y/n` hitting enter without typing anything will select Yes.  `y/N` hitting enter = No.

## Aliases
^f37034
Aliases are useful tools for the terminal that help automate certain tasks or just make them simpler. An example can be found [[Installing Packages#^c900d4|here.]]

Some built in aliases include:
`~` is to your user/home folder. (Ex: cd ~/Pictures = cd /home/username/Pictures)
`.` is the current directory. (Ex: cd ./Wallpapers = cd /home/username/Pictures/Wallpapers)
`..` is one directory up. (Ex: cd .. = cd /home/username/Pictures)

## Text Editing
Text editing can be done from the terminal if needed. 
The most common way of doing this is with `nano`, but I prefer `micro`, as it is easier to use coming from other GUI based text editors with similar keybindings.

You can install `micro` by running the command `yay -S micro`. in a terminal window. This is pretty much required if you want to fully follow this guide.

---
[[CachyOS Repos]]
