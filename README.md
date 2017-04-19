# pimotd
This tweaks the motd do be much cooler


![alt tag](https://raw.githubusercontent.com/deathbybandaid/pimotd/master/image.png)


### Instructions

sudo uname -snrvm > /var/run/motd.dynamic

sudo systemctl disable motd

sudo mkdir /etc/update-motd.d

sudo rm -f /etc/motd

sudo wget https://raw.githubusercontent.com/deathbybandaid/pimotd/master/10logo -P /etc/update-motd.d/

chmod a+x /etc/update-motd.d/*

sudo sed -i "s/motd.dynamic/motd.new/" /etc/pam.d/sshd
