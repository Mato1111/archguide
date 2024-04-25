All of these options require you to add `%command%` at the very end of the launch options, but before game-specific options.
Example: `ALSOFT_DRIVERS=ALSA gamemoderun gamescope -f --force-grab-cursor -s 0.5 %command% -nojoy -novid -threads 12`

## IMPORTANT!!!
 **Use [ProtonDB](https://www.protondb.com/dashboard) to check if a game will work on Linux and if any changes need to be made for it to work.**
 Some games require different launch options, and some need a specific version of Proton. An example is Garry's Mod, which only works well after forcing Proton Experimental, setting a specific launch option, and applying the [codec fix.](https://github.com/solsticegamestudios/GModCEFCodecFix)

## Options
`gamemoderun`
When gamemode is installed to the system (`paru -S gamemode`), adding this to launch options allows the game to apply optimizations that can result in better performance.

`gamescope -f --force-grab-cursor`
`gamescope -w 1600 -h 900 -W 1920 -H 1080 -f --filter fsr --force-grab-cursor`
Installed using `paru -S gamescope`. Can be used to fix input issues or windowing issues, such as the one with CS2 where it won't go fullscreen properly. The second one can be used to upscale games from a lower resolution to get better performance. `-w 1600 -h 900` controls the rendering resolution, `-W 1920 -H 1080` controls the screen/window size/res.

## Variables
Variables are included in launch options and include an equal sign and usually included parts that are in all-caps. There are usually easy to spot in launch options and always go before any other launch options

`ALSOFT_DRIVERS=ALSA PULSE_LATENCY_MSEC=100`
Can sometimes fix audio bugs. Not recommended unless you are experiencing issues with audio. Remove if it does not resolve the issues.

`PROTON_SET_GAME_DRIVE=1`
This is used for Garry's Mod. I'm not sure what it does, but its apparently required, as well as [GModCEFCodecFix](https://github.com/solsticegamestudios/GModCEFCodecFix)

## Examples
Some other examples:
My CS2 Launch options: `SDL_VIDEODRIVER=wayland XKB_DEFAULT_LAYOUT=us XKB_DEFAULT_VARIANT=colemak_dh gamemoderun gamescope -f --force-grab-cursor -r 180 -s 0.5 %command% -nojoy -novid -threads 12`

Broken down: The Environment Variable `SDL_VIDEODRIVER=wayland` ensures that it runs using Wayland specific code.
`XKB_DEFAULT_LAYOUT=us XKB_DEFAULT_VARIANT=colemak_dh` sets the keyboard layout to US Colemak-DH (the one that I use).
`gamemoderun` is described below.
`gamescope -f --force-grab-cursor -s 0.5` runs the game under gamescope, forces it so use fullscreen and to grab the cursor to fix input issues with gamescope. Finally it multiplies the mouse speed by 0.5. Running the game under gamescope is a fix for the game not covering the panel in fullscreen.

Usable CS2 options that I recommend you apply: 
`SDL_VIDEODRIVER=wayland gamemoderun gamescope -f -r 300 --force-grab-cursor %command% -nojoy -novid`

