# WiFi-DoS

A Python-based WiFi deauthentication tool for security testing and educational purposes.

![Python](https://img.shields.io/badge/Python-3.6+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Platform](https://img.shields.io/badge/Platform-Linux-orange.svg)

## ⚠️ Disclaimer

**This tool is for educational and authorized security testing purposes only.**

Using this tool against networks you don't own or don't have explicit permission to test is **illegal** and unethical. The author is not responsible for any misuse of this software.

## Features

- Automatic detection of wireless interfaces
- Real-time scanning of nearby WiFi networks
- Target selection with BSSID and channel information
- Continuous deauthentication attack capability

## Requirements

### System Requirements
- Linux (Kali Linux recommended)
- Wireless adapter with monitor mode support
- Root/sudo privileges

### Dependencies
```bash
# Install aircrack-ng suite
sudo apt update
sudo apt install aircrack-ng wireless-tools
```

### Python
- Python 3.6 or higher
- No external Python packages required (uses standard library only)

## Installation

```bash
# Clone the repository
git clone https://github.com/aradhyacp/Wifi-dos.git

# Navigate to the directory
cd Wifi-dos

# Make the script executable (optional)
chmod +x main.py
```

## Usage

```bash
# Run with sudo privileges
sudo python3 main.py
```

### Steps:
1. Select your wireless interface
2. Wait for networks to appear (Ctrl+C to stop scanning)
3. Select target network by number
4. Attack runs until you press Ctrl+C

## How It Works

1. **Interface Detection** - Detects available wireless interfaces
2. **Monitor Mode** - Puts the selected interface into monitor mode
3. **Network Scanning** - Uses airodump-ng to discover nearby networks
4. **Deauthentication** - Sends deauth packets to disconnect clients from the target network

## Legal Notice

This tool should only be used:
- On networks you own
- On networks you have written permission to test
- In controlled lab environments for learning

Unauthorized access to computer networks is a criminal offense in most jurisdictions.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Author

**@aradhyacp**
- GitHub: [https://github.com/aradhyacp](https://github.com/aradhyacp)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⭐ Star This Repo

If you find this project useful, please consider giving it a star!
