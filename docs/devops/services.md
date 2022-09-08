## 


## Disable unnecessary services

```
systemctl stop binfmt-support && systemctl disable binfmt-support
systemctl stop apport && systemctl disable apport
systemctl stop atd && systemctl disable atd
systemctl stop varnish && systemctl disable varnish
systemctl stop varnishncsa && systemctl disable varnishncsa
systemctl stop dbus && systemctl disable dbus
systemctl stop collectd && systemctl disable collectd
```
