# CyberX 🚀

```
 ██████╗██╗   ██╗██████╗ ███████╗██████╗ ██╗  ██╗
██╔════╝╚██╗ ██╔╝██╔══██╗██╔════╝██╔══██╗╚██╗██╔╝
██║      ╚████╔╝ ██████╔╝█████╗  ██████╔╝ ╚███╔╝ 
██║       ╚██╔╝  ██╔══██╗██╔══╝  ██╔══██╗ ██╔██╗ 
╚██████╗   ██║   ██████╔╝███████╗██║  ██║██╔╝ ██╗
 ╚═════╝   ╚═╝   ╚═════╝ ╚══════╝╚═╝  ╚═╝╚═╝  ╚═╝    

        CYBERX RECON FRAMEWORK
```

---

## 🧠 Overview

CyberX is a lightweight automated reconnaissance framework designed for bug bounty hunters and security researchers.

It connects multiple tools into a **structured pipeline**, ensuring clean and efficient scanning.

---

## 🔗 Workflow

```
Subdomain Enumeration
        ↓
Merge & Clean
        ↓
Alive Domains
        ↓
Port Scan
        ↓
Technology Detection
        ↓
JS Collection
        ↓
Screenshots + WAF Detection
```

---

## ⚡ Features

* 🔗 Chained pipeline (no wasted scans)
* ⚡ Fast execution using alive targets only
* 🧼 Clean output structure
* 🛠️ Uses industry-standard tools

---

## 🧰 Tools Used

* assetfinder
* amass
* subfinder
* httprobe
* naabu
* gau
* gowitness
* whatweb
* wafw00f

---

## 📦 Installation

Clone the repo:

```
git clone https://github.com/yourusername/cyberx.git
cd cyberx
```

Install dependencies:

```
go install github.com/tomnomnom/assetfinder@latest
go install github.com/projectdiscovery/subfinder/v2/cmd/subfinder@latest
go install github.com/projectdiscovery/naabu/v2/cmd/naabu@latest
go install github.com/lc/gau/v2/cmd/gau@latest
```

```
sudo apt install amass httprobe whatweb wafw00f
```

---

## 🚀 Usage

### Single Target

```
./cyberx.sh -t example.com
```

### Multiple Targets

```
./cyberx.sh -l domains.txt
```

---

## 📁 Output

```
cyberx_output/
└── target.com/
    ├── subdomains/
    ├── httprobe/
    ├── scans/
    ├── tech/
    ├── gau/
    ├── screenshots/
    └── waf/
```

---

## ⚠️ Disclaimer

For educational and authorized testing only.
Do not scan targets without permission.

---

## 👨‍💻 Author

Built by you.

---

## 🙌 Credits

This project is built upon the original ReconX framework developed by Sakibul Ali Khan.

CyberX introduces improvements in pipeline structuring, output chaining, and performance optimization while preserving the core reconnaissance logic.

Full credit goes to the original author for the base implementation.

---

## ⭐ Support

If you like this project, give it a star ⭐
