# Linux Server Configuration
*Full Stack Nanodegree Project*

### Project Overview
For this project I had to take a baseline installation of a Linux distribution on a virtual machine and prepare it to host my web application by installing updates, securing it from a number of attack vectors, and installing/configuring web and database servers.


### IP Address and SSH port
The static IP address for this project is 13.59.60.140.
The SSH port is 2200.

### Hosted Web Application
The web application resides at http://13.59.60.140/.

### Summary of Installed Software and Configuration Changes
Here's a summary of the steps I've taken:
* Created a unique ssh-keygen pair for my admin account and removed the default key provided by AWS from the authorized_keys directory.
* Updated all installed packages.
* Autoremoved any packages no longer required after update.
* Configured the UFW to only allow incoming on 2200, 80, and 123.
* Created a new user for the project reviewer and provided them sudo access by creating a sudo file in sudoers.d.
* Created a SSH key pair for the reviewer.
* Confiured the local timezone to UTC.
* Installed Apache, mod_wsgi, PostgreSQL, flask, oauth2client, requests, git and application dependencies.
* Cloned my project to the remote server and configured wsgi to point to it.
* Updated my project code to reflect use of PostgreSQL.


### List of Resources Used to Assist in Project Completion
Here's a brief summary of resources I used for this project:
* Stack Overflow
* Udacity Discussion Forums
* DigitalOcean tutorial [How to Deploy a Flask Application on an Ubuntu VPS](https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps).
* Apache Error Log