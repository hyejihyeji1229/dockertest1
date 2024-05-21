# dockerfiles-ubuntu-user-adderable
Ubuntu, It support base user creation and password setting.

# Building & Running

Copy the sources to your docker host and build the container, and to run.
```
	docker build   --rm -t hyeji2929/ubuntu:test .
	docker run -it --rm --name u1  hyeji2929/ubuntu:test
```
Get the port that the container is listening on:

```
# docker ps
CONTAINER ID        IMAGE                COMMAND             CREATED             STATUS              PORTS               NAMES
fc199e02d300        hyeji2929/ubuntu:test   "/bin/bash"         41 seconds ago      Up 40 seconds                           u1
```

To test, ("hyeji2929" is username. )
```
	tree
```
To Rollback
```
    docker rm u1 -f
    docker rmi hyeji2929/ubuntu:test
```
