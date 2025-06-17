# ideal-guacamole
django web server project. 

Created a virtual python environment call django-venv.
Activate the venv: source django-env/bin/activate

Installed the packeges in requirements.txt via pip.

Errors during initial installation required running ./install_certificates.command in Python to add certificates too Python installation.

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

