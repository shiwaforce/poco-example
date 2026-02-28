About
-----

Examples for the project: https://github.com/shiwaforce/poco

Poco lets you catalogue and manage your Docker projects using
simple YAML files to shorten the route from finding your project to
initialising it in your local environment.

This helps you set up your local development environment and to run
demos.

Requirements
------------

-   Docker 17+ (Docker Compose V2)
-   Python 3.12.3+
-   Poco: `pip install poco`

Quick start 
------------

1. Install the latest poco:
	```shell
	$ pip install poco
	```

2. List all projects in the catalogue and list all available plans of the example voting app:
	```shell
	$ poco catalog
	nginx
	example-voting-app
	mysql
	
	$ poco plan ls example-voting-app
    default
    javaworker
    simple
	```
     
3. Start and stop the Docker example voting app in default plan:
	```sh
	$ poco up example-voting-app
	...
	$ poco down example-voting-app 
	```
    
4. Start and stop with javaworker plan:
	```shell
	$ poco up example-voting-app/javaworker
	...
	$ poco down example-voting-app/javaworker
	```

Other examples
--------------

- [nginx](https://github.com/shiwaforce/poco-example/blob/master/nginx/README.md)
- [mysql](https://github.com/shiwaforce/poco-example/blob/master/mysql/README.md)

More information
----------------

- [getpoco.io](https://getpoco.io)
- [Poco on GitHub](https://github.com/shiwaforce/poco)
