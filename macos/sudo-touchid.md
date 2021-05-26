# Enable TouchID for sudo

```shell
$ sudo vim /etc/pam.d/sudo

# add as a first line
auth sufficient pam_tid.so
```
