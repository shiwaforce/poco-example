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
===========

Install the latest project-compose:
```shell
$ pip install project-compose
```

Initialise sample catalogue:
```shell
$ project-catalog init https://github.com/shiwaforce/project-compose-example.git
```

List all projects in the catalogue:
```shell
$ project-catalog ls
```

List all available modes of the example voting app:
```shell
$ project-compose mode ls example-voting-app
```

Start the Docker example voting app in javaworker mode:
```shell
$ project-compose start example-voting-app javaworker
```

Stop the example voting app:
```shell
$ project-compose down example-voting-app javaworker
```

Start the Docker example voting app in default mode:
```shell
$ project-compose start example-voting-app default
```

Stop the example voting app:
```shell
$ project-compose down example-voting-app default
```

More information
-----------------
- https://github.com/shiwaforce/project-compose
- https://www.shiwaforce.com

