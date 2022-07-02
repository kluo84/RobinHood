# RobinHood
A Bug Hunting automation script for dreamers and low-hanging fruits

![](https://github.com/CalfCrusher/RobinHood/blob/main/RobinHood.jpg)

### Required Tools (you need to install those by yourself)

- SUBFINDER (https://github.com/projectdiscovery/subfinder)

- AMASS (https://github.com/OWASP/Amass)

- SUBLIST3R (https://github.com/aboul3la/Sublist3r)

- HTTPX (https://github.com/projectdiscovery/httpx)

- GF (https://github.com/1ndianl33t/Gf-Patterns)

- GAU (https://github.com/lc/gau)

- DALFOX (https://github.com/hahwul/dalfox)

- QSREPLACE (https://github.com/tomnomnom/qsreplace)

- SUBJACK (https://github.com/haccer/subjack)

- GOWITNESS (https://github.com/sensepost/gowitness)

- JSUBFINDER (https://github.com/ThreatUnkown/jsubfinder)

- NUCLEI (https://github.com/projectdiscovery/nuclei)

- NUCLEI TEMPLATE (https://github.com/projectdiscovery/nuclei-templates)

- SQLMAP (https://github.com/sqlmapproject/sqlmap)

- NMAP (https://github.com/nmap/nmap)

- CLOUDFLAIR (https://github.com/christophetd/CloudFlair)

- SCIPA_VULSCAN NSE (https://github.com/scipag/vulscan)

### API AND TOOLS LOCATIONS
*If you don't set those variables the related tools will not run!*

`BURP_COLLAB_URL="" # Burp Collaborator`

`FINGERPRINTS="" # Subjack fingerprints location`

`CLOUDFLAIR="" # CloudFlair tool location`

`CENSYS_API_ID="" # Censys api id for CloudFlair`

`CENSYS_API_SECRET="" # Censys api secret for CloudFlir`

`VULSCAN_NMAP_NSE="" # Vulscan NSE script for Nmap`

`JSUBFINDER_SIGN="" # Signature location for jsubfinder tool`

`NUCLEI_TEMPLATES="" # Directory template for Nuclei`

### Features

* Search for subdomains
* Search for live urls using gau
* Get screenshot of subdomains
* Search for secrets, token and APIs
* Scan live hosts with Nmap and Vulscan NSE Script
* Run Nuclei on all subdomains
* Try to get origin of IPs using CloudFlair
* Get interesting URLs for XSS, SSRF, SQLi, LFI
* Scan with Dalfox
* Scan with SQLMAP
* Test for basic LFI vulnerability
* Test for basi SSRF using burp.collaborator
* Search for subdomains takeover

### Usage

`$ git clone https://github.com/CalfCrusher/RobinHood/`

`$ cd RobinHood && chmod +x RobinHood.sh`

Run in background:

`$ nohup ./RobinHood.sh LARGE_SCOPE_DOMAIN 2>&1 &`

You can also give the out-of-scope domains list separated by commas:

`$ nohup ./RobinHood.sh example.com vpn.example.com,test.example.com 2>&1 &`

`$ tail -f nohup.out` to see progress output

