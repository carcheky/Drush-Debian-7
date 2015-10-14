Install drush in Debian 7

# INSTALL drush 6
cd /tmp; git clone "https://github.com/carcheky/Drush-Debian-7.git"; cd Drush*; chmod +x install-drush6.sh; bash install.sh

# INSTALL drush 7
cd /tmp; git clone "https://github.com/carcheky/Drush-Debian-7.git"; cd Drush*; chmod +x install-drush7.sh; bash install.sh




# CONTENT SCRIPT
sudo apt-get install git;
curl -sS https://getcomposer.org/installer | php;
mv composer.phar /usr/local/bin/composer;
ln -s /usr/local/bin/composer /usr/bin/composer;
git clone https://github.com/drush-ops/drush.git /usr/local/src/drush;
cd /usr/local/src/drush;
git checkout X.0.0;  #or whatever version you want.
ln -s /usr/local/src/drush/drush /usr/bin/drush;
composer install;
drush --version;
