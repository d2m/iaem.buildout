iaem.buildout
=============

Base package for iaem.at.


Requirements
------------
* Create a sandbox with virtualenv[1] and Python2.6
  

Buildout configurations
-----------------------
dev.cfg - Development version
deploy.cfg - Deployment version


How to install
--------------
$ python bootstrap.py -d -c dev.cfg
$ ./bin/buildout -c dev.cfg
$ ./bin/zeoserver start # Zope Enterprise Objects Database Server
$ ./bin/instance fg # Zope instance, foreground mode

* Point your webbrowser to http://localhost:8080/ (username admin,
  password admin)
* Add a ZODB Mount Point (iaem is already configured) and enter the folder
* Install a Plone instance.


References
----------
[1] http://pypi.python.org/pypi/virtualenv
