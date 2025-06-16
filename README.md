# 🚀 Mountzilla: DIY Harmonic Equatorial Mount
*A mount so strong, NASA blocked me.*

Mountzilla started as a crazy idea: *“If my Pixel phone can capture galaxies standing still… what if it tracked the stars too?”*  
That question cost me **450 JDs**, several weekends, and most of my desk space — but the result? A DIY harmonic equatorial mount so capable, it made NASA nervous.

I built Mountzilla to prove you don’t need to sell a kidney for precision tracking. Harmonic drive mounts are normally *outrageously expensive*, so I set out to build one myself — cheap, powerful, and fully open-source.

Inspired by amazing open projects like [AlkaidMount](https://github.com/alanzjl/AlkaidMount) and [DHEM](https://github.com/polvinc/DHEM), Mountzilla uses a harmonic drive, GT2 pulley system, and OnStepX firmware to deliver rock-solid accuracy and ridiculous payload capacity — all while being way too fun to build.


---

## 🧠 Features

- ⚙️ **Harmonic Drive** – CSG 25-100-2A  
- 🔩 **Pulley Reduction** – 5:1 GT2 belt drive  
- 🌀 **Stepper Motors** – NEMA 23 (400 steps, 0.9°, 23HM22-2804S)  
- 🧠 **Controller** – FYSETC E4 running OnStepX  
- ⏱️ **Time Sync** – RTC included  
- 🧱 **Mount Base** – Custom powerful Tangent-Style DIY Wedge  
- 📸 **Astro-Ready** – Tested with Pixel 8 Pro 5x (Astro mode, and trust me it's fantastic)
- 🧲 **Payload** – Tested with 30–40 kg capacity (it can hold more)  
- 🤖 **Voice Control** – Compatible with Gemini for hands-free control(need extra work & **external PC** to run Gemini api)  

---

## 📁 Repository Structure

```
Mountzilla/
├── Firmware/
│   └── Mountzilla_OnStepX_Config
├── Design_Files/
│   ├── dovetail
│   └── motor_housing
│   └── wedge
├── Guides/
│   └── build_guide.md
├── Docs/
│   └── BOM.md
```

---

## 🛠️ Getting Started
Before diving in, a moment of silence for your wallet... (or just grab a big coffee!)

1.  Clone the repo
    ```bash
    git clone [https://github.com/jabb4man/Mountzilla.git](https://github.com/jabb4man/Mountzilla.git)
    ```
2.  Gather all necessary components from the [Bill of Materials](docs/BOM.md).
3.  Fabricate parts using the SolidWorks files found in `Design_Files/` (e.g., export to STL for 3D printing or DXF for CNC).
4.  Flash OnStepX to the FYSETC E4 board using the configuration provided in `firmware/Mountzilla_OnStepX_Config`.
5.  Build the mount following the detailed instructions in [`/guides/build_guide.md`](guides/build_guide.md).
6.  Connect via USB/Wi-Fi and control using any OnStep client (e.g., Stelalrium, ASCOM/INDI drivers).
7.  For guiding, use PHD2 with a webcam or dedicated guide camera. 

---

## 🧪 Performance

| Specification         | Value                               |
|-----------------------|-------------------------------------|
| RA RMS Error          | ~0.5–1.5 arcsec (tested)            |
| DEC Slew Speed        | Up to 5°/s                          |
| Max Payload           | 30–40 kg (it can hold more)         |
| Voice Control         | Gemini (need extra work)            |
| Total Gear Ratio      | 400:1 (100:1 gear * 5:1 Pulley)     |
| Resolution            | ~0.14 arcsec/step (calculated)      |
| Materials             | Aluminum or Steel for more cheap    |
| Estimated Cost        | ~Approx. $450 to $600 depend on BOM |

---

## 📷 Gallery

Coming soon: build photos, test shots, time-lapses, and memes :).

---

## 🥔 Credits

Created by [Rami Azap](https://github.com/ramiazap)  
Powered by: OnStepX, FYSETC, caffeine, and stubbornness.

Special thanks to:  
**Wesam Khaled, Afnan AbuQlesha, Raed Abushekha, Sadeen Srour**  
and honorary AI co-developers: **ChatGPT & Gemini**

---

## 📜 License

MIT License — fork it, tweak it, and launch it to the stars.

> "Built a telescope mount because IKEA didn’t sell one."  
