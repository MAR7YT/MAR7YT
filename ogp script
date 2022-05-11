sudo apt-get install apache2 curl subversion php7.4 php7.4-gd php7.4-zip libapache2-mod-php7.4 php7.4-curl php7.4-mysql php7.4-xmlrpc php-pear phpmyadmin mariadb-server-10.3 php7.4-mbstring git php-bcmath

sed -i "s/^bind-address.*/bind-address=0.0.0.0/g" "/etc/mysql/mariadb.conf.d/50-server.cnf" && sudo apt-get install mariadb-server && sudo mysql_secure_installation

wget -N "https://github.com/OpenGamePanel/Easy-Installers/raw/master/Linux/Debian-Ubuntu/ogp-panel-latest.deb" -O "ogp-panel-latest.deb" && sudo dpkg -i "ogp-panel-latest.deb"


INSTALLING AGENT
sudo apt-get install libxml-parser-perl libpath-class-perl perl-modules screen rsync sudo e2fsprogs unzip subversion libarchive-extract-perl pure-ftpd libarchive-zip-perl libc6 libgcc1 git && sudo apt-get install libc6-i386 libgcc1:i386 && sudo apt-get install lib32gcc1 && sudo apt-get install libhttp-daemon-perl && wget -N "https://github.com/OpenGamePanel/Easy-Installers/raw/master/Linux/Debian-Ubuntu/ogp-agent-latest.deb" -O "ogp-agent-latest.deb" && sudo dpkg -i "ogp-agent-latest.deb" && sudo cat /root/ogp_user_password 

INSTALLING TWEAKS INCLUDING THEMES AND PHPMYADMIN BUG FIX
cd /var/www/html/themes/ && wget https://github.com/hmrserver/Obsidian/archive/master.zip && unzip master.zip && cd Obsidian-master/themes/ && cp -R Obsidian /var/www/html/themes/ && cd /var/www/html/themes/ && mkdir CHENSAMPTHEME && cd /var/www/html/themes/CHENSAMPTHEME/ && wget https://github.com/chenschmidt/OGPSAMP/raw/main/OGPSAMPUPDATE.zip && unzip OGPSAMPUPDATE.zip && cd /var/www/html/themes/Obsidian/images/ && rm favicon.ico && rm hk. Jpg&& rm mrg.png && cd /var/www/html/themes/CHENSAMPTHEME/images/ && cp favicon.ico /var/www/html/themes/Obsidian/images/ && cp bg.jpg /var/www/html/themes/Obsidian/images/ && cp Êœá´‹.png /var/www/html/themes/Obsidian/images/ && sudo ln -s /usr/share/phpmyadmin /var/www/html/ && cd /var/www/html/includes/ && chmod 644 config.inc.php

FIX MYSQL BUG
sudo mysql -u root -p

USE mysql;

SELECT plugin FROM user WHERE user='root';

UPDATE user SET plugin='' WHERE User='root';

FLUSH PRIVILEGES;

EXIT;

INCREASE PHPMYADMIN UPLOAD SIZE
cd /etc/php/7.4/apache2 && nano php.ini

memory_limit = 2500M

post_max_size = 2500M

upload_max_filesize = 2500M

sudo service apache2 restart


--------------- gcp phpmyadmin fix [optional fix ]-------------- [root must ]
nano /etc/apache2/apache2.conf

[bottom]
Include /etc/phpmyadmin/apache.conf
