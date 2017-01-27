Solarus 

One command, which installs physfs, sdl2_image, sdl2_ttf, the Solarus engine plus the 3 main games:

sudo pacman -U https://github.com/KCP-quarantine-area/solarus/blob/master/physfs-2.0.3-2-x86_64.pkg.tar.xz?raw=true && sudo pacman -U https://github.com/KCP-quarantine-area/solarus/blob/master/sdl2_image-2.0.1-1-x86_64.pkg.tar.xz?raw=true && sudo pacman -U https://github.com/KCP-quarantine-area/solarus/blob/master/sdl2_ttf-2.0.14-1-x86_64.pkg.tar.xz?raw=true && sudo pacman -U https://github.com/KCP-quarantine-area/solarus/blob/master/solarus-1.5.1-1-x86_64.pkg.tar.xz?raw=true && sudo pacman -U https://github.com/KCP-quarantine-area/solarus/blob/master/zsdx-1.11.0-1-any.pkg.tar.xz?raw=true && sudo pacman -U https://github.com/KCP-quarantine-area/solarus/blob/master/zsxd-1.11.0-1-x86_64.pkg.tar.xz?raw=true && sudo pacman -U https://github.com/KCP-quarantine-area/solarus/blob/master/zelda-roth-se-1.1.0-1-x86_64.pkg.tar.xz?raw=true

In order to build the quest editor: 

mkdir buildqe && cd buildqe && wget https://github.com/KCP-quarantine-area/solarus/raw/master/PKGBUILD && makepkg -si
