# Linux-Configs

# Update all system
sudo pacman -Suuyy

# install yay
sudo pacman -S --needed git base-devel
cd /tmp
git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si

# zsh
chsh -s /usr/bin/zsh

# Install some usefull programs...
yay nano rust alacritty htop tmux
cargo install exa ripgrep procs bat

# Enable systemd-homed for login and password work every time
systemctl start systemd-homed
systemctl enable systemd-homed
