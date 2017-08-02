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

2. List all projects in the catalogue and list all available modes of the example voting app:
	```shell
	$ project-catalog ls
	nginx
	example-voting-app
	mysql

	$ project-compose mode ls example-voting-app
    default
    javaworker
    simple
	```

3. Start and stop the Docker example voting app in default mode:
	```sh
	$ project-compose start example-voting-app
	...
	$ project-compose down example-voting-app
	```

4. Start and stop the Docker example voting app in javaworker mode:
	```shell
	$ project-compose start example-voting-app javaworker
	...
	$ project-compose down example-voting-app javaworker
	```
Other examples
----------------
- [example-voting-app](https://github.com/shiwaforce/project-compose-example/blob/master/example-voting-app/README.md)
- [nginx](https://github.com/shiwaforce/project-compose-example/blob/master/nginx/README.md)
- [mysql](https://github.com/shiwaforce/project-compose-example/blob/master/mysql/README.md)

License
-------

MIT

Contributors
------------

[ShiwaForce.com Inc.](https://www.shiwaforce.com/en/)
