# MqttLedController
Control leds using https://home-assistant.io/components/light.mqtt_json/ and mqtt
https://www.youtube.com/watch?v=V6dNrCIA-V0&spfreload=5

# Installation

Clone this repository to `/home/pi` directory then run this commands:

```
cd /home/pi/snips-aiy
pip install -r requirements.txt

cp mqtt.yaml.example ~/.config/mqtt.yaml
```

Edit configuration under `~/.config/mqtt.yaml` and after that run:

```
sudo cp systemd/mqtt-light.service /lib/systemd/system/
sudo systemctl enable mqtt-light
sudo systemctl start mqtt-light
```
