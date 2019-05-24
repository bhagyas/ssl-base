$ docker build -t alfresco/ssl-base .
$ docker run -v $PWD/keystores:/keystores alfresco/ssl-base
$ docker run -v $PWD/keystores:/keystores -e KEY_SIZE=2048 -e ALFRESCO_VERSION=enterprise alfresco/ssl-base
