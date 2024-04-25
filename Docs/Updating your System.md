## System Packages
You can update your system packages using `paru`. 
Running the command with nothing extra will allow you to update all system packages you have installed on your system.

## Flatpak
You can update Flatpak from Discover or by running `flatpak upgrade`.

## Bonus
I have also made an [[General Info#^f37034|alias]] that makes updating your system easier. Run the following command to add it: ^c900d4
```
alias -s up="paru -Syu && echo '----- Updating flatpak -----' && flatpak upgrade"
```

Now if you run the command `up`, it will update everything on your system, including Flatpaks.

---
[[Useful Packages and Apps]]