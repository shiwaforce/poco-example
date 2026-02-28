About
-----

MySQL example for [Poco](https://github.com/shiwaforce/poco). Add the poco-example catalog first (`poco repo add poco-examples https://github.com/shiwaforce/poco-example.git`).

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
	poco plan ls mysql
	```

2. Start and stop (default plan):
	```shell
	poco up mysql
	poco down mysql
	```

3. Start with phpMyAdmin (dev/with-phpmyadmin plan):
	```shell
	poco up mysql/dev/with-phpmyadmin
	poco down mysql/dev/with-phpmyadmin
	```
Other examples
--------------

- [example-voting-app](https://github.com/shiwaforce/poco-example/blob/master/example-voting-app/README.md)
- [nginx](https://github.com/shiwaforce/poco-example/blob/master/nginx/README.md)

More information
----------------

- [getpoco.io](https://getpoco.io)
- [Poco on GitHub](https://github.com/shiwaforce/poco)
