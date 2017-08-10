About
-----

Examples for the project: https://github.com/shiwaforce/project-compose

Project Compose lets you catalogue and manage your Docker projects using simple YAML files to shorten the route from finding your project to initialising it in your local environment.

This helps you set up your local development environment and to run demos.

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
	nginx
	example-voting-app
	mysql
	
	$ project-compose plan ls mysql
	default
	dev/with-phpmyadmin
	```
    
3. Start and stop the mysql in default plan:
	```sh
	$ project-compose start mysql
	...
	$ project-compose down mysql
	```
    
4. Start and stop the mysql in dev/with-phpmyadmin plan:
	```shell
	$ project-compose start mysql dev/with-phpmyadmin
	...
	$ project-compose down mysql dev/with-phpmyadmin
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
