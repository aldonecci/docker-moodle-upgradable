docker-moodle-upgradable
========================

A Dockerfile that installs and runs Moodle stable 3.1.

## Installation

```
git clone https://github.com/aldonecci/docker-moodle-upgradable
cd docker-moodle-upgradable
docker build -t moodle .
```

## Usage

To spawn a new instance of Moodle:

```
docker run -d -P --name moodle --link DB:DB -e MOODLE_URL=http://192.168.127.227:8080 -p 8080:80 moodle
```

You can visit the following URL in a browser to get started:

```
http://192.168.127.227:8080 
```

## Credits
This is by myself
