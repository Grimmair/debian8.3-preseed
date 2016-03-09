# debian8.3-preseed
Preseed for Debian Jessie - Rebuild a Debian ISO with preseed/custom files. Credits for the original rebuild-debian-iso script belong to cdown on github. 

You might want to configure/change the following values of preseed.cfg
- root and user password
- host and domain names
- NTP and DHCP Configs
- Keyboard locals
- Apt repository url
- Packages you want to install

Dependencies
- bsdtar
- genisoimage

# Usage

    rebuild-debian-iso <input-iso> <output-iso> <preseed-file> [file-dir]

    input-iso:    the debian iso to modify
    output-iso:   where to store the modified iso
    preseed-file: the location of a preseed file to inject
    file-dir:     an optional directory to be put at extra/ in the iso
