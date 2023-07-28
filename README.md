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

![Screenshot from 2023-07-28 07-54-10](https://github.com/Chillsmeit/network-manager-wireguard-jammy/assets/93094077/d6f04745-0892-445d-a954-84800de7916c)
### As you can see there's already a wireguard option
![Screenshot from 2023-07-28 07-17-56](https://github.com/Chillsmeit/network-manager-wireguard-jammy/assets/93094077/225d0d49-b7d8-4bbc-9fcb-9953ce285960)
![Screenshot from 2023-07-28 08-07-38](https://github.com/Chillsmeit/network-manager-wireguard-jammy/assets/93094077/2eb48742-56b1-4e53-b107-9f11bad67bbf)
![Screenshot from 2023-07-28 07-55-08](https://github.com/Chillsmeit/network-manager-wireguard-jammy/assets/93094077/b4b46f34-e6b6-48db-96ce-84a151c85175)

