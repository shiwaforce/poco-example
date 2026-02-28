About
-----

Nginx example for [Poco](https://github.com/shiwaforce/poco). Add the poco-example catalog first (`poco repo add poco-examples https://github.com/shiwaforce/poco-example.git`).

Requirements
------------

-   Docker 17+ (Docker Compose V2)
-   Python 3.12.3+
-   Poco: `pip install poco`

Quick start
-----------

1. Add catalog and list plans:
	```shell
	poco repo add poco-examples https://github.com/shiwaforce/poco-example.git
	poco plan ls nginx
	```

2. Start and stop (default plan):
	```shell
	poco up nginx
	poco down nginx
	```

3. Start with demo/hello plan:
	```shell
	poco up nginx/demo/hello
	poco down nginx/demo/hello
	```
Other examples
--------------

- [example-voting-app](https://github.com/shiwaforce/poco-example/blob/master/example-voting-app/README.md)
- [mysql](https://github.com/shiwaforce/poco-example/blob/master/mysql/README.md)

More information
----------------

- [getpoco.io](https://getpoco.io)
- [Poco on GitHub](https://github.com/shiwaforce/poco)
