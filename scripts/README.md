# imagebuilder

## `Dockerfile.image`

```
$ cd imagebuilder-qemu-aarch64/scripts

$ docker build --force-rm --network=host --file Dockerfile.image -t imagebuilder-qemu-aarch64 .
```

## `/vos_run`

```
$ docker run --rm --network=host --privileged=true -ti -v $(pwd):/home/builder/src -v /dev:/dev -v /tmp:/tmp \
    imagebuilder-qemu-aarch64 /vos_run
```
