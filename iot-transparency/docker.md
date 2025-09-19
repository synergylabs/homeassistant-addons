# Docker setup

If you are setting up a Docker installation of IoT Transparency, there are a few additional steps to enable packet forwarding and set up the integration with Home Assistant.

## Configure packet forwarding

IoT Transparency intercepts traffic going to and from your IoT devices to allow it to display the traffic to you.
To do so, your system must be configured to allow packet forwarding/routing.

Enable IP forwarding using:

```
sudo sysctl -w net.ipv4.ip_forward=1
```

Additionally, your firewall must be configured to allow forwarding.
Some sample configurations are below:

UFW:

```
sudo ufw default allow FORWARD
```

iptables:

```
sudo iptables -P FORWARD ACCEPT
```

## Create Home Assistant API token

IoT Transparency uses the Home Assistant API to access a list of devices in your home.

Create an API token by going to Home Assistant -> User profile (bottom left) -> Security -> Long-lived access tokens -> Create token.

Save this token for the next step.

## Configure and start container

1. Download [docker-compose.yml](docker-compose.yml) and [iot-transparency.env](iot-transparency.env) and place them in the same directory on your server
2. If running on an ARM machine, change `ghcr.io/synergylabs/iot-transparency-amd64` to `ghcr.io/synergylabs/iot-transparency-arm64` in `docker-compose.yml`
3. Update the `HA_URL` field of the `iot-transparency.env` file with the correct domain name and port for your Home Assistant server
4. Update the `SUPERVISOR_TOKEN` field of the `iot-transparency.env` file with the token you just generated

Then, you can start the Docker container using:

```
$ docker compose up
```

## Help

Please contact us at [mailto:iot-transparency@andrew.cmu.edu](iot-transparency@andrew.cmu.edu) if you need help troubleshooting any issues.
