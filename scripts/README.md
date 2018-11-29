# imagebuilder

## `Dockerfile.image`

```
$ cd imagebuilder-qemu-aarch64/scripts

$ docker build --force-rm --squash --file Dockerfile.image -t imagebuilder-qemu-aarch64 .
```

## `/vos_run`

```
$ docker run --rm --privileged=true -ti -v $(pwd):/home/builder/src -v /dev:/dev -v /tmp:/tmp \
    imagebuilder-qemu-aarch64 /vos_run
```
