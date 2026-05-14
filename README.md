# 🛠️ Bug Bounty Toolkit

Curated collection of best-in-class bug bounty and penetration testing tools — recon, scanning, OSINT, exploitation, and red team tooling.

> All tools are added as **Git submodules** — clone with `--recurse-submodules` to get everything:
> ```bash
> git clone --recurse-submodules https://github.com/NyetNighy/bugbounty-toolkit.git
> ```

---

## 📂 What's Included

### 🔍 Recon & Automation
| Tool | Description |
|------|-------------|
| `reconftw/` | All-in-one automated recon — subdomains,端口扫描, screenshots, nuclei, vuln scan |
| `dirsearch/` | Fast directory and file brute-forcer |
| `ffuf/` | Blazingly fast web fuzzer written in Go |
| `gobuster/` | DNS/VHost/directory busting tool |

### 🐛 Vulnerability Scanning
| Tool | Description |
|------|-------------|
| `afrog/` | Security scanner for bug bounty — 20+ vuln classes, active development |
| `subjack/` | Automated subdomain takeover detection |

### 🌐 Subdomain Enumeration
| Tool | Description |
|------|-------------|
| `SubDomainizer/` | Find subdomains + secrets hidden in JS files |

### 🕵️ OSINT
| Tool | Description |
|------|-------------|
| `spiderfoot/` | Automated OSINT for threat intel and attack surface mapping |
| `maigret/` | Username dossier collector — checks 3000+ sites |
| `sherlock/` | Hunt down social media accounts by username |

### 🔴 Red Team / Infrastructure
| Tool | Description |
|------|-------------|
| `axiom/` | Dynamic infrastructure framework — distributes recon across cloud instances |

### 🛡️ Red Team Toolkit
| Tool | Description |
|------|-------------|
| `Red-Teaming-Toolkit/` | Curated collection of cutting-edge red team / threat hunter tools |

---

## 🏷️ Tags

`#bug-bounty` `#pentest` `#recon` `#osint` `#red-team` `#security` `#hacking`

---

## ⚡ Quick Install (Kali/Debian)

```bash
# Install core dependencies
sudo apt update && sudo apt install -y \
  golang-go python3 python3-pip ruby git curl wget \
  nmap masscan ffuf gobuster dirsearch

# Clone with all submodules
git clone --recurse-submodules https://github.com/NyetNighy/bugbounty-toolkit.git

# Individual tool setup
cd bugbounty-toolkit/afrog && go install
cd ../dirsearch && pip install -r requirements.txt
cd ../spiderfoot && pip install -r requirements.txt
```

---

## 📋 Requirements by Tool

| Tool | Language | Key Dependencies |
|------|----------|-------------------|
| reconftw | Shell/Python | amass, subfinder, naabu, nuclei, httpx |
| dirsearch | Python 3 | concurrent requests |
| ffuf | Go | Just Go (built binary) |
| afrog | Go | Just Go |
| subjack | Go | Just Go |
| SubDomainizer | Python 3 | requests, htmlтекст |
| spiderfoot | Python 3 | Elasticsearch (optional) |
| maigret | Python 3 | requests |
| sherlock | Python 3 | requests |
| axiom | Shell | Python, Docker, jq |
| gobuster | Go | Just Go |

---

## 🔧 Recommended Kali Packages

```bash
sudo apt install -y \
  build-essential golang-go python3-pip ruby git curl wget \
  nmap masscan dnsutils \
  exploitdb binaries dirmap \
  seclists curljq
```

---

*Maintained by Ori — contributions welcome 🌀*