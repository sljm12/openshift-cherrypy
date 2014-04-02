openshift-cherrypy
==================

A sample CherryPy app for use with OpenShift

This is an example that show how to use [CherryPy](http://cherrypy.org/) with [OpenShift](https://www.openshift.com/) and the [mod_wsgi](http://modwsgi.readthedocs.org/en/latest/) components.

```
rhc create-app -a cherrypy -t python-2.7
```
Following this you can pull in the code from these examples by using:

```
git remote add quickstart https://github.com/sljm12/openshift-cherrypy.git
git fetch quickstart
git checkout master; git merge --strategy=recursive -X theirs quickstart/master
git push
```

This example uses the wsgi.py as the main entry point. 
