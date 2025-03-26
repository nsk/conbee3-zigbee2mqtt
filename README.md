

1. ports.sh

2. modify Configuraiton.yaml

3. docker run    --name zigbee2mqtt    --restart=unless-stopped    --device=/dev/serial/by-id/usb-dresden_elektronik_ConBee_III_DE03186404-if00-port0:/dev/ttyUSB0    -p 8080:8080    -v $(pwd)/data:/app/data    -v /run/udev:/run/udev:ro    -e TZ=Europe/Zurich    koenkk/zigbee2mqtt
