# learn-v8
v8 learning stuff

# disclaimer
please only use it for learning/testing purpose. I'm not responsible for any consequences done with illegal/unpermitted actions.

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
refer to my blog on v8: 
- https://y4y.space/2022/08/05/browser-exploitation-a-case-study-of-cve-2020-6507/
- https://y4y.space/2023/05/06/cve-2021-38001-a-brief-introduction-to-v8-inline-cache-and-exploitating-type-confusion/

# CVEs & exploits
all exploits are tested on Kali Linux 2021.1 / ubuntu 22.04 and my docker images (Ubuntu 20.04 base). all shellcodes in my exploits executes `execve("/bin/bash", null, null)`.

the table below shows CVE exploits and the corresponded v8 version I developed exploits on:

|CVE|V8 Version|
|---|---|
|CVE-2020-6507|8.3.110.9|
|CVE-2021-30632|9.3.345.16|
|CVE-2021-30517|9.0.257.23|
|CVE-2021-20220|8.9.255.24|
|CVE-2021-38001|9.5.172.21|

