# fixtime
#### Crude time-reset-on-poweroff fix

Simple script that periodically syncronizes clock with time.nist.gov and saves current time to file.
When computer starts up it tries to sync with ntp, or restores time from file, which later will be fixed with ntp sync.

to build package run
```shell
dpkg-deb --build fixtime
```
    
and then install
```shell
sudo dpkg -i fixtime.deb
```

