# Bootsplash-manjaro-globe

Kernel Bootsplash theme for manjaro Linux using White Manjaro logo and a rotate world spinner with maia color wallpaper.

This project was based on multiple other great projects like:

https://github.com/Blacksuan19/Bootsplash-Themes

https://github.com/GrayJack/manjaro-grayjack/tree/master/PKGBUILDs/manjaro-bootsplash-green

The spinner base gif was created using Preloaders.net and heavily modified afterwards

Author: Pablo Lenna

# Installation:

- `git clone https://github.com/githubgeeker/bootsplash-manjaro-globe`
- `cd bootsplash-manjaro-globe`
- run `chmod +x bootsplash-manjaro-globe.sh`
- run `chmod +x bootsplash-packer`
- run `sh bootsplash-manjaro-globe.sh` to generate STL model.
- run `makepkg -s` to create an Arch package and install it with `pacman -U $package_name`or alternatively make and install with one single command: `makepkg -sci`
- append `bootsplash-manjaro-globe` hook at the end of HOOKS string in `/etc/mkinitcpio.conf`
- add `bootsplash.bootfile=bootsplash-themes/manjaro-globe/bootsplash` at the end of `GRUB_CMDLINE_LINUX` string in `/etc/default/grub` and don't forget to remove the `quiet` parameter!
- run `sudo mkinitcpio -P linux`
- run `sudo update-grub`
