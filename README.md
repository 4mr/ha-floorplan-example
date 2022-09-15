# Home Assistant Floorplan Example

https://user-images.githubusercontent.com/78191171/190462547-12e55c77-c7e6-46ef-9d15-3f49898ce00b.mp4

### Было использовано

* Docker 
* Docker Compose
* [Inkscape](https://inkscape.org/) для редактирования SVG
* [Sweet Home 3D](https://www.sweethome3d.com/) для создания 3D плана
* [Home Assistant](https://www.home-assistant.io/)
* [HA Floorplan](https://github.com/ExperienceLovelace/ha-floorplan/)
* [Kiosk Mode](https://github.com/maykar/kiosk-mode)

### Установка

```
git clone https://github.com/4mr/ha-floorplan-example/
cd ha-floorplan-example
docker compose up -d
```

После установки откройте http://IP:8123/ и произведите первичную настройку Home Assistant.

Если Вы используете Wirenboard то добавьте устройства в Home Assistant используя модуль [wb-mqtt-homeassistant](https://github.com/4mr/wb-mqtt-homeassistant).

Для корректной работы примера необходимо чтобы id устройств в Home Assistant совпадали (можно переименовать id необходимых устройств в Home Assistant) с id в yaml/svg файлах.

В примере использованы следующие id:
* Зоны освещения: light.light_1, light.light_2, light.light_3, light.light_4, light.light_5_1, light.light_5_2, light.light_6_1, light.light_6_2
* Датчики температуры: sensor.temperature_2, sensor.temperature_3, sensor.temperature_4, sensor.temperature_6
* Датчики влажности: sensor.humidity_2, sensor.humidity_3, sensor.humidity_4, sensor.humidity_6
* Датчики движения: binary_sensor.motion_3, binary_sensor.motion_6
* Датчик CO2: sensor.co2_6
* Датчик VOC: sensor.voc_2
