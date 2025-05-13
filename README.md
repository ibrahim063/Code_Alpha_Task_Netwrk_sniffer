
# 🕵️‍♂️ Network Sniffer CLI Tool

A lightweight, command-line based network packet sniffer built in Python using `scapy`. It allows you to capture and analyze network traffic in real-time directly from your terminal.

## 📦 Features

- Live packet capturing
- Filter by protocol (TCP, UDP, ICMP, etc.)
- Display source & destination IPs, ports, and packet summaries
- Option to save captured packets to a `.pcap` file
- Simple, readable CLI interface

## 🚀 Installation

1. **Clone the repository:**

```bash
git clone https://github.com/yourusername/network-sniffer-cli.git
cd network-sniffer-cli
````

2. **Install dependencies:**

Make sure you have Python 3.x installed.

```bash
pip install -r requirements.txt
```

> Note: You may need to run the script with elevated privileges (e.g., `sudo`) to capture packets.

## 🛠️ Usage

```bash
python sniffer.py [options]
```

### 📘 Options

| Option             | Description                                       |
| ------------------ | ------------------------------------------------- |
| `-i`, `--iface`    | Network interface to sniff on (e.g., `eth0`)      |
| `-p`, `--protocol` | Protocol filter (e.g., `tcp`, `udp`, `icmp`)      |
| `-c`, `--count`    | Number of packets to capture (default: unlimited) |
| `-w`, `--write`    | Save captured packets to `.pcap` file             |
| `-h`, `--help`     | Show help message                                 |

### 📎 Examples

Capture 10 TCP packets on `eth0`:

```bash
sudo python sniffer.py -i eth0 -p tcp -c 10
```

Capture all packets and save to file:

```bash
sudo python sniffer.py -i wlan0 -w output.pcap
```

## 🔒 Requirements

* Python 3.6+
* `scapy`
* Root/admin privileges for packet capturing

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

Created by [Muhammad Ibrahim](https://github.com/muhammadibrahim) — contributions welcome!

---

✅ If you find this useful, consider giving it a ⭐️!


