About
-----

Example projects for [Poco 1.0](https://github.com/shiwaforce/poco) — one CLI for Docker, Kubernetes and Helm.

Poco lets you catalogue and manage Docker Compose projects using simple YAML files, so you can run projects without cloning or remembering long commands.

Requirements
------------

-   Docker 17+ (Docker Compose V2)
-   Python 3.12.3+
-   Poco: `pip install poco`

Quick start
-----------

Note: do not clone this repository for the quick start. Poco fetches the catalog for you.

1. Install poco:
	```shell
	pip install poco
	```

2. Add the catalog:
	```shell
	poco repo add poco-examples https://github.com/shiwaforce/poco-example.git
	```

3. List projects and plans:
	```shell
	poco catalog
	```

	Output:
	```
	Available projects:
	-------------------
	nginx
	example-voting-app
	mysql
	kubernetes
	gitlab
	```

	```shell
	poco plan ls example-voting-app
	```

4. Start the example voting app (default plan):
	```shell
	poco up example-voting-app
	```

	Visit http://localhost:5000. Stop with:
	```shell
	poco down example-voting-app
	```

5. Start with a different plan (javaworker):
	```shell
	poco up example-voting-app/javaworker
	poco down example-voting-app/javaworker
	```

Other examples
--------------

- [example-voting-app](example-voting-app/README.md)
- [nginx](nginx/README.md)
- [mysql](mysql/README.md)
- [kubernetes](kubernetes/) — Kubernetes Ingress example
- [gitlab](gitlab/) — GitLab Runner example

Links
-----

- [getpoco.io](https://getpoco.io) — Documentation
- [Poco on GitHub](https://github.com/shiwaforce/poco)

License
-------

MIT

Contributors
------------

[ShiwaForce.com Inc.](https://www.shiwaforce.com/en/)
