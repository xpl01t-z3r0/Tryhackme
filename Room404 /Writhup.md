```
ffuf -u http://10.49.181.208:8080/FUZZ \
-w /usr/share/seclists/Discovery/Web-Content/common.txt \
-fc 404
```
```
feroxbuster \
-u http://10.49.181.208:8080 \
-x php,html,js,json,txt \
-r
```
<img width="1972" height="1192" alt="image" src="https://github.com/user-attachments/assets/a8832bd9-7104-40f5-9879-5bcba340a0da" />
