<p align="center">
  <img src="assets/banner.png" alt="Lenovo WiFi Whitelist Remover" width="100%">
</p>

[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-support-%23FFDD00?logo=buymeacoffee&logoColor=black)](https://buymeacoffee.com/socal370xs)

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

## Installation

```bash
git clone https://github.com/socalit/proxychan-tor.git
cd proxychan-tor
chmod +x proxychan
./proxychan --install
```
## Support

### ⭐ **Star the GitHub repo**  
### Share it with communities  
### Open issues or request features  

If this project saved you time or solved a problem, consider supporting development:

[![Buy Me a Coffee](https://img.buymeacoffee.com/button-api/?text=Buy%20me%20a%20coffee&slug=socal370xs&button_colour=FFDD00&font_colour=000000&font_family=Arial&outline_colour=000000&coffee_colour=ffffff)](https://buymeacoffee.com/socal370xs)
