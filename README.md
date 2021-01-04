# ATutor Docker Setup

This was created to practice before starting the Offensive Security AWAE course.

### How to start

Ensure you have Docker and docker-compose. Then run the following commands:

```
$ git clone https://github.com/bad5ect0r/atutor-docker.git
...
$ cd atutor-docker
$ docker-compose up
...
```

The App/atutor.conf file is an Apache config for a virtual host. You can make appropriate changes, but the default requires that you have an entry in your `/etc/hosts` file like so:

```
127.0.0.1   localhost atutor
```

Then you can browse to `http://atutor:8080`.
