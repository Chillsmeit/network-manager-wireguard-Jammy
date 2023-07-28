# Network-Manager VPN Plugin for WireGuard 
### Ubuntu 22.04 / Pop!_OS 22.04 - ProtonVPN

Network manager plugin for Wireguard working with Ubuntu 22.04 and Pop!_OS 22.04.<br>
This fork is intended for ease of use of ProtonVPN users that want wireguard support in the Network Manager.

# How to Install

### Install Dependencies:
```
sudo apt install wireguard git dh-autoreconf libglib2.0-dev intltool build-essential libgtk-3-dev libnma-dev libsecret-1-dev network-manager-dev resolvconf
```
### Clone Repo and Install Network Manager:
```
git clone https://github.com/Chillsmeit/network-manager-wireguard-jammy
cd network-manager-wireguard-jammy
./autogen.sh --without-libnm-glib
./configure --without-libnm-glib --prefix=/usr --sysconfdir=/etc --libdir=/usr/lib/x86_64-linux-gnu --libexecdir=/usr/lib/NetworkManager --localstatedir=/var
make
sudo make install
```
# Import ProtonVPN Wireguard Configs

### Open Network Manager
![Screenshot from 2023-07-28 07-17-37](https://github.com/Chillsmeit/network-manager-wireguard-jammy/assets/93094077/5a67d732-7676-4c62-b2ab-28ede7a7c1b8)
### As you can see there's already a wireguard option
![Screenshot from 2023-07-28 07-17-56](https://github.com/Chillsmeit/network-manager-wireguard-jammy/assets/93094077/225d0d49-b7d8-4bbc-9fcb-9953ce285960)
### Import your config
![Screenshot from 2023-07-28 07-18-07](https://github.com/Chillsmeit/network-manager-wireguard-jammy/assets/93094077/7abd897f-7f92-4c02-b933-e21bb23dd052)
