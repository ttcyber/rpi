# rpi
rpi code and configuration
<pre>
Updated 
As root (sudo -i)

# useradd -m -d /home/username  username
# usermod -a -G pi,adm,dialout,cdrom,sudo,audio,video,plugdev,games,users,input,netdev,gpio,i2c,spi cwc

# apt-get upgrade
# apt-get update
// optional
# dpkg --configure -a
#apt-get autoremove

#apt-get install firefox-esr
#apt-get install bless

// nodejs
curl -sL https://deb.nodesource.com/setup_7.x | sudo -E bash -
sudo apt-get install -y nodejs


</pre>

