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
### Process Killing
```
ps -ef | grep some_process_name | grep -v | grep | awk '{print $2}' | xargs kill -9
```
