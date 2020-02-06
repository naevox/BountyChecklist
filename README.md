# BountyChecklist

Step 1 (scoping)
- Domain scraping with: crt.sh, Sublist3r, censys

Is host alive?
#!/bin/bash
while read LINE; do
  curl -o /dev/null --silent --head --write-out "%{http_code} $LINE\n" "$LINE"
done < url-list.txt

- nmap -sn (ICMP) -Pn (treat all as online) -n (No DNS resolution) -iL <sublist.txt> -o output.txt
- add to scope on Burp for more features such as sitemap and HTML rendering of sites
- screenshot live hosts using: eyewitness
- visit hosts and enumerate manually
- Nmap is used to enumerate the host incase port is anything other than 80 for HTTP
- gobuster for subdomain enumeration
- wfuzz for possible attack manual enumeration
