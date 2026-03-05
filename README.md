## OnePlus Pad 3 Porting Status

| Feature                    | Status |
| :------------------------- | :----: |
| **CPU**                    | ✅     |
| **Internal Storage**       | ✅     |
| **Display**[^1][^2]        | ✅     |
| **USB Host Mode**          | ✅     |
| **USB Device Mode**        | ✅     |
| **Side Buttons**           | ✅     |
| **Flashlight**             | ✅     |
| **Charging**[^3]           | ⚠️     |
| **WLAN**                   | ❔     |
| **Bluetooth**              | ❔     |
| **Touchscreen**            | ❔     |
| **Battery**                | ❔     |
| **Microphone**             | ❔     |
| **Speakers**[^4][^5]       | ❔     |
| **Oneplus Smart Keyboard** | ❔     |
| **Oneplus Stylo**[^6]      | ❌     |
| **GPU**[^7]                | ❌     |
| **USB PD**                 | ❌     |
| **Display Port**[^8]       | ❌     |
| **Camera**                 | ❌     |
| **Accel. Sensor**          | ❌     |
| **Compass Sensor**         | ❌     |
| **Gyroscope Sensor**       | ❌     |
| **Temp. Sensor**           | ❌     |
| **NFC Sensor**[^9]         | ❔     |
| **GPS**                    | ❌     |
| **Haptics**[^9]            | ❔     |

## To-do:
> [!NOTE]
> Sorted by: priority (high to low)

- [ ] Test everything
- [ ] Display (native)[^10]
- [ ] Camera
- [ ] GPU (once upstreamed)
- [ ] Charger[^11]

#### Footnotes

[^1]: Utilises simple frambuffer (UEFI FB), not native (yet)
[^2]: Requires `mdss` to be upstreamed
[^3]: No driver for sc8547a, so charging depends on qcom glink and is very slow. Also, no indication.
[^4]: May have to be changed to `aw88261` (All I know is that it's aw882xx)
[^5]: Interestingly, there are only 6 nodes (in dt) for `aw882xx` while Oneplus advertised 8 speakers (the same 6 node config is also found in Oneplus Pad Pro, so idk)
[^6]: Needs touchpanel integration, no driver for cps8601
[^7]: Requires mainline support
[^8]: Requires `DP` to be upstreamed
[^9]: Part of Keyboard Accessory
[^10]: Driver is present, but untested[^2]
[^11]: May not be possible, since the downstream driver is heavily wrapped with oneplus vooc functions.
---
