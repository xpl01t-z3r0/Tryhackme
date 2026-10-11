```
ffuf -u http://10.49.181.208:8080/FUZZ \
-w /usr/share/seclists/Discovery/Web-Content/common.txt \
-fc 404
```
