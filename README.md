# Live USB As Stage 4

This script downloads the Gentoo livegui ISO and extracts it to a BTRFS subvolume and adds a boot entry to sytemd-boot so that you can boot into the system afterwards. With this I installed Gentoo with KDE, Libreoffice, Two browsers, etc. in 1 min 8 sec. It's my PB and probably a WR for a Gentoo install ;-)

Here's the result:

![Screenshot](https://github.com/damianoognissanti/luas4/blob/main/luas4.png?raw=true)

This script:

- Downloads the LiveUSB and checksum and verify checksum.
- Creates a new btrfs subvolume.
- Copies and extracts the live-image.
- Creates fstab entries
- Creates a boot loader entry.
- Configures the installed system (adds user, set locale, etc.)

Pull requests are welcome if you want to help improving the script. Otherwise, do what you want with it.
