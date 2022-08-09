# learn-v8
v8 learning stuff

# docker environment
currently doesn't have many versions. refer to https://hub.docker.com/r/brdns/v8/tags to see all available versions.

pulling images
```
docker pull brdns/v8:<version>
```

running images
```
docker run --rm -it brdns/v8:<version>
```
# notes
refer to my blog on v8: https://y4y.space/2022/08/05/browser-exploitation-a-case-study-of-cve-2020-6507/

# CVEs & exploits
all exploits are tested on Kali Linux 2021.1 and my docker images (Ubuntu 20.04 base). all shellcodes in my exploits executes `execve("/bin/bash", null, null)`.

the table below shows CVE exploits and the corresponded v8 version I developed exploits on:

|CVE|V8 Version|
|---|---|
|CVE-2020-6507|8.3.110.9|
|CVE-2021-30632|9.3.345.16|

