# Folf Labs SlimeVR Trackers [WIP]
Unofficial (DIY) Smol SlimeVR-compatible trackers powered by Nordic nRF52840 SoC and ICM-45686 IMU. 

## SmolBoard
![photo_2025-08-24_10-34-24](https://github.com/user-attachments/assets/ec8327ec-e5b5-4dbe-9d43-9afd16250137)

SmolBoard is a PCB that sits on top of the SuperMini nRF52840 as an alternative to the [Stacked Slime](https://docs.slimevr.dev/smol-slimes/hardware/smol-tracker.html). It contains the ICM-45686 IMU, a 32.768kHz crystal, a battery switch, and two buttons: SW0 (user button) + RST (reset).

> [!NOTE]
> The battery switch physically disconnects the battery from the rest of the circuit. Keep it switched ON during charging, otherwise the battery won't charge.

> [!WARNING]
> On **rev 1**, the IMU and crystal are powered from the VCC pin.
> The recommended way is to power them through P0.31 (right below the VCC).
> Fix: jumper VCC and P0.31 on the SmolBoard, then solder just the P0.31 on the SuperMini.

### To-Do (Future Revision)
- [ ] Reduce the board width slightly to match the SuperMini
- [X] Power the IMU and crystal via P0.31

## Credits
The enclosure is inspired by Sorakage033's Cheesecake. I own a set of six Cheesecakes, and they're really well designed!

## License
This project is licensed under the [Creative Commons Attribution-NonCommercial 4.0](https://creativecommons.org/licenses/by-nc/4.0/).
