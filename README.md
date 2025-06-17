# ideal-guacamole
django web server project. 

Created a virtual python environment call django-venv.
Activate the venv: source django-env/bin/activate

Installed the packeges in requirements.txt via pip.

Errors during initial installation required running ./install_certificates.command in Python to add certificates too Python installation.

Added 'mod_wsigi.server', to settings.py

It seems that httpd.conf is already configured to run at Daemon? (This is the recommended option for non-Windows systems.)

# Useful Commands: 
Compilation of commands that I have used to help manage this project. 

# mod_wsgi-express start-server
Starts the apache/mod_wsgi server. 

# lsof -i :8000 
Lists the PIDs on the current port. Mainly used to find the PIDs of httpd processes that I forgot to close. 

# kill -9 PID
Kills the given PID. 
    
# Commands: mod_wsgi-express
mod_wsgi-express start-server wsgi.py
mod_wsgi-express start-server wsgi.py --port 8080
mod_wsgi-express start-server --help

# django documentation
django-admin startproject mysite djangotutorial
python manage.py runmodwsgi --reload-on-changes
python manage.py runmodwsgi
