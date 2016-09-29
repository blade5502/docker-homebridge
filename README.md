# docker: homebridge (with indigo plugin)

This is a docker image to run the [homebridge tool](https://github.com/nfarina/homebridge) with the 
[homebridge-lifx plugin](https://www.npmjs.com/package/homebridge-lifx) enabled.

### Build from docker file

If you want to build the docker container image yourself you can do so with the
following commands:

```bash
git clone git@github.com:blade5502/docker-homebridge.git
cd docker-homebridge
docker build -t homebridge .
```

### Pulling from docker hub

If you just want to obtain the image from the docker registry, you can use the
following command:

```bash
docker pull blade5502/homebridge
```

### Running the image

In order to run the homebridge server command in daemonized mode, use the following:

```bash
docker run -d --net="host" -v /PATH_TO_HOMEBRIDGE_CONFIG_DIRECTORY:/config blade5502/homebridge
```

