#Linux Server Project

##Connection Information
The public IP address for the Lightsail instance is 34.221.80.254. SSH port 2200 is open. The main project files are located at /var/www/html/catalog/

##URL
The project can be seen from any browser at http://34.221.80.254/
Note that the Google Sign In does not work as it requires a .com address.

##Software Installed
The server had Apache, Python, Mod-WSGI, PostgreSQL, Flask, and Flask-SQLAlchemy packages installed.

Configuration changes necessary to serve the webpage included: 
  * Adding the /catalog/ folder to the system search path
  * Creating an application.wsgi file to route requests to application.py
  * Modifying the Apache configuration file to setup the WSGI routing
  * Replacing relative file paths with absolute paths within the python code
  * Changing a table name from 'user' to 'owner'

##Resources Used
  * http://flask.pocoo.org/docs/1.0/deploying/mod_wsgi/
  * https://vim.rtorr.com/
  * https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
  * https://www.digitalocean.com/community/tutorials/how-to-configure-logging-and-log-rotation-in-apache-on-an-ubuntu-vps
  * http://flask-sqlalchemy.pocoo.org/2.3/queries/
  * https://www.postgresql.org/docs/current/static/app-createdb.html
  * https://dba.stackexchange.com/questions/75551/returning-rows-in-postgresql-with-a-table-called-user