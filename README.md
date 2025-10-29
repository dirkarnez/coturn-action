coturn-action
=============
[coturn/coturn: coturn TURN server project](https://github.com/coturn/coturn)

### DevTunnel
- See [dirkarnez/devtunnel-playground](https://github.com/dirkarnez/devtunnel-playground)

### Web UI
- `https://${Tunnel ID}.devtunnels.ms:8080/`

### Tools
- [Trickle ICE](https://webrtc.github.io/samples/src/content/peerconnection/trickle-ice/)

### Notes
- `sudo chmod -R +x . && ./build.sh` in CI/CD .yaml file is good enough for running docker build on GitHub Action
- too busy - use Docker image instead
  - `docker run -d -p 3478:3478 -p 3478:3478/udp -p 5349:5349 -p 5349:5349/udp -p 49152-65535:49152-65535/udp coturn/coturn`
    - [coturn/docker/coturn/README.md at master · coturn/coturn](https://github.com/coturn/coturn/blob/master/docker/coturn/README.md)
