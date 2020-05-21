# BountyChecklist

ADD THESE TOOLS
https://www.youtube.com/watch?v=1J7dWJMEnl8

https://github.com/s0md3v/Striker

Step 1 (scoping)
- Domain scraping with: crt.sh, Sublist3r, censys
- nmap default port scan for host discovery
- nmap -sn (ICMP) -Pn (treat all as online) -n (No DNS resolution) -iL <sublist.txt> -o output.txt
- add to scope on Burp for more features such as sitemap and HTML rendering of sites
- screenshot live hosts using: eyewitness
- visit hosts and enumerate manually
- Nmap is used to enumerate the host incase port is anything other than 80 for HTTP
- gobuster for subdomain enumeration
- wfuzz for possible attack manual enumeration

Finding IP spaces (domain scraping)
- bgp.he.net - search internet services by key word for whois enumeration.
- https://www.arin.net/
- https://www.ripe.net/
- https://reverse.report/
- Shodan to search for sites which have key words

Acquisitions (side companies which may be in scope)
- Wikipedia
- crunchbase

Linked discovery
- Burp (using burp while navigating the website will spider the website passively)
