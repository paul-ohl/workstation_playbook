# My setup

## Hyprland:

### binary install

1. install deps: `sudo dnf install ninja-build cmake meson gcc-c++ libxcb-devel libX11-devel pixman-devel cairo-devel pango-devel wayland-devel libdrm-devel libxkbcommon-devel mesa-libEGL-devel libinput-devel rust-libudev-devel wlroots-devel xdg-desktop-portal-wlr xorg-x11-server-Xwayland-devel hwdata-devel libdisplay-info-devel`

I also needed [v1.32 of wayland-protocols](https://dl.fedoraproject.org/pub/fedora/linux/development/rawhide/Everything/x86_64/os/Packages/w/wayland-protocols-devel-1.32-2.fc39.noarch.rpm). Download and `sudo dnf localinstall file`
2. clone: `git clone --recursive https://github.com/hyprwm/Hyprland.git`
3. checkout latest tag: `git checkout --recursive tags/v0.29.1` (the --recursive may not be necessary)
4. in the project root: `meson setup _build`
5. in the project root: `sudo ninja -C _build install`

### Extra programs

sudo dnf install waybar wofi dunst

git clone https://github.com/Horus645/swww.git && cd swww && cargo build --release
cp target/release/swww target/release/swww-daemon ~/.local/bin

pip install pywal
