The following text assumes Sway, but likely easily portable for Hyprland 

Requires nerd-fonts package 
https://www.nerdfonts.com/
May work with nerd-fonts-symbols-ttf instead 

Also requires Rajdnahi font: 
https://fonts.google.com/specimen/Rajdhani

Putting extracted fonts in /usr/share/fonts works for me

I managed to get alacritty blur rendering working with SwayFX, have not tried anything else. 

No GTK themes - I have not worked on them before and don't plan to for the time being
No theme manager - the code should function as-is, but in Sway (unsure of hyprland) I would reccommend using, example: 

Put themes in their own directory, for me, I used ~/path/to/.config/alacritty/2077/alacritty.toml
```
bindsym $mod+Return exec alacritty --config-file ~/.config/alacritty/2077/alacritty.toml
bindsym $mod+d exec wofi -S drun -c ~/.config/wofi/2077/config -s ~/.config/wofi/2077/style.css
exec waybar -c ~/.config/waybar/2077/config -s ~/.config/waybar/2077/style.css
```
Enjoy!
