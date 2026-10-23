# ⚡ SIMAM (صِمَام) | Smart A/C Circuit Breaker Monitoring System

> **Hajj Research & Innovation Showcase Project**  
> *A wireless IoT monitoring solution for Mina tent A/C Sub-Main Distribution Boards (AC-SMDB), reducing emergency power disruption response times from hours to minutes.*

---

## 📌 Problem Overview
During the Hajj season, ambient temperatures in Mina can exceed $45^\circ\text{C}$. A/C disruptions pose a critical safety and comfort challenge for pilgrims:
- **The Blind Spot:** Power failures frequently occur at the **Sub-Main Distribution Board (AC-SMDB)** level—each feeding 10 to 20 tents.
- **Lack of Digital Signals:** Traditional SCADA systems monitor higher-level sub-stations and smart meters but do not cover individual AC-SMDB units.
- **Manual Troubleshooting:** Maintenance teams must manually inspect hundreds of identical electrical boards in extreme heat to locate a single tripped breaker, leading to prolonged delays.

---

## 💡 The SIMAM Solution
**SIMAM** is an add-on, non-invasive wireless IoT monitoring system designed to overlay directly onto existing AC-SMDB panels without requiring structural or electrical modifications:
- **Instant Fault Signal:** Detects automatic breaker trips immediately and sends pinpoint location telemetry to the central operations dashboard.
- **Smart Auxiliary Switches (OF / SD Contacts):** Distinguishes between scheduled manual maintenance (`OF`) and emergency fault trips (`SD`), completely eliminating false alarms.
- **LoRaWAN Connectivity:** Operates on an isolated 868 MHz spectrum to bypass cellular network congestion during peak Hajj days.
- **Long Battery Life:** Powered by high-durability $\text{Li-SOCl}_2$ batteries lasting 5 to 10 years with ultra-low sleep-mode consumption.

---

## 🏗️ Technical Architecture & Key Components
1. **Auxiliary Switch Module:** Attached to the circuit breaker arm to capture mechanical state changes (`OF` vs `SD`).
2. **Microcontroller & LoRaWAN Transmitter:** Integrated `STM32WLE5` chip for instant interrupt-driven event transmission.
3. **Rugged Industrial Enclosure:** IP65-rated housing resistant to harsh environmental temperatures ($-40^\circ\text{C}$ to $+85^\circ\text{C}$).
4. **Operations Dashboard:** Real-time web-based control panel for continuous status monitoring, automated alerts, and spatial fault visualization.

---

## 📂 Repository Contents
- `presentation/` - Official Innovation Pitch Deck (`__ابتكار صمام_.pdf`)
- `documentation/` - Comprehensive Project Technical & Business Memo (`__مذكرة مشروع صمام_..pdf`)
- `prototype/` - Interactive Dashboard Prototype Access QR Code (`تجربة النموذج الأولي لواجهة مركز التحكم .jpg`)

---

## 👥 SIMAM Team
* **Aseel Zainy** (أسيل زيني)
* **Hala Al-Jawii** (حلا الجاوي)
* **Asal Kalntan** (آصال كلنتن)

*Developed under the auspices of the Custodian of the Two Holy Mosques Institute for Hajj and Umrah Research, Umm Al-Qura University.*
