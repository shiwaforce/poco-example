About
-----

Examples for the project: https://github.com/shiwaforce/project-compose

Project Compose lets you catalogue and manage your Docker projects using
simple YAML files to shorten the route from finding your project to
initialising it in your local environment.

This helps you set up your local development environment and to run
demos.

`Shiwaforce.com <https://www.shiwaforce.com>`\_

Requirements
------------

-   Docker, version \> 17
-   Python, version \> 2.7

Quick start
===========

Install the latest project-compose:

`$ pip install project-compose`

Initialise sample catalogue:

`$ project-catalog init https://github.com/shiwaforce/project-compose-example.git`

List all projects in the catalogue:

`$ project-catalog ls`

List all available modes of the ex:mple voting app:

`$ project-compose mode ls example-voting-app`

Start the Docker example voting app in javaworker mode:

`$ project-compose start example-voting-app javaworker`

Stop the example voting app:

`$ project-compose down example-voting-app javaworker`

Start the Docker example voting app in default mode:

`$ project-compose start example-voting-app default`

Stop the example voting app:

`$ project-compose down example-voting-app default`
