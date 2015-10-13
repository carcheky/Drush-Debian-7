# Drush-Debian-7
Install drush in Debian 7

# CONTENT SCRIPT
sudo apt-get install git
curl -sS https://getcomposer.org/installer | php
sudo mv composer.phar /usr/local/bin/composer
sudo ln -s /usr/local/bin/composer /usr/bin/composer
sudo git clone https://github.com/drush-ops/drush.git /usr/local/src/drush
cd /usr/local/src/drush
sudo ln -s /usr/local/src/drush/drush /usr/bin/drush
sudo composer install
drush --version


# INSTALL

cd /tmp; wget --no-check-certificate -O installer.tgz "https://github.com/carcheky/Drush-Debian-7.git"; tar zxvf installer.tgz; cd *Drush*; chmod +x install.sh; bash install.sh
