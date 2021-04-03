1. Started with Ubuntu system on Contabo.net

1. [nix-os-infect](https://github.com/elitak/nixos-infect) This script is handy. I ran this to convert to NixOS. A few hiccups:
    - Ignored a Warning about not supporting multiuser Nix setup or something like that
    - Didn't like "." in hostname. So changed hostname and re-ran
    - couldn't rename /boot to /boot.bak (resource busy error).  I edited the script to skip this

1. Looks like partitioning disks and creating filesystems is done the traditional way. No reproducible, functional NixOS magic here.  I didn't change the partitions. Kept what nixos-infect left me, which seems to be the partitioning that was in effect under Ubuntu. 
1. [flox](https://beta.floxdev.com/docs/tour/tour-1/#install-flox) A DESCO tool for building/installing/managing Nix packages
2. Looks like `/etc/nixos/configuration.nix` and its nested imports will control the OS environment. Packages will be installed by floxpm command or from the flox website
