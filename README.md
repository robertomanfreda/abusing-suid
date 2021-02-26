# abusing-suid
A tool to detect vulnerable SUIDs on any machine.

---

# Disclaimer
This tool is designed to automatically detect SUID vulnerabilities by providing a hint about a possible payload,
it is not addressed to those who want to destroy but to those who want to research and mitigate.  
Use it at your discretion, better if you know that me and whoever contributed, **we take no responsibility for this**.  

---

#Example output

```
------------------------------
10 possible vulnerabilities
------------------------------
-rwsr-xr-x  1  root  root  31032  ago  16  2019   /usr/bin/pkexec                 https://gtfobins.github.io/gtfobins/pkexec/  pkexec
-rwsr-xr-x  1  root  root  55528  lug  21  2020   /usr/bin/mount                  https://gtfobins.github.io/gtfobins/mount/   mount
-rwsr-xr-x  1  root  root  43088  set  16  20:43  /snap/core18/1988/bin/mount     https://gtfobins.github.io/gtfobins/mount/   mount
-rwsr-xr-x  1  root  root  40152  gen  27  2020   /snap/core/10823/bin/mount      https://gtfobins.github.io/gtfobins/mount/   mount
-rwsr-xr-x  1  root  root  55528  lug  21  2020   /snap/core20/904/usr/bin/mount  https://gtfobins.github.io/gtfobins/mount/   mount
-rwsr-xr-x  1  root  root  31032  ago  16  2019   /usr/bin/pkexec                 https://gtfobins.github.io/gtfobins/pkexec/  pkexec
-rwsr-xr-x  1  root  root  67816  lug  21  2020   /usr/bin/su                     https://gtfobins.github.io/gtfobins/su/      su
-rwsr-xr-x  1  root  root  44664  mar  22  2019   /snap/core18/1988/bin/su        https://gtfobins.github.io/gtfobins/su/      su
-rwsr-xr-x  1  root  root  40128  mar  25  2019   /snap/core/10823/bin/su         https://gtfobins.github.io/gtfobins/su/      su
-rwsr-xr-x  1  root  root  67816  lug  21  2020   /snap/core20/904/usr/bin/su     https://gtfobins.github.io/gtfobins/su/      su

```
---

# Usage

## Latest release
```shell
git clone https://github.com/robertomanfreda/abusing-suid.git
cd abusing-suid
cd bin
./find_exploitable_suids
```

## Specific release
```shell
curl 'https://codeload.github.com/robertomanfreda/abusing-suid/tar.gz/1.0.0' --output abusing-suid.tar.gz
tar -xzvf abusing-suid.tar.gz
cd abusing-suid-<version> 
cd bin
./find_exploitable_suids
```

---