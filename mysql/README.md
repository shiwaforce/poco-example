About
-----

Examples for the project: https://github.com/shiwaforce/poco

Project Compose lets you catalogue and manage your Docker projects using simple YAML files to shorten the route from finding your project to initialising it in your local environment.

This helps you set up your local development environment and to run demos.

Requirements
------------
-   Docker, version \> 17
-   Python, version \> 2.7

Quick start 
------------
1. Install the latest poco:
	```shell
	$ pip install poco
	```
	
2. List all projects in the catalogue and list all available plans of the example voting app:
	```shell
	$ poco catalog ls
	nginx
	example-voting-app
	mysql
	
	$ poco plan ls mysql
	default
	dev/with-phpmyadmin
	```
    
3. Start and stop the mysql in default plan:
	```sh
	$ poco start mysql
	...
	$ poco down mysql
	```
    
4. Start and stop the mysql in dev/with-phpmyadmin plan:
	```shell
	$ poco start mysql dev/with-phpmyadmin
	...
	$ poco down mysql dev/with-phpmyadmin
	```
Other examples
----------------
- [example-voting-app](https://github.com/shiwaforce/poco-example/blob/master/example-voting-app/README.md)
- [nginx](https://github.com/shiwaforce/poco-example/blob/master/nginx/README.md)
- [mysql](https://github.com/shiwaforce/poco-example/blob/master/mysql/README.md)

More information
-----------------
- https://github.com/shiwaforce/poco
- https://www.shiwaforce.com
