# PaaSTA-EDU_20.3

# [1일차]

# [2일차]

## Pre-Reqs
실습환경 : Ubuntu 18.04

Vmware EXE Server => http://192.168.55.26/
ID/PW => root /JSlab123

https://github.com/PaaS-TA 접속

** https://github.com/PaaS-TA/Guide-4.0-ROTELLE/blob/master/Install-Guide/Bosh
 -> Bosh-Lite 설치 가이드 환경설정v2.0.md

1. Inception 서버 설치
ubuntu / 1234
Inception 서버 IP : 192.168.55.136

** https://github.com/PaaS-TA/Guide-4.0-ROTELLE/blob/master/Install-Guide/Bosh
 -> Bosh-Lite 설치 가이드v2.0.md
 
### Inception 서버 설치
```
$ sudo apt-get update
$ mkdir workspace
$ cd workspace
$ sudo apt-get install -y curl
$ curl -Lo ./bosh https://s3.amazonaws.com/bosh-cli-artifacts/bosh-cli-6.1.0-linux-amd64
$ chmod +x ./bosh
$ sudo mv ./bosh /usr/local/bin/bosh
$ bosh -v
```
### [dependency 설치]
[Ubuntu 18.04]
```
$ sudo apt-get install -y build-essential zlibc zlib1g-dev ruby ruby-dev openssl libxslt1-dev libxml2-dev libssl-dev libreadline7 libreadline-dev libyaml-dev libsqlite3-dev sqlite3
```

[다운로드]
```
$ wget http://45.248.73.44/index.php/s/Qi2zGPnGNEjb4Ax/download.zip
```

### [Bosh 환경 설정]
```
$ cd ~/workspace/paasta-5.0/deployment/bosh-deployment
$ chmod 755 *.sh
```
