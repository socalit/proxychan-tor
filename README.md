# proxychan-tor

Run any Linux command anonymously through [Tor](https://www.torproject.org/) using `proxychains` — with automatic Tor startup, IP rotation, and verification.

Built by [socalit](https://github.com/socalit) for quick privacy and recon tasks.

---

## Features

- Route any command through Tor's SOCKS5 proxy using `proxychains`
- Automatically requests a **new Tor circuit** (changes your Tor exit IP)
- Auto-installs Tor and ProxyChains if missing
- Updates `/etc/tor/torrc` to enable ControlPort for IP rotation
- Displays real IP vs Tor IP before running your command
- Works with: `curl`, `nmap`, `sqlmap`, `whois`, `git`, etc.

---
## Use it globally:

## proxychan curl https://ifconfig.me
## proxychan whois example.com
## proxychan nmap -Pn -sT scanme.nmap.org

---

## 🛠 Installation

```bash
git clone https://github.com/socalit/proxychan-tor.git
cd proxychan-tor
chmod +x proxychan
./proxychan --install
