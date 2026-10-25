

## Bandit (0-15 done, now on 16)
- ls -a (hidden files), cat ./- (dash names), quotes for spaces
- file ./* (find readable file), find / -user -group -size 33c 2>/dev/null
- grep, sort | uniq -u, strings | grep "==", base64 -d
- tr 'A-Za-z' 'N-ZA-Mn-za-m' (ROT13: shift 13 twice = original)
- L12 loop: file > rename (.gz/.bz2) > gzip -d / bzip2 -d / tar xf > repeat
- L13: ssh -i keyfile (key file needs a final newline)
- L14: nc localhost 30000
- L15: openssl s_client -connect localhost:30001 (SSL = sealed envelope)
- L16: nmap -sV -p 31000-32000 localhost, find ssl ports, test each

## Mistakes and fixes
- Wrong username (each level has its own)
- mv only renames; tools need the right ending
- tar xf unpacks everything; > overwrites, >> appends
- Passwords stay in a private note, never GitHub

## What confused me
- tr and ROT13 mapping, tar vs gzip, SSL/TLS

## Next
- Finish Bandit 16, then 17-20
- Google cert Module 2
- Push notes to GitHub (no passwords)