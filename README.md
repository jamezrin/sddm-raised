# sddm-raised

Simple script to constantly raise/focus SDDM window, to prevent other
windows being shown over it. Requires xdotool

## Installing

### Clone this repository

```
git clone https://github.com/jamezrin/sddm-raised
```

### Install dependencies

- For Arch Linux, do `sudo pacman -S xdotool` 

- For Ubuntu, do `sudo apt install xdotool`

### Move necessary files

```
sudo cp sddm-raised /usr/local/bin/sddm-raised
sudo cp sddm-raised.service /etc/systemd/system/sddm-raised.service
sudo chmod 644 /etc/systemd/system/sddm-raised.service
```

### Enable and start service

```
sudo systemctl enable sddm-raised
sudo systemctl start sddm-raised
```
