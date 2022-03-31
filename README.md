# Linux-Configs

# Update all system
```bash
sudo pacman -Suuyy
```


# install yay
```bash
sudo pacman -S --needed git base-devel
cd /tmp
git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si
```


# zsh
```bash
chsh -s /usr/bin/zsh
```


# Install some usefull programs...
```bash
yay nano rust alacritty htop tmux
cargo install exa ripgrep procs bat
```


# Enable systemd-homed for login and password work every time
```bash
systemctl start systemd-homed
systemctl enable systemd-homed
```

