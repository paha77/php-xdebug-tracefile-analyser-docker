# php-xdebug-tracefile-analyser-docker

Builds a PHP container with https://github.com/derickr/xdebug/blob/master/contrib/tracefile-analyser.php

Build:

```sh
docker build -t php-tracefile-analyser .
```

Usage:

```sh
docker run -it --rm -v <path to generated php trace file>:/tracefile.xt php-tracefile-analyser php tracefile-analyser.php /tracefile.xt time-own 20
```
