MySQL andmebaasi serveri installeerimine
```
sudo apt-get install mysql-server
```
* MySQL seadistamine
```
sudo mysql_secure_installation

* MySQL kasutamine

sudo mysql


* MySQL kasutaja loomine

 mysql>CREATE USER 'heikovalli'@'localhost' IDENTIFIED BY '******';


 * õiguste andmine

  mysql>GRANT ALL PRIVILEGES ON *.* TO 'heikovalli'@'localhost';

  * MySQL-ist väljumine

  mysql> exit

* .env failis:
```
DATABASE_URL=mysql://kasutajanimi:parool@127.0.0.1:3306/bookingappdatabase 

* andmebaasi loomine
```
php bin/console doctrine:database:create