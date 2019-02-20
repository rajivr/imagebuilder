# imagebuilder

## `Dockerfile.image`

```
$ cd imagebuilder

$ docker build --force-rm --squash --file Dockerfile.image -t imagebuilder .
```

## `/vos_run`

```
$ docker run --rm --privileged=true -ti -v $(pwd):/home/builder/src -v /dev:/dev -v /tmp:/tmp \
    imagebuilder /vos_run
```
