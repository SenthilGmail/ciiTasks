=== User Dashboard and Registration===
Language: PHP 7.3
MVC Pattern: CodeIgniter 3
Database: mysql

=====Composer
(Composer will install all dependencies)
Install the composer
run command composer install inside the root directory of the project

=====Database dump:
db_dump.sql
1. Create a database with name cii_db
2. Import the db_dump which has table for users.
3. Go to Codeigniter folder application/config.php => change the database settings.


Plugins used:
Google Captcha = To enable captcha validation in the registration page.
Kickbox = Check the email is real mail not junk or test mail.
Datatables = to table with sorting options.

==Google Captcha===
Please change the google captcha key in Controller/User.php line 41
Please change the google site key in user_add.php in view folder line 41

== Kickbox===
Please change the kickbox key in Controller/User kickboxcheck function in line number 65


===Secure REST=====
auth = basic
username = admin
password = 1234

GET - http://localhost:8080/mycii/api/user/1 = Read
GET - http://localhost:8080/mycii/api/users/ = all user
POST - http://localhost:8080/mycii/api/user/add
DELETE - http://localhost:8080/mycii/api/user/delete/6

