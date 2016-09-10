
# must be trusty
crouton -r trusty -t x11 -n t2

apt-get install php5

apt-get install i3

echo "exec i3" > ~/.xinitrc

apt-get install curl

curl -s https://packagecloud.io/install/repositories/phalcon/stable/script.deb.sh | sudo bash

sudo apt-get install php5-phalcon

apt-get install chromium-browser

# dont launch as root first time or root will own the data files
chromium browser&

# test php / phalcon
sudo sh -c 'echo "<?php print_r(get_loaded_extensions());" > /var/www/html/index.php'

sudo /etc/init.d/apache2 start

# check for phalcon in the array
chromium-browser http://localhost/index.php

# get git
apt-get install git 

#download sublime text

curl -s https://download.sublimetext.com/sublime-text_build-3114_amd64.deb

dpkg -i /home/tom/Downloads/sublime-text_build-3114_amd64.deb

#run sublime
subl


