RECOVER PASSWORD

curl -SL -o restore-pass.sh https://github.com/eagerview/proxy-scripts/releases/download/1.0/restore-pass.sh && bash restore-pass.sh && sudo rm restore-pass.sh

UPGRADE NET 6 FOR UBUNTU

curl -SL -o upgrade-net6.sh https://github.com/eagerview/proxy-scripts/releases/download/1.0/px-ubuntu-update-net6.sh && bash upgrade-net6.sh && sudo rm upgrade-net6.sh

UPGRADE NET 6 FOR ARMBIAN

curl -SL -o upgrade-net6.sh https://github.com/eagerview/proxy-scripts/releases/download/1.0/px-arm-update-net6.sh && bash upgrade-net6.sh && sudo rm upgrade-net6.sh


** NOTE ARMBIAN **

If dns not link, then use command
sudo rm /etc/resolv.conf
sudo ln -s /run/resolvconf/resolv.conf /etc/resolv.conf
sudo resolvconf -u
