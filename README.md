# bootsplash-theme-tardis
Kernel Bootsplash theme for manjaro Linux using tardis

# Installation:

- append `bootsplash-theme-tardis` hook in the end of HOOKS string of `/etc/mkinitcpio.conf`
- add `quiet bootsplash.bootfile=bootsplash-themes/tardis/bootsplash` into `GRUB_CMDLINE_LINUX` string in `/etc/default/grub`
- run `sudo mkinitcpio -p linux414`
- run `sudo update-grub`
