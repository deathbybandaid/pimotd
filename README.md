# pimotd
This tweaks the motd do be much cooler


It should look like this without the weather.

![alt tag](https://raw.githubusercontent.com/deathbybandaid/pimotd/master/raspilogin2.jpg)


### Instructions

sudo systemctl disable motd

mkdir /etc/update-motd.d

rm -f /etc/motd

sudo wget https://raw.githubusercontent.com/deathbybandaid/pimotd/master/10logo -P /etc/update-motd.d/
