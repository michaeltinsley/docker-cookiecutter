# docker-cookiecutter


Run Cookiecutter in a Docker container.

Docker Hub repo: https://hub.docker.com/r/cookiecutter/cookiecutter/


# Usage	# Usage

A sample command:
```bash	
docker run -it --rm \
	-e LC_ALL=C.UTF-8 \
	-e TEMPLATE=gh:pydanny/cookiecutter-django \
	-e OUT_DIR=/cookie \
	-v $(PWD):/cookie \
	cookiecutter/cookiecutter
```	```

# Contributing

To set it up for local development:

```
git clone https://github.com/audreyr/docker-cookiecutter.git
cd docker-cookiecutter
docker build -t cookiecutter .
docker run -t cookiecutter
```
