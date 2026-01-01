# 📶 WiFi-DoS

### Advanced WiFi Deauthentication Tool for Security Testing

[![Python](https://img.shields.io/badge/Python-3.6+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://www.linux.org/)
[![Kali Linux](https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)](https://www.kali.org/)
[![Security](https://img.shields.io/badge/Security-Pentesting-red?style=for-the-badge&logo=hackaday&logoColor=white)]()

<p align="center">
  <img src="https://img.shields.io/github/stars/aradhyacp/Wifi-dos?style=social" alt="Stars">
  <img src="https://img.shields.io/github/forks/aradhyacp/Wifi-dos?style=social" alt="Forks">
  <img src="https://img.shields.io/github/watchers/aradhyacp/Wifi-dos?style=social" alt="Watchers">
</p>

---

**WiFi-DoS** is a professional-grade Python automation tool designed for security researchers and network administrators. It streamlines WiFi deauthentication attacks using the `aircrack-ng` suite, enabling efficient testing of network resilience and wireless security.

```
╔═══════════════════════════════════════════════════════════════════╗
║                                                                   ║
║    _  _  _ _____ _______ _____     ______   _____  _______        ║
║    |  |  |   |   |______   |   ___ |     \ |     | |______        ║
║    |__|__| __|__ |       __|__     |_____/ |_____| ______|        ║
║                                                                   ║
╚═══════════════════════════════════════════════════════════════════╝
```

---

## ⚠️ Disclaimer

> **This tool is for educational and authorized security testing purposes only.**
>
> Using this tool against networks you don't own or don't have explicit permission to test is **illegal** and unethical. The author is not responsible for any misuse of this software. It is the end user's responsibility to obey all applicable local, state, and federal laws.

---

## 📖 Table of Contents

- [Features](#-features)
- [How It Works](#-how-it-works)
- [Requirements](#-requirements)
- [Installation](#-installation)
- [Usage](#-usage)
- [Project Structure](#-project-structure)
- [Screenshots](#-screenshots)
- [Contributing](#-contributing)
- [License](#-license)
- [Author](#-author)

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🔍 **Auto Interface Detection** | Automatically detects available wireless interfaces |
| 🚀 **Automated Monitor Mode** | Switches your wireless card into monitor mode seamlessly |
| 📡 **Real-time AP Scanning** | Displays nearby networks with BSSID, Channel & ESSID |
| 🎯 **Targeted Attacks** | Select specific networks for deauthentication |
| 🧹 **Auto Cleanup** | Automatically cleans up CSV files and restores interface on exit |
| ✅ **Tool Validation** | Checks for required dependencies before running |
| 💻 **Beautiful CLI** | Clean, intuitive interface with formatted tables |

---

## 🔄 How It Works

1. **Interface Detection** — Identifies available wireless interfaces (`wlan0`, etc.)
2. **Monitor Mode** — Kills conflicting processes and enables monitor mode
3. **Network Scanning** — Uses `airodump-ng` to discover nearby access points
4. **Target Selection** — Interactive menu to select target network
5. **Deauthentication** — Sends deauth packets to disconnect clients
6. **Cleanup** — Restores interface and removes temporary files

---

## 🛠 Requirements

### System Requirements

| Requirement | Description |
|-------------|-------------|
| **OS** | Linux (Kali Linux recommended) |
| **WiFi Adapter** | Must support Monitor Mode & Packet Injection |
| **Privileges** | Root/sudo access required |

### Dependencies

```bash
# Update system and install dependencies
sudo apt update && sudo apt upgrade -y
sudo apt install aircrack-ng wireless-tools python3 -y
```

### Python

- Python 3.6 or higher
- **No external packages required** (uses standard library only)

---

## 🚀 Installation

```bash
# Clone the repository
git clone https://github.com/aradhyacp/Wifi-dos.git

# Navigate to the directory
cd Wifi-dos

# Make the script executable (optional)
chmod +x main.py
```

---

## 💻 Usage

```bash
# Run with sudo privileges
sudo python3 main.py
```

### Workflow

| Step | Action |
|------|--------|
| 1️⃣ | Select your wireless interface from the list |
| 2️⃣ | Wait for networks to appear in the scan table |
| 3️⃣ | Press `Ctrl+C` when ready to select a target |
| 4️⃣ | Enter the number of the target network |
| 5️⃣ | Attack runs until you press `Ctrl+C` again |

### Example Output

```
┌─────┬───────────────────┬─────────┬────────────────────────────────┐
│ No  │ BSSID             │ Channel │ ESSID                          │
├─────┼───────────────────┼─────────┼────────────────────────────────┤
│ 0   │ AA:BB:CC:DD:EE:FF │    6    │ HomeNetwork                    │
│ 1   │ 11:22:33:44:55:66 │   11    │ CoffeeShop_WiFi                │
└─────┴───────────────────┴─────────┴────────────────────────────────┘
```

---

## 📂 Project Structure

```
Wifi-dos/
├── main.py            # Main script with all automation logic
├── requirements.txt   # Python dependencies (standard library)
├── LICENSE            # MIT License
├── .gitignore         # Git ignore rules
└── Readme.md          # This file
```

---

## 🖼 Screenshots

> Coming soon! Screenshots of the tool in action.

---

## 🤝 Contributing

Contributions are what make the open-source community amazing! Any contributions are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📜 License

Distributed under the **MIT License**. See [LICENSE](LICENSE) for more information.

---

## 👤 Author

**Aradhya CP** — [@aradhyacp](https://github.com/aradhyacp)

[![GitHub](https://img.shields.io/badge/GitHub-aradhyacp-181717?style=for-the-badge&logo=github)](https://github.com/aradhyacp)

---

## ⭐ Star This Repo

If you find this project useful, please consider giving it a star! It helps others discover the project.

---

## 🏷️ Topics

`wifi` `wifi-hacking` `deauth` `deauthentication` `deauth-attack` `wifi-deauther` `wireless` `wireless-security` `network-security` `penetration-testing` `pentesting` `ethical-hacking` `hacking-tool` `security-tools` `aircrack-ng` `kali-linux` `python` `cybersecurity` `infosec` `red-team`

---

<p align="center">
  <b>Made with ❤️ for the Cybersecurity Community</b>
</p>
