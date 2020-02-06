# BountyChecklist

Step 1 (scoping)
- (getting URLs which are available on the scope.)
- crt.sh
- Sublist3r

Is host alive?
#!/bin/bash
while read LINE; do
  curl -o /dev/null --silent --head --write-out "%{http_code} $LINE\n" "$LINE"
done < url-list.txt

screenshot live hosts:
- eyewitness
- Nmap is used to enumerate the host incase port is anything other than 80 for HTTP
