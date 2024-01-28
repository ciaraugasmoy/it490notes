sudo apt install
sudo apt install apache2 -y

----------------------------------
go to local host in browser:
128.0.0.1
aka home, me, loopback, localhost
if it works
----------------------------------
--important files to look out for--
/etc/apache2/apache2.conf
etc/apache2/sites-available/default-ssl.conf
etc/apache2/sites-enabled
----------------------------------
vim or vi
sudo apt install vim
-------------------------
10:00min
branch to checkout
rabbitmq example
git checkout websample

sudo cp 001-sample.conf etc/apache2/sites-available/
----------------------------------------------------
in var/www/sample$
sudo cp ~/git/rabbitmqphp_example/sample/index.html

in etc/apache2/sites-enabled/
sudo rm 000-default.conf
THEN CREATE NEW SYMBOLIC LINK
sudo ln -s ..sites-available/001-sample.conf

sudo service apache2 reload
(at this point it will redirect, we will be doing a local override)
cd etc/hosts
---------
sudo vim hosts
to add
127.0.0.1 www.sample.com
-------------------------------------
TTL 
time to live
we need to flush the cache
go to 127.0.0.1 and clear history
then restart apache2
--
sudo service apache2 stop
(to see more)
sudo service apache2 status

-------------------------------------
LOOKING AT THE BACKEND
from home cd
/var/www/sample/index.html

-----------------------------

sudo cp ~git/rabbitmqphp_example/sample/login.php ./

------------------------------
2 different phps




