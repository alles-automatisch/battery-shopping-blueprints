# 🪫 Battery Alert: ToDo Lists – Home Assistant Blueprint

![Battery Alert Banner](https://raw.githubusercontent.com/alles-automatisch/battery-shopping-blueprints/main/docs/banner.png)

This Home Assistant blueprint monitors a battery sensor and automatically creates ToDo entries in two separate lists:

- A shopping item (e.g. "Battery for Motion Sensor")
- A battery replacement task (e.g. "Replace battery in Motion Sensor")

## ✅ Features

- Works with any `sensor.*` battery level
- Uses two customizable `todo.*` lists
- No helpers, plugins, or HACS integrations needed
- Supports clean `use_blueprint:` integration
- Fully local and secure

## 📥 Import Blueprint

[![Open in Home Assistant](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/alles-automatisch/battery-shopping-blueprints/main/blueprints/automation/allesautomatisch/battery_alert.yaml)

## ✍️ Example Usage

```yaml
use_blueprint:
  path: allesautomatisch/battery_alert.yaml
  input:
    battery_sensor: sensor.motion_sensor_battery
    battery_name: Motion Sensor
    threshold: 20
    todo_list_shopping: todo.shopping
    todo_list_tasks: todo.home