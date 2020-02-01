# Cookiecutter Docker Container

Pull Cookiecutter templates in a Docker container without setting up a Python environment. 

Forked from [Audreyr docker-cookiecutter](https://github.com/audreyr/docker-cookiecutter).

[Docker Hub repo available here.](https://hub.docker.com/r/michaeltinsley/cookiecutter/)


# Usage

A sample command:

Change the `TEMPLATE` variable to your Cookiecutter repository.
 
```shell script	
docker run -it --rm \
	-e LC_ALL=C.UTF-8 \
	-e TEMPLATE=gh:pawamoy/cookiecutter-awesome \
	-e OUT_DIR=/cookie \
	-v $(PWD):/cookie \
	michaeltinsley/cookiecutter
```

# Contributing

To set it up for local development:

```shell script
git clone https://github.com/michaeltinsley/docker-cookiecutter.git
cd docker-cookiecutter
docker build -t cookiecutter .
docker run -t cookiecutter
```


