RECOVER PASSWORD

curl -SL -o restore-pass.sh https://github.com/eagerview/proxy-scripts/releases/download/1.0/restore-pass.sh && bash restore-pass.sh && sudo rm restore-pass.sh

UPGRADE NET 6 FOR UBUNTU

curl -SL -o upgrade-net6.sh https://github.com/eagerview/proxy-scripts/releases/download/1.0/px-ubuntu-update-net6.sh && bash upgrade-net6.sh && sudo rm upgrade-net6.sh

UPGRADE NET 6 FOR ARMBIAN

curl -SL -o upgrade-net6.sh https://github.com/eagerview/proxy-scripts/releases/download/1.0/px-arm-update-net6.sh && bash upgrade-net6.sh && sudo rm upgrade-net6.sh


** NOTE ARMBIAN **
First open the nm conf file /etc/NetworkManager/NetworkManager.conf:

sudo vim /etc/NetworkManager/NetworkManager.conf
And add this to the [main] section:

dns=none
rc-manager=unmanaged

If dns not link, then use command </br>
sudo rm /etc/resolv.conf </br>
sudo ln -s /run/resolvconf/resolv.conf /etc/resolv.conf </br>
sudo resolvconf -u
