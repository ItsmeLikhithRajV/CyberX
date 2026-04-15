🚀 CyberX – Automated Reconnaissance Framework
   ______      __                __  __
  / ____/___  / /_  ____  ____  / /_/ /
 / /   / __ \/ __ \/ __ \/ __ \/ __/ / 
/ /___/ /_/ / /_/ / /_/ / /_/ / /_/ /  
\____/\____/_.___/\____/\____/\__/_/   

        CYBERX RECON FRAMEWORK
🧠 Overview

CyberX is a lightweight, automated reconnaissance pipeline designed for bug bounty hunters and security researchers.

It chains multiple industry-standard tools into a structured workflow, ensuring that each step feeds into the next — eliminating noise and improving efficiency.

🔗 Pipeline Flow
Subdomain Enumeration
        ↓
Merge & Deduplicate
        ↓
Alive Domain Detection
        ↓
Port Scanning
        ↓
Technology Detection
        ↓
JS Collection
        ↓
Screenshots + WAF Detection
⚡ Features
🔗 Chained Workflow – Each stage feeds the next (no wasted scans)
⚡ Fast & Efficient – Only scans alive targets
🧼 Clean Output Structure
🧠 Beginner-Friendly + Pro-Level Design
🛠️ Uses top recon tools in one pipeline
🧰 Tools Used

CyberX integrates:

assetfinder
amass
subfinder
httprobe
naabu
gau
gowitness
whatweb
wafw00f
📦 Installation
1. Clone the repository
git clone https://github.com/yourusername/cyberx.git
cd cyberx
2. Install dependencies

Make sure all required tools are installed:

go install github.com/tomnomnom/assetfinder@latest
go install github.com/projectdiscovery/subfinder/v2/cmd/subfinder@latest
go install github.com/projectdiscovery/naabu/v2/cmd/naabu@latest
go install github.com/lc/gau/v2/cmd/gau@latest

Also install:

sudo apt install amass httprobe whatweb wafw00f
🚀 Usage
🔹 Scan a single domain
./cyberx.sh -t example.com
🔹 Scan multiple domains
./cyberx.sh -l domains.txt
📁 Output Structure
cyberx_output/
└── example.com/
    ├── subdomains/
    │   ├── final.txt
    ├── httprobe/
    │   ├── alive.txt
    ├── scans/
    │   ├── ports.txt
    ├── tech/
    │   ├── tech.txt
    ├── gau/
    │   ├── js.txt
    ├── screenshots/
    ├── waf/
    │   ├── waf.txt
🧪 Example Workflow
./cyberx.sh -t example.com

✔ Finds subdomains
✔ Filters alive domains
✔ Scans ports
✔ Detects technologies
✔ Collects JS files
✔ Captures screenshots
✔ Identifies WAF

⚠️ Disclaimer

CyberX is intended for educational purposes and authorized testing only.

Do not use this tool on systems without proper permission.

👨‍💻 Author
Developed by You
Inspired by modern bug bounty workflows
🌟 Future Improvements
🔥 Parallel execution (faster scans)
📊 HTML report generation
🧠 Vulnerability detection modules
💾 Resume scan capability
⭐ Support

If you like this project:

⭐ Star the repo
🍴 Fork it
🛠️ Contribute
💬 Final Note

CyberX is not just a script — it’s a structured recon workflow built to think like a hacker.
