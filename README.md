# sddm-raised

Simple script to constantly raise/focus SDDM window, to prevent other
windows being shown over it. Requires xdotool

## Installing
It can be installed via the AUR in Arch Linux

```bash
yay -S sddm-raised
```

## Installing manually

### Clone this repository

```bash
git clone https://github.com/jamezrin/sddm-raised
```

### Install dependencies

- For Arch Linux, do `sudo pacman -S xdotool` 

- For Ubuntu, do `sudo apt install xdotool`

### Move necessary files

```bash
sudo cp sddm-raised /usr/local/bin/sddm-raised
sudo cp sddm-raised.service /etc/systemd/system/sddm-raised.service
sudo chmod 755 /usr/local/bin/sddm-raised
sudo chmod 644 /etc/systemd/system/sddm-raised.service
```

### Enable and start service

```bash
sudo systemctl enable sddm-raised
sudo systemctl start sddm-raised
```
