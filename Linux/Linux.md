### rpm dependencies quering
RHEL-Based such as CentOS
```bash
repoquery --nvr --whatprovides cppcheck*
```
Fedora

```bash
dnf provides cppcheck
```
Or just let yum do the dirty work.
```bash
sudo yum install somePackage.rpm 
```

### Decompress
01. tar.bz2  
```
tar -xjvf *.tar.bz2
```

### Traffic related
01. replay pcap 
```
sudo tcpreplay -i wlp4s0 -tK --loop 1 --unique-ip web.pcap
```

### go get through local socks5 proxy
```
git config --global http.proxy socks5://127.0.0.1:1080
http_proxy=socks5://127.0.0.1:1080 go get -u github.com/gin-gonic/gin
```
revert git global configuration
```
git config --global --unset http.proxy
```
### Process Killing
```
ps -ef | grep some_process_name | grep -v | grep | awk '{print $2}' | xargs kill -9
```
