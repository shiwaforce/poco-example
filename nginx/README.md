About
-----

Examples for the project: https://github.com/shiwaforce/project-compose

Project Compose lets you catalogue and manage your Docker projects using
simple YAML files to shorten the route from finding your project to
initialising it in your local environment.

This helps you set up your local development environment and to run
demos.

Requirements
------------

-   Docker, version \> 17
-   Python, version \> 2.7

Quick start 
------------

1. Install the latest project-compose and initialise sample catalogue:
	```shell
	$ pip install project-compose
	$ project-catalog init https://github.com/shiwaforce/project-compose-example.git
	```

2. List all projects in the catalogue and list all available plans of the example voting app:
	```shell
	$ project-catalog ls
	default
	demo/hello
	```
    
3. Start and stop the Docker example voting app in default plan:
	```sh
	$ project-compose start nginx
	...
	$ project-compose down nginx
	```
    
4. Start and stop the Docker example voting app in javaworker plan:
	```shell
	$ project-compose start nginx demo/hello
	...
	$ project-compose down nginx demo/hello
	```
Other examples
----------------
- [example-voting-app](https://github.com/shiwaforce/project-compose-example/blob/master/example-voting-app/README.md)
- [nginx](https://github.com/shiwaforce/project-compose-example/blob/master/nginx/README.md)
- [mysql](https://github.com/shiwaforce/project-compose-example/blob/master/mysql/README.md)

More information
-----------------
- https://github.com/shiwaforce/project-compose
- https://www.shiwaforce.com
