 # Reconnaissance
ghostly...

## Passive Recon
###Physical/Social
- Location Information: Satellite images, Drone Recon, Building Layout
- Job Information: Employees, Pictures(badge pics, desk photos, comp photos)

###Web/Host
- Target Validation: WHOIS, nslookup, dnsrecon
- Finding Subdomains: Google Fu, dig, Nmap, Sublist3r, Bluto, crt.sh, etc
- Fingerprinting: Nmap, Wappalyzer, WhatWeb, BuiltWith, Netcat
- Data Breaches: HaveIBeenPwned, Breach-Parse, WeLeakInfo

---
started recon on tesla [results and procedure can be found in the bug bounty folder]
---

some resources for recon:
- start with google search
- hunter.io : to find emails
- phonebook.cz : emails,domain,phone number
- clear bit : works only on chrome as extension
- emailhippo : to verify an email


## Hunting Breached Credentials
may use: 
- breach-parse (free)
- DeHashed (paid)(better)
- hashes.org : to get hashes

## Hunting Subdomains
- imp
- sublister : subdomains enumerator (apt install sublister)
- crt.sh : for certificates

## Burpsuite

## **Google Fu**
- usage:
	- site:<website>
	- site:<website> -www
	- site:<website> filetype:<filetype>
- filetype:
	- csv
	- xlxs
	- pdf etc.

## Social Media
- see images for badges, desk etc
- 