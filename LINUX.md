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


