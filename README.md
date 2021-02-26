# abusing-suid
A tool to detect vulnerable SUIDs on any machine.

---

# Disclaimer
This tool is designed to automatically detect SUID vulnerabilities by providing a hint about a possible payload,
it is not addressed to those who want to destroy but to those who want to research and mitigate.  
Use it at your discretion, better if you know that me and whoever contributed, **we take no responsibility for this**.  

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