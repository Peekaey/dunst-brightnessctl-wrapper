# Wrapper for dunst & brightnessctl - WIP

Small python program that uses brightnessctl and dunst to adjust the brightness of the display as well as provide a system notification upon increase/decrease of the brightness.

# Screenshot
*To provide screenshot*

## Requirements
- dunst - https://github.com/dunst-project/dunst
- brightnessctl - https://github.com/Hummer12007/brightnessctl
- python - https://www.python.org/

### How to run
- Increase brightness `python3 brightness.py up`
- Decrease brightness `python3 brightness.py down`

By default the program will increase or decrease by 10% 

Could also integrate and bind this program to keys (such as laptop brightness increase/decrease keys).
Example of this could be with hyprland DE and through adding the below to bind the actions to their respective keys.

Example in hyprland.config file  
`bindle=,XF86MonBrightnessUp,exec,"/usr/bin/python3 ~/.config/hypr/scripts/brightness.py up"`
`bindle=,XF86MonBrightnessDown,exec,"/usr/bin/python3 ~/.config/hypr/scripts/brightness.py down"`