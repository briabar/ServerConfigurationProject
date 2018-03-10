Server Configuration Project
=============================

i.
--
ssh -i graderKey -p 2200 grader@159.65.91.239

ii.
----
http://159.65.91.239/

iii.
-----
1. Upgraded all packages.
2. Installed pip, apache2, WSGI, and postgresql  
3. Downloaded and installed Required python modules: sqlalchemy, requests, psycopg2,
      flask, Oauth2, and Oauth2client
4. Configured /etc/ssh/sshd_config to host on port 2200, only use public/private
      key authorization, and disallow root login.
5. Created user grader and added grader to sudoers.
6. logged into postgres and created database.
7. Gave postgres database permissions to www-data to be hosted by apache.
9. edited the WSGI configuration file to run start.WSGI
10. Wrote an app called start.wsgi to call main.py.  This allows me to
      import app as application from main.

iv.
-----
udacity forums
apache documentation
WSGI documentation
