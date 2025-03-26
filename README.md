

1. ports.sh

2. modify Configuraiton.yaml

3. docker run    --name zigbee2mqtt    --restart=unless-stopped    --device=/dev/serial/by-id/"replace by your serial"    -p 8080:8080    -v $(pwd)/data:/app/data    -v /run/udev:/run/udev:ro    -e TZ=Europe/Zurich    koenkk/zigbee2mqtt
