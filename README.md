## OnePlus Pad 3 Porting Status

| Feature                    | Status |
| :------------------------- | :----: |
| **CPU**.                   | ✅     |
| **Internal Storage**       | ✅     |
| **Display**[^1]            | ✅     |
| **USB Host Mode**          | ✅     |
| **USB Device Mode**        | ✅     |
| **Side Buttons**           | ✅     |
| **Flashlight**             | ✅     |
| **Charging**[^2]           | ⚠️     |
| **WLAN**                   | ❔     |
| **Bluetooth**              | ❔     |
| **Touchscreen**            | ❔     |
| **Battery**                | ❔     |
| **Microphone**             | ❔     |
| **Speakers**[^3]           | ❔     |
| **Oneplus Smart Keyboard** | ❔     |
| **Oneplus Stylo**          | ❌     |
| **GPU**[^4]                | ❌     |
| **USB PD**                 | ❌     |
| **Camera**                 | ❌     |
| **Accel. Sensor**          | ❌     |
| **Compass Sensor**         | ❌     |
| **Gyroscope Sensor**       | ❌     |
| **Temp. Sensor**           | ❌     |
| **GPS**                    | ❌     |
| **Haptics**                | N/A    |

## To-do:
> [!NOTE]
> Sorted by: priority (high to low)

- [ ] Test
- [ ] Display (native)
- [ ] Camera
- [ ] Charger
- [ ] GPU (once upstreamed)

#### Footnotes

[^1]: Utilises simple frambuffer (UEFI FB), not native (yet)
[^2]: No driver for sc8547a
[^3]: Uses two chips: aw88261 and sia9196
[^4]: Requires mainline support

---
