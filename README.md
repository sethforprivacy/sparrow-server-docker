# sparrow-server-docker

A simple Docker image for Sparrow Wallet Server

## How to Use

You can run the docker command with:

```shell
docker run --rm -it --net=host -v $HOME/.sparrow:/home/sparrow/.sparrow ghcr.io/sethforprivacy/sparrow-server:latest
```

* `--rm` automatically remove the container when it exits
* `-i` is interactive (you need to use the wallet)
* `-t` is TTY (you need to use the wallet)
* `--net=host` shares the host network with the container
* `-v $HOME/.sparrow:/home/sparrow/.sparrow` mounts the `.sparrow/` dir in the container.
  Uses the default path for Sparrow Wallet.

## Credits

All credit for Sparrow Wallet goes to the incredible Craig Raw: https://sparrowwallet.com/
