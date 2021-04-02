1. Started with Ubuntu system on Contabo.net

1. [nix-os-infect](https://github.com/elitak/nixos-infect) This script is handy. I ran this to convert to NixOS. A few hiccups:

  - Ignored a Warning about not supporting multiuser Nix setup or something like that
  - Didn't like "." in hostname. So changed hostname and re-ran
  - couldn't rename /boot to /boot.bak (resource busy error).  I edited the script to skip this
  
