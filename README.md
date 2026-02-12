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
| **GPS**                    | ❌     |
| **Haptics**                | N/A    |

## To-do:
> [!NOTE]
> Sorted by: priority (high to low)

- [ ] Test everything
- [ ] Display (native)
- [ ] Camera
- [ ] Charger
- [ ] GPU (once upstreamed)

#### Footnotes

[^1]: Utilises simple frambuffer (UEFI FB), not native (yet)
[^2]: Requires `mdss` to be upstreamed
[^3]: No driver for sc8547a
[^4]: Uses two chips: `aw88261` and `sia9196` (unconfirmed)
[^5]: Interestingly, there's only 6 nodes each for both `aw88261` and `sia9196` while Oneplus advertised 8 speakers
[^6]: Needs touchpanel integration
[^7]: Requires mainline support
[^8]: Requires `DP` to be upstreamed

---
