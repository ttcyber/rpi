# rpi
rpi code and configuration
<pre> 
As root (sudo -i)
Configure the pi
#raspi-config
- Expand the file system.
- Se pi password 
- Change your keyboard layout to US
- Change hostname to z314 where z is NATO letter of your work station.
- Enable ssh

# useradd -m -d /home/username  username
# usermod -a -G pi,adm,dialout,cdrom,sudo,audio,video,plugdev,games,users,input,netdev,gpio,i2c,spi username
Change your password
#passwd username

# apt-get upgrade
# apt-get update
// optional
# dpkg --configure -a
#apt-get autoremove

#apt-get install firefox-esr
#apt-get install bless (hex editor)

// nodejs
curl -sL https://deb.nodesource.com/setup_7.x | sudo -E bash -
sudo apt-get install -y nodejs

<hr />
DO NOT DO THIS ON CLIENTS
Back up /etc/dhcpcd.conf
then replace the code with the following:

# /etc/dhcpcd.conf
interface eth0

static ip_address=192.168.0.10/24
static routers=192.168.0.1
static domain_name_servers=192.168.0.1

interface wlan0

static ip_address=192.168.0.200/24
static routers=192.168.0.1
static domain_name_servers=192.168.0.1

</pre>

