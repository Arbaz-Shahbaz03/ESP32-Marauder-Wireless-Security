# ESP32 Marauder — Wireless Vulnerability Testing

> University Cybersecurity Project | Educational Lab Demo | Authorized Use Only

---

## Overview

This project demonstrates wireless security vulnerabilities using the **ESP32 Marauder** — an open-source firmware built on the affordable ESP32 microcontroller.

The goal is to understand how common Wi-Fi attacks work from a defensive perspective, so we can better protect against them. All testing was done on an isolated lab network with full authorization — no real users or external networks were targeted.

---

## Demos

| Attack | Description |
|--------|-------------|
| Wi-Fi Scanner | Lists nearby SSIDs, channels, RSSI, and encryption type |
| Deauthentication | Forces clients to disconnect from a target AP |
| Evil Portal / Evil Twin | Creates a rogue AP with a fake captive login page |
| Packet / Probe Sniffing | Captures probe requests from nearby devices |

Demo videos are in the `/demo` folder.

---

## Hardware Used

- ESP32 Dev Board (WROOM / WROVER)
- USB power supply / power bank
- OLED display (optional)
- MicroSD card module (optional)
- Isolated test router + test device

---

## Project Structure

```
esp32-marauder-wireless-security/
├── README.md
├── report/
│   └── ESP32_Report.docx
├── slides/
│   └── presentation.pptx
├── demo/
│   ├── evil_portal_demo.mp4
│   └── deauth_demo.mp4
└── images/
    └── setup.jpg
```

---

## Key Findings

- Open networks are still common and traffic on them is fully visible
- Evil twin APs are indistinguishable from real ones without careful attention
- Devices passively leak previously connected network names via probe requests
- Deauth attacks work on WPA2 and require no credentials to execute

---

## Prevention Tips

- Use HTTPS + a trusted VPN on public Wi-Fi
- Disable auto-connect on your devices
- Always verify the exact SSID before connecting
- Use WPA3 if your router supports it
- Enable MFA on important accounts

---

## Disclaimer

This project is strictly for **educational purposes**. All testing was performed on an authorized, isolated lab network. Do not use any of these techniques on networks or devices you do not own or have explicit permission to test.

---

## Contribution

 Arbaz Shahbaz
 BITF24M049
 BSIT(MOR)

## References

- [ESP32 Marauder](https://github.com/justcallmekoko/ESP32Marauder)
- OWASP Wireless Security Testing Guide
- NIST SP 800-97
