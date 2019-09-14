# A Simple Docker Example on Mac with a PHP 7.2 / Apache container

## Install and run Docker Desktop for Mac
Download it here: https://hub.docker.com/editions/community/docker-ce-desktop-mac


```bash
# build it
docker build -t hello-docker .

# run it
docker run -p 80:80 -v /Users/yourusername/Projects/docker-example/src/:/var/www/html/ hello-docker

```

The `-v` option mounts a local directory on your machine inside the container, so changes to your code will show up instantly at `http://localhost`.
