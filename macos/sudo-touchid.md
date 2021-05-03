# Enable TouchID for sudo

```shell
$ vim /etc/pam.d/sudo

# add as a first line
auto sufficient pam_tid.so
```