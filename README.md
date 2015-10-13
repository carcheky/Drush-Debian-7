# Drush-Debian-7
Install drush in Debian 7

# CONTENT SCRIPT
sudo apt-get install git
curl -sS https://getcomposer.org/installer | php
sudo mv composer.phar /usr/local/bin/composer
sudo ln -s /usr/local/bin/composer /usr/bin/composer
composer global require drush/drush:7.*



cd /usr/local/src/drush
sudo ln -s /usr/local/src/drush/drush /usr/bin/drush
sudo composer install
drush --version


# INSTALL

cd /tmp; git clone "https://github.com/carcheky/Drush-Debian-7.git"; cd *Drush*; chmod +x install.sh; bash install.sh
