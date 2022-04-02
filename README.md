# Linux-Configs

## Update all system
```bash
sudo pacman -Suuyy
```


## install yay
```bash
sudo pacman -S --needed git base-devel
cd /tmp
git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si
```


## zsh
```bash
chsh -s /usr/bin/zsh
```


## Install some usefull programs...
```bash
yay nano rust ruby alacritty htop tmux wget zsh-autosuggestions zsh-syntax-highlighting visual-studio-code-bin teamviewer python-pip
cargo install exa ripgrep procs bat
```


## Enable systemd-homed for login and password work every time
```bash
systemctl start systemd-homed
systemctl enable systemd-homed
```

## Hacking Tools
```bash
pip install impacket
pip install pwntools
gem install evil-winrm
yay ffuf
```

## Vscode Compatibility
```bash
yay -S visual-studio-code-bin
yay -S libdbusmenu-glib
yay -S gnome-keyring
yay -Suuyy

```

# I3WM customization
fibonacci layout:

```bash
yay -S python-i3ipc
cd $HOME/.config/i3/
wget https://raw.githubusercontent.com/olemartinorg/i3-alternating-layout/master/alternating_layouts.py
chmod +x alternating_layouts.py
```
add this line on /.config/i3/config
>exec_always python $HOME/.config/i3/alternating_layouts.py