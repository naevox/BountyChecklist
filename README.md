# bbChecklist

Scoping:
- crt.sh
- Sublist3r

Is host alive?

#!/bin/bash
while read LINE; do
  curl -o /dev/null --silent --head --write-out "%{http_code} $LINE\n" "$LINE"
done < url-list.txt
