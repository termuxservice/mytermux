                  mytermux
#container 
git clone https://github.com/Moe-hacker/termux-container
cd termux-container/package
chmod -R 755 DEBIAN
chmod 777 data/data/com.termux/files/usr/bin/container
dpkg -b . ~/termux-container.deb
apt update
apt install ~/termux-container.deb
