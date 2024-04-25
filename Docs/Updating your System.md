## System Packages
You can update your system packages using `paru`. <br/>
Running the command with nothing extra will allow you to update all system packages you have installed on your system.<br/>

## Flatpak
You can update Flatpak from Discover or by running `flatpak upgrade`.<br/>

## Bonus
I have also made an [alias](https://github.com/Mato1111/archguide/blob/main/Docs/General%20Info.md#aliases) that makes updating your system easier. Run the following command to add it:<br/>
```
alias -s up="paru -Syu && echo '----- Updating flatpak -----' && flatpak upgrade"
```
<br/>
Now if you run the command `up`, it will update everything on your system, including Flatpaks.<br/>

---
[Useful Packages and Apps](https://github.com/Mato1111/archguide/blob/main/Docs/Useful%20Packages%20and%20Apps.md)
