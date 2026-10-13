<h3 align="center">oxpoe</h3>
<p align="center"><em>Linux ↔ hardware tinkering · reverse engineering for interoperability</em></p>

<p align="center">
  <a href="https://github.com/oxpoe/Gamemax-linux-apps/releases/latest"><img alt="GAMEMAX LCD release" src="https://img.shields.io/github/v/release/oxpoe/Gamemax-linux-apps?color=def750&label=GAMEMAX%20LCD"></a>
  <a href="https://github.com/oxpoe/Gamemax-linux-apps/blob/main/LICENSE"><img alt="MIT" src="https://img.shields.io/badge/license-MIT-def750"></a>
  <a href="https://donasi.oxpoe.qzz.io/"><img alt="Donate" src="https://img.shields.io/badge/%E2%9D%A4-donate-def750"></a>
</p>

---

### ★ Featured: GAMEMAX LCD — a Windows-only cooler panel, running on Linux

The LCD block of a GAMEMAX **IceBurg Digital** AIO cooler ships only with a Windows
application. I reverse engineered the panel's HID protocol from that app and rebuilt the
part that matters for Linux:

- **Sender** — pure-stdlib Python: reads `hwmon`/`/proc`/`sysfs`, streams the exact
  65-byte HID report the firmware expects (CPU/GPU temp, load, clocks, fans, power, RAM, disk)
- **Tray app** — PySide6: animated gauge, fan-channel and temperature-source pickers,
  blank mode, autostart, single instance, plug & play on replug
- **AppImage** released by CI, plus `udev` rule and `systemd` user unit

[Repository](https://github.com/oxpoe/Gamemax-linux-apps) ·
[Releases](https://github.com/oxpoe/Gamemax-linux-apps/releases) ·
[Reverse-engineering notes](https://github.com/oxpoe/Gamemax-linux-apps/blob/main/docs/reverse-engineering.md)

### How I like to work

- **Reverse engineering for interoperability** — read the shipped binaries, map the
  protocol, document the evidence, then write the smallest thing that works
- **No dependencies where the platform already provides it** — `hidraw`, `hwmon`, `systemd`
- **Honest tooling** — state the limits (what the firmware cannot do, what was verified
  on real hardware and what was not)

### Support

If something I built saved you time: ❤ **<https://donasi.oxpoe.qzz.io/>**
