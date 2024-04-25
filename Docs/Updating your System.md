## System Packages
You can update your system packages using `paru`. 
Running the command with nothing extra will allow you to update all system packages you have installed on your system.

## Flatpak
You can update Flatpak from Discover or by running `flatpak upgrade`.

## Bonus
I have also made an [alias](https://github.com/Mato1111/archguide/blob/main/Docs/General%20Info.md#aliases) that makes updating your system easier. Run the following command to add it:
```
alias -s up="paru -Syu && echo '----- Updating flatpak -----' && flatpak upgrade"
```

Now if you run the command `up`, it will update everything on your system, including Flatpaks.

---
[Useful Packages and Apps](https://github.com/Mato1111/archguide/blob/main/Docs/Useful%20Packages%20and%20Apps.md)
