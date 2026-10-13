<div align="center">

<a href="https://github.com/oxpoe/Gamemax-linux-apps">
  <img src="https://raw.githubusercontent.com/oxpoe/Gamemax-linux-apps/main/assets/social-preview.png" alt="GAMEMAX LCD — Linux bridge" width="100%">
</a>

<a href="https://github.com/oxpoe">
  <img src="https://readme-typing-svg.demolab.com?font=Noto+Sans&weight=700&size=28&pause=1200&color=DEF750&center=true&vCenter=true&width=760&lines=Linux+%E2%86%94+hardware+tinkering;Reverse+engineering+for+interoperability;Making+Windows-only+devices+work+on+Linux" alt="oxpoe">
</a>

<p>
  <a href="https://github.com/oxpoe/Gamemax-linux-apps/releases/latest"><img alt="release" src="https://img.shields.io/github/v/release/oxpoe/Gamemax-linux-apps?color=def750&label=GAMEMAX%20LCD&style=for-the-badge"></a>
  <a href="https://github.com/oxpoe/Gamemax-linux-apps/blob/main/LICENSE"><img alt="license" src="https://img.shields.io/badge/license-MIT-def750?style=for-the-badge"></a>
  <a href="https://donasi.oxpoe.qzz.io/"><img alt="donate" src="https://img.shields.io/badge/%E2%9D%A4-donate-def750?style=for-the-badge"></a>
</p>

<p>
  <img alt="Linux" src="https://img.shields.io/badge/Linux-141614?style=flat-square&logo=linux&logoColor=def750">
  <img alt="Python" src="https://img.shields.io/badge/Python-141614?style=flat-square&logo=python&logoColor=def750">
  <img alt="Qt / PySide6" src="https://img.shields.io/badge/PySide6-141614?style=flat-square&logo=qt&logoColor=def750">
  <img alt="systemd" src="https://img.shields.io/badge/systemd-141614?style=flat-square&logo=systemd&logoColor=def750">
  <img alt="Ghidra" src="https://img.shields.io/badge/Ghidra-141614?style=flat-square&logo=ghidra&logoColor=def750">
  <img alt="Git" src="https://img.shields.io/badge/Git-141614?style=flat-square&logo=git&logoColor=def750">
</p>

</div>

---

## ★ Featured — GAMEMAX LCD

An AIO cooler whose LCD panel only spoke to a Windows application. I reverse engineered the
panel's HID protocol from that app and rebuilt the useful part for Linux: a dependency-free
sender that streams the exact 65-byte report the firmware reads, plus an animated PySide6
tray app with fan/temperature channel pickers, systemd autostart and plug & play. AppImage
built by CI.

[**Repository**](https://github.com/oxpoe/Gamemax-linux-apps) · [**Releases**](https://github.com/oxpoe/Gamemax-linux-apps/releases) · [**Reverse-engineering notes**](https://github.com/oxpoe/Gamemax-linux-apps/blob/main/docs/reverse-engineering.md)

## How I work

- **Reverse engineering for interoperability** — read the shipped binaries, map the protocol, keep the evidence
- **Use what the platform already gives you** — `hidraw`, `hwmon`, `systemd`; no dependencies where it counts
- **Say what was verified** — on real hardware, and which limits belong to the firmware

<div align="center">

<a href="https://github.com/oxpoe">
  <img height="160" alt="stats" src="https://github-readme-stats.vercel.app/api?username=oxpoe&show_icons=true&hide_border=true&bg_color=141614&title_color=def750&icon_color=def750&text_color=e8ece8&include_all_commits=true&rank_icon=github">
</a>
<a href="https://github.com/oxpoe">
  <img height="160" alt="languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=oxpoe&layout=compact&hide_border=true&bg_color=141614&title_color=def750&text_color=e8ece8&langs_count=6">
</a>

<a href="https://github.com/oxpoe">
  <img alt="streak" src="https://streak-stats.demolab.com?user=oxpoe&hide_border=true&background=141614&stroke=2a2e2a&ring=def750&fire=def750&currStreakLabel=def750&sideLabels=e8ece8&dates=a9b0a9&currStreakNum=e8ece8&sideNums=e8ece8">
</a>

<img alt="contribution snake" src="https://raw.githubusercontent.com/oxpoe/oxpoe/output/snake.svg">

<p><sub>❤ If something I built saved you time: <a href="https://donasi.oxpoe.qzz.io/">donasi.oxpoe.qzz.io</a></sub></p>

</div>
