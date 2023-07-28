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
git clone https://github.com/Chillsmeit/network-manager-wireguard-Jammy
cd network-manager-wireguard-Jammy
./autogen.sh --without-libnm-glib
./configure --without-libnm-glib --prefix=/usr --sysconfdir=/etc --libdir=/usr/lib/x86_64-linux-gnu --libexecdir=/usr/lib/NetworkManager --localstatedir=/var
make
sudo make install
```
