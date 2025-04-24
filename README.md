# 🪫 Battery Alert: Shopping List & ToDo – Home Assistant Blueprint

This Home Assistant automation blueprint helps you track low battery levels in your smart home and take action automatically.

![Battery Alert Blueprint Banner](https://raw.githubusercontent.com/alles-automatisch/battery-shopping-blueprints/main/docs/banner.png)

---

## ⚡ What It Does

- Monitors a battery sensor (e.g. `sensor.motion_sensor_battery`)
- Adds an item to the [Shopping List](https://www.home-assistant.io/integrations/shopping_list/)
- Creates a task in the internal [ToDo List](https://www.home-assistant.io/integrations/todo/)
- Prevents duplicates using an `input_boolean`
- Resets itself when the battery level goes back above the recovery threshold

---

## 🧠 Why This Is Awesome

No more guessing which battery is about to die. This automation helps you:
- Stay organized
- Never forget to buy replacements
- Be reminded to actually swap out batteries

---

## 📥 Import This Blueprint

[![Open in Home Assistant](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/alles-automatisch/battery-shopping-blueprints/main/blueprints/automation/allesautomatisch/battery_alert.yaml)

---

## 🔧 Requirements

You can optionally use your own `input_boolean` helper to control one-time execution per device.
Otherwise, the blueprint will auto-generate a name like:  
`input_boolean.battery_alert_motion_sensor_battery`

You may need to manually create the input_boolean if it doesn’t already exist via:
**Settings → Devices & Services → Helpers → + Add Helper → Toggle**

---

## 🙌 Created by

**Daniel Boberg – [Alles Automatisch](https://www.youtube.com/@AllesAutomatisch)**

- 🎥 YouTube: [youtube.com/@AllesAutomatisch](https://www.youtube.com/@AllesAutomatisch)
- 💡 Snippets: [alles-automatisch.de/snippets](https://alles-automatisch.de/snippets)
- 🌐 Website: [alles-automatisch.de](https://alles-automatisch.de)

If you like it, drop a ⭐️ on GitHub or subscribe on YouTube. Enjoy!
